# pkg-mate-power-manager (Menta Linux)

Debian packaging of a mate-power-manager git snapshot (upstream master, 1.29.0+; base from
debian-mate-team on Salsa). Version scheme: `<upstream>+git<date>.<sha>-<rev>mentaN`; CI clones
upstream and checks out `<sha>`.

Changes: meson build with `-Denable-wayland=true`, `-Dapplets-in-process=true` and
`-Dappindicator=enabled` (StatusNotifierItem tray icon via libayatana-appindicator). No patches.

CI builds on pushes to `master`; a `menta/<version>` tag publishes a release.
