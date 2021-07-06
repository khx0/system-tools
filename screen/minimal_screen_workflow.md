# Minmal screen workflow

This section describes how a minimal screen workflow can look like.

1) Start a new named screen session.
```bash
screen -S <SESSION_NAME>
```
This will attach you to this new named session `<SESSION_NAME>`.

2) Do work in this session, *e.g.*, start a processing job which might take longer.

3) Detach from the currently active session.
Type
```
Ctrl + A, d
```
to detach.

4) Check for screen sessions using
```bash
screen -ls
```
This should list you the session `<SESSION_NAME>` as a currently still running but detached session.

5) Rejoin / resume (named) session. Type
```bash
screen -r <SESSION_NAME>
```
for the re-joining / resuming (re-attaching) the session `<SESSION_NAME>`.

6) Close screen session.
To quit a currently active (attached) screen session, type
```bash
exit.
```
