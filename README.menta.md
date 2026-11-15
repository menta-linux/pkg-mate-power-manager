# pkg-mate-power-manager (Menta Linux)

Debian packaging of mate-power-manager 1.28.1 (from debian-mate-team on Salsa,
1.26.1-1.1). Version scheme: `<upstream>-<rev>mentaN`, bump with `dch -i`.

Changes: `0001_in-process-applets.patch` builds the Brightness and Inhibit panel
applets as in-process modules (`InProcess=true`, `Platforms=X11;Wayland;`).
Upstream has no Wayland build option. The session daemon, preferences,
statistics tools and the pkexec backlight helper are standalone programs and
stay separate processes.

CI builds on pushes to `master`; a `menta/<version>` tag publishes a release.
