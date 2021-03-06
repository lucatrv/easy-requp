# Easy ReqUp

Easily manage Python packages based on requirements file specifications.

Run `python -m easy_requp -h` for help:

```
usage: python -m easy_requp [-h] [-V] [-v] [-q] [-y] [-s] [-r FILE]
                            [-a ACTION [ACTION ...]] [-n] [-u]
                            [-o OPTION [OPTION ...]] [-m N] [-d] [-c LIMIT]

Easily manage Python packages based on requirements file specifications.

optional arguments:
  -h, --help            show this help message and exit
  -V, --version         show version information and exit
  -v, --verbose         let pip give more output, option is additive and can be
                        used up to 3 times, try 'pip help' for more information
  -q, --quiet           let pip give less output, option is additive and can be
                        used up to 3 times, try 'pip help' for more information
  -y, --yes             don't ask for confirmations
  -s, --skip-python-version-check
                        don't check for Python updates
  -r FILE, --requirement FILE
                        install from the given requirements file, try 'pip help
                        install' for more information (default: easy_requp.txt)
  -a ACTION [ACTION ...], --actions ACTION [ACTION ...]
                        perform selected actions: all, reqs, deps, orph, check,
                        clean (default: all)
  -n, --not             invert actions selection
  -u, --user            pass the --user flag to pip, try 'pip help install' for
                        more information
  -o OPTION [OPTION ...], --options OPTION [OPTION ...]
                        additional pip options, escape leading '-' character
                        with '\', try 'pip help' for more information
  -m N, --max-pip-retries N
                        maximum number of retries if pip fails (default: 3)
  -d, --deps_complete   repeat dependencies upgrade until no changes are
                        detected
  -c LIMIT, --cache LIMIT
                        clean cache if folder size is above given limit, in MB
                        (default: 200)

examples:
  python -m easy_requp                  # full system upgrade
  python -m easy_requp -r FILE          # use given requirements file
  python -m easy_requp -a reqs          # upgrade required packages
  python -m easy_requp -na clean        # do not clean pip cache
  python -m easy_requp -u               # pass --user flag to pip
  python -m easy_requp -uo \--log PATH  # pass --user and --log flags to pip

Report any bugs to: <https://github.com/lucatrv/easy-requp>
```
