# Nebble Examples

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

### Beginner

| Example | Description | Concepts |
|---------|-------------|----------|
| **hello_world** | Basic app with text layer | App structure, text rendering |
| **simple_watchface** | Minimal watchface | Time display, watchface basics |
| **battery_status** | Display battery level | System events, status bar |
| **vibes_demo** | Vibration patterns | Haptic feedback |

### Intermediate

| Example | Description | Concepts |
|---------|-------------|----------|
| **graphics_demo** | Drawing primitives | Shapes, bitmaps, paths |
| **menu_demo** | Menu layer usage | Navigation, callbacks |
| **action_bar_demo** | Action bar patterns | UI controls, icons |
| **persist_demo** | Data persistence | Storage, settings |
| **animation_demo** | Property animations | Transitions, tweens |

### Advanced

| Example | Description | Concepts |
|---------|-------------|----------|
| **accelerometer_demo** | Motion sensing | Sensors, data processing |
| **comms_demo** | AppMessage communication | Phone connectivity, serialization |
| **health_watchface** | Health data display | Activity tracking, permissions |
| **glance_menu_demo** | App Glance integration | Timeline, menu actions |

## 🏗️ Project Structure

Each example follows the standard Nebble project layout:

```
example_name/
├── src/
│   └── example_name.nim       # Main application code
├── resources/                  # Images, fonts, etc.
├── nebble.json                # Nebble configuration
├── package.json               # Pebble app metadata
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
