CHANGES
=======

0.4
---
???next release


0.3.4 - 2012-05-30
------------------

- Fixed a race condition that prevented the controller
  to cleanly reap finished processes.
- Now check_flapping can be controlled in the configuration.
  And activated/deactivated per watcher.


0.3.3 - 2012-05-29
------------------

- Fixed the regression on the uid handling

0.3.2 - 2012-05-24
------------------

- allows optional args property to add_watcher command.
- added circushttpd, circus-top and circusd-stats
- allowing Arbiter.add_watcher() to set all Watcher option
- make sure the redirectors are re-created on restarts


0.3.1 - 2012-04-18
------------------

- fix: make sure watcher' defaults aren't overrided
- added a StdoutStream class.

0.3 - 2012-04-18
----------------

- added the streaming feature
- now displaying coverage in the Sphinx doc
- fixed the way the processes are killed (no more SIGQUIT)
- the configuration has been factored out
- setproctitle support


0.2 - 2012-04-04
----------------

- Removed the *show* name. replaced by *watcher*.
- Added support for setting process **rlimit**.
- Added support for include dirs in the config file.
- Fixed a couple of leaking file descriptors.
- Fixed a core dump in the flapping
- Doc improvments
- Make sure circusd errors properly when another circusd
  is running on the same socket.
- get_arbiter now accepts several watchers.
- Fixed the cmd vs args vs executable in the process init.
- Fixed --start on circusctl add


0.1 - 2012-03-20
----------------

- initial release
