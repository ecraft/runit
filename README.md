Fork of Gerrit Pape's init [`runit`](http://smarden.org/runit/)

Shutdown on `SIGTERM` to make runit more docker-friendly.

~When docker 1.11 drops this will be redundant since docker will actually use `STOPSIGNAL` from your `Dockerfile`.~ It has been released for over a year, and after https://github.com/ecraft/bep-baseimage/pull/51 is rolled out, this code is not used. It is forked here just to preserve it while it is being used, since the original author of the fix ([@qzio](https://github.com/qzio)) has left eCraft and we don't want to be dependent on repositories out of our control.

* Reported: https://github.com/docker/docker/issues/19300
* Fix: https://github.com/docker/docker/pull/20290
