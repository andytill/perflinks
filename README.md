# Erlang Performance Links

Nuggets of erlang performance wisdom, from those kind enough to share.

## EProf

[eprof](http://www.erlang.org/doc/man/eprof.html) attaches to a running process and and can produces a flat list of functions that are most called, and took the most time.

 + [Quick start](http://stackoverflow.com/a/4354188/1673868)

## FProf

[fprof](http://www.erlang.org/doc/man/fprof.html) attaches to a running process, like eprof but gives a hierarchical breakdown of function calls counts and their total time.  Useful when there are several calls throughout a process but it is not clear which one is taking the most time.

 + [Quick start](http://timanovsky.wordpress.com/2009/01/20/profiling-running-erlang-server/)
 + [erlgrind](https://github.com/isacssouza/erlgrind) converts fprof output into valgrind format that can be visualised using [KCacheGrind](http://kcachegrind.sourceforge.net/html/Home.html).

This is still a WIP.
