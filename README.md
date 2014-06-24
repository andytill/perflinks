# Erlang Performance Links

Nuggets of erlang performance wisdom, from those kind enough to share.

## EProf

[eprof](http://www.erlang.org/doc/man/eprof.html) attaches to a running process and and can produces a flat list of functions that are most called, and took the most time.

 + [Quick start](http://stackoverflow.com/a/4354188/1673868)

## FProf

[fprof](http://www.erlang.org/doc/man/fprof.html) attaches to a running process, like eprof but gives a hierarchical breakdown of function calls counts and their total time.  Useful when there are several calls throughout a process but it is not clear which one is taking the most time.

 + [Quick start](http://timanovsky.wordpress.com/2009/01/20/profiling-running-erlang-server/)
 + [erlgrind](https://github.com/isacssouza/erlgrind) converts fprof output into valgrind format that can be visualised using [KCacheGrind](http://kcachegrind.sourceforge.net/html/Home.html).

## Beyond OTP

Loïc Hoguin achieves LOLSPEED in cowboy by ditching OTP behaviours and rolling his own, OTP compliant processes in critical parts of the code.

 + [Slides](http://ninenines.eu/talks/beyond-otp/beyond-otp.html)
 + [Video presentation](http://youtu.be/fyobN-6YyJY)

## Networking

 + [inet options](http://www.erlang.org/doc/man/inet.html#setopts-2)

## Message Batching

@ostinelli benchmarks message batching inside application code (as opposed to the TCP stack).

 + [Blog](http://www.ostinelli.net/boost-message-passing-between-erlang-nodes/)
 + [Code](https://github.com/davide/erlang_mq_boost)

This is still a WIP.
