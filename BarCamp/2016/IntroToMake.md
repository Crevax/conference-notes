What is Make?
Build Automation tool
    Create an executable from source code
    Update files automatically when related files change

Filename: Makefile
    Uses commands to make targets from files

Books:
    ManaginG Projects with GNU Make

Why use Make?
    It doesn't have the bootstrapping problems like Grunt, Gulp, etc.
        How to install dependencies?
    More robust depedency tracking
    Less overhead when switching projects
        One has Gulp, another has Grunt, etc.
    Make is self-contained
        No dependencies to run
    Has established conventions for functions
        Make
        Make clean
        Make test
    CI Servers can digest them more easily
    Easier build debugging
        Each steps are in isolated chunks that can be executed individually

Make checks files and timestamps to see what needs to be created and/or updated

Variables in Make
    CONSTANT := value
    LAZY = $(shell ls *.py) -- only evaluated when it's used
    OPTIONAL ?= value2 -- can be overridden when executing make commands
    -- Automatic variables --
        $@ -- Name of the target
        $< -- All of the dependencies
        $^ -- First dependency

Examples
`
BE := bundle executable

JEKYLL := $(BE) jekyll

.PHONY: install
`

Has the same quicks and shell scripting quirks (using tabs in the Makefile, no spaces in file names, etc)
