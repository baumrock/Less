# 0.0.8

- Added Wikimedia LESS v5.5.0 with PHP 8.5 compatibility fixes.
- Backported comma-separated selector lists in pseudo-classes (`:is()`, `:not()`, `:where()`, `:has()`) from [elabx/less.php#1](https://github.com/elabx/less.php/pull/1) to bundled less.php 5.5.0.

# 0.0.7

- Backport comma-separated selector lists in pseudo-classes (`:is()`, `:not()`, `:where()`, `:has()`) from [elabx/less.php#1](https://github.com/elabx/less.php/pull/1) (Less.js 4.2 / wikimedia/less.php#136) to bundled less.php 4.1.1 and 5.4.0.
- Backport native CSS color function passthrough (e.g. `rgba(0, 0, 0, var(--opacity))`) from wikimedia/less.php 5.5.0 (T405815) to bundled less.php 4.1.1 and 5.4.0.

# 0.0.6

- Added Wikimedia LESS v5.4.0 in addition to existing v4.1.1.
- Made LESS version selectable in module config.
- Made it auto select newest supported version when installing module.
- Note: if upgrading it will use 4.1.1 unless you select newer version in module config.