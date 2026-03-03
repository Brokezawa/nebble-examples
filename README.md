# Nebble Examples

[![CI](https://github.com/Brokezawa/nebble-examples/actions/workflows/ci.yml/badge.svg)](https://github.com/Brokezawa/nebble-examples/actions/workflows/ci.yml)

A collection of example applications and watchfaces demonstrating the [Nebble](https://github.com/Brokezawa/nebble) framework for Pebble smartwatch development.

## 🚀 Quick Start

### Prerequisites

- [Nim](https://nim-lang.org/) 2.2.0 or later
- [Pebble SDK](https://developer.rebble.io/developer.pebble.com/sdk/index.html)
- [Nebble](https://github.com/Brokezawa/nebble) v1.1.0 or later

```bash
# Install Nebble
nimble install nebble

# Clone this repository
git clone https://github.com/Brokezawa/nebble-examples
cd nebble-examples

# Build an example
cd hello_world
nebble build

# Install on emulator
nebble install --emulator basalt
```

## 📚 Examples

These examples demonstrate Nebble-idiomatic Nim patterns for Pebble development. Each example focuses on a specific feature not covered by the ported Pebble SDK examples.

**For C parity examples**, see the [ported-examples](https://github.com/Brokezawa/ported-examples) repository, which contains official Pebble SDK examples ported to Nim (simple_analog, ks_clock_face, battery display, accelerometer, persistence, etc.).

| Example | Type | Description | Key Features |
|---------|------|-------------|--------------|
| **hello_world** | App | Minimal entry point | Declarative DSL, text rendering, click handling |
| **animation_demo** | App | Property animation patterns | AnimationHandle, sequences, event-driven tweens |
| **comms_demo** | App | Full-stack communication | AppMessage, phone-side Nim (PKJS), typed messaging |
| **health_watchface** | Watchface | Health data display | Health service, activity metrics, background data |
| **glance_menu_demo** | App | App Glance + menus | AppGlance API, dynamic menu callbacks, timeline integration |
| **menu_demo** | App | Menu layer patterns | SimpleMenuLayer, sections, selection handling |
| **vibes_demo** | App | Haptic feedback | Vibes API, vibration patterns, user interaction |

## 🏗️ Project Structure

Each example follows the standard Nebble project layout:

```
example_name/
├── src/
│   └── example_name.nim       # Main application code
├── resources/                  # Images, fonts, etc.
├── package.json               # Pebble SDK app metadata
├── wscript                    # Build configuration
└── nim.cfg                    # Nim compiler settings
```

## 🛠️ Building Examples

### Build for all platforms
```bash
nebble build
```

### Build for specific platform
```bash
nebble build --platform basalt    # Pebble Time
nebble build --platform aplite    # Original Pebble
nebble build --platform chalk     # Pebble Time Round
nebble build --platform diorite   # Pebble 2
nebble build --platform emery     # Pebble Time 2
nebble build --platform flint     # Rebble-ready devices
```

### Install on device
```bash
nebble install --phone <IP_ADDRESS>
```

### Install on emulator
```bash
nebble install --emulator basalt
```

## 📖 Documentation

- [Nebble Documentation](https://brokezawa.github.io/nebble/)
- [Nebble GitHub](https://github.com/Brokezawa/nebble)
- [Pebble Developer Documentation](https://developer.rebble.io/)
- [Nim Language](https://nim-lang.org/documentation.html)

## 🤝 Contributing

Contributions are welcome! To add a new example:

1. Fork this repository
2. Create a new directory with your example
3. Include a clear README.md explaining what the example demonstrates
4. Ensure it builds for all platforms
5. Submit a pull request

### Example Guidelines

- Keep examples focused on one concept
- Include comments explaining key parts
- Use consistent naming conventions
- Test on multiple platforms if possible
- Include a screenshot if applicable

## 📄 License

This repository is licensed under the MIT License. See [LICENSE](LICENSE) for details.

Individual examples may contain their own licenses. Check each example's directory for specifics.

## 🔗 Related Projects

- [Nebble](https://github.com/Brokezawa/nebble) - The main framework
- [Pebble SDK](https://github.com/pebble/pebble-sdk) - Official SDK
- [Rebble](https://rebble.io/) - Pebble community revival

## 💬 Support

- [GitHub Issues](https://github.com/Brokezawa/nebble-examples/issues) - Bug reports and feature requests
- [GitHub Discussions](https://github.com/Brokezawa/nebble/discussions) - General questions and community

---

Made with ❤️ for the Pebble community
