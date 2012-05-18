#Lines

Lines is a bash script that will count the number of lines of text present in a directory and return that number to you.

##Usage

    Usage: lines [directory]

    $ lines
    Found 562 lines of text in .
    $ lines test-project
    Found 2287 lines of text in test-project/

##Installing Lines

My personal preference is to create a symbolic link between `lines` and
`/usr/bin/lines`. This way, the command is accessible to all users of the
computer, but still remains within the repository for easy updates. An example
of how to do this follows:

    // make the command executable
    $ chmod +x lines
    
    // create the symbolic link (cannot be a relative path)
    $ sudo ln -s <full path to this repository>/lines /usr/bin/lines