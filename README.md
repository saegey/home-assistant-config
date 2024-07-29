# Home Assistant Configuration

Welcome to my Home Assistant configuration repository. This repository contains the configuration files for my Home Assistant setup.

## Introduction

Home Assistant is an open-source home automation platform that focuses on privacy and local control. This repository is used to manage and version control my Home Assistant configuration, making it easier to maintain, back up, and share.

## Getting Started

### Prerequisites

To use this configuration, you need to have Home Assistant installed. You can find installation instructions on the [Home Assistant website](https://www.home-assistant.io/installation/).

### Cloning the Repository

Clone this repository to your Home Assistant configuration directory:

```sh
git clone https://github.com/saegey/home-assistant-config.git
```

### Configuration

Before using the configuration, make sure to update the secrets and customize the settings according to your environment.

1. **Secrets File**: Create a `secrets.yaml` file in the root directory to store sensitive information like passwords and API keys. Here's an example:

```yaml
# secrets.yaml
mariadb_connection_string: your_mariadb_connection_string
influxdb_password: your_influxdb_password
```

2. **Configuration File**: Update the `configuration.yaml` file with your specific settings and preferences.

## Folder Structure

The repository is organized as follows:

```
home-assistant-config/
├── configuration.yaml     # Main configuration file
├── secrets.yaml           # Sensitive information (not included in the repo)
├── automations.yaml       # Automations configuration
├── scripts.yaml           # Scripts configuration
├── scenes.yaml            # Scenes configuration
├── groups.yaml            # Groups configuration
├── custom_components/     # Custom components
├── www/                   # Static files
├── esphome/               # ESPHome device configurations
└── README.md              # This file
```

## ESPHome Configurations

The `esphome` directory contains the configurations for ESPHome devices. Each device has its own YAML file. For example:

```yaml
# esphome/secrets.yaml

wifi_ssid: your_wifi_ssid
wifi_password: your_wifi_password

esphome_password: your_esphome_password
esphome_fallback_wifi_password: your_esphome_fallback_wifi_password

api_encrypt: your_api_encrypt
```

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Make your changes and commit them (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to customize this template further to suit your specific needs and preferences.
