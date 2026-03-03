# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2026-03-03

### Added

- This is the first public release of nebble-examples as a separate repository.
  Previously, examples were part of the main nebble package (`examples/` directory).
- 7 Nebble-idiomatic examples:
  - **hello_world**: Minimal declarative app using the `nebbleApp` DSL
  - **animation_demo**: Property animation patterns with `AnimationHandle`
  - **comms_demo**: Full-stack AppMessage communication with phone-side Nim (PKJS)
  - **health_watchface**: Health service integration and activity metrics
  - **glance_menu_demo**: App Glance API and dynamic menu callbacks
  - **menu_demo**: `SimpleMenuLayer` patterns and selection handling
  - **vibes_demo**: Haptic feedback and vibration patterns
- Requires nebble >= 1.1.0

[1.1.0]: https://github.com/Brokezawa/nebble-examples/releases/tag/v1.1.0
