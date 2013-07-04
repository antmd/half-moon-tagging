# tag

## Danger

Here be dragons. You use this at your own risk.

## Install

    pip install --user git+https://github.com/schwa/half-moon-tagging.git
    
## Usage

    $ tag -h
    tag - Mavericks command line tool for tagging files

    Usage:
      tag --list <path>...
      tag --add <tag> <path>...
      tag --set <tag> <path>...
      tag --remove <tag> <path>...
      tag (-h | --help)
      tag --version

    Options:
      -l --list          List all tags at each path
      -a --add=<tag>     Add one or more (comma separated) tags to paths
      -s --set=<tag>     Set one or more (comma separated) tags on paths
      -r --remove=<tag>  Remove one or more (comma separated) tags from paths
      -h --help          Show this screen.
      --version          Show version.
    $ touch example.txt
    $ tag --list example.txt
    example.txt ()
    $ tag --set Green example.txt
    $ tag --list example.txt
    example.txt (Green)
    $ tag --add Examples example.txt
    $ tag --list example.txt
    example.txt (Green, Examples)
    $ tag --set Red,Green,Purple example.txt
    $ tag --list example.txt
    example.txt (Red, Green, Purple)

## License
    
    BSD 2-clause

