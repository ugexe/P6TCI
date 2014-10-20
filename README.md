## Demonstrate Perl6 module testing on Travis-CI

### HOWTO

Just copy the .travis.yml file from this repo to yours and turn on testing for that repository on Travis-CI.org

### TODO

######bin/p6tci

Generate a .travis.yml in some location based on some arguments.

* Option to use rakudobrew to test all $ENV{BACKEND}s in one job. However if any of the backends fail it will result in a failure for the job as a whole and you'll have to actually look at the build history to see what failed.

* Run tests in parallel with prove -j like the [Travis-CI testing helper for Perl modules](https://github.com/travis-perl/helpers)
