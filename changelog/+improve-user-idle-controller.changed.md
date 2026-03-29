Added ``reset`` field to `UserIdleTimeoutUpdateFrame` (default ``False``). When
``True``, the frame ignores ``timeout`` and restores `UserIdleController` to
the timeout it was initialised with. If the current state warrants it (bot not
speaking, no user turn in progress, no pending function calls) the idle timer
is started immediately after restoring.
