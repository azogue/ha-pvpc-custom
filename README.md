[![hacs_badge](https://img.shields.io/badge/HACS-Custom-41BDF5.svg)](https://github.com/hacs/integration)
![Validate with hassfest](https://github.com/azogue/ha-pvpc-custom/workflows/Validate%20with%20hassfest/badge.svg)
![HACS Validation](https://github.com/azogue/ha-pvpc-custom/workflows/HACS%20Validation/badge.svg)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
[![pre-commit.ci Status](https://results.pre-commit.ci/badge/github/azogue/ha-pvpc-custom/main.svg)](https://results.pre-commit.ci/latest/github/azogue/ha-pvpc-custom/main)

<br><a href="https://www.buymeacoffee.com/azogue" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-black.png" width="150px" height="35px" alt="Buy Me A Coffee" style="height: 35px !important;width: 150px !important;" ></a>

# Spain electricity hourly pricing

Custom integration _mirroring_ [official HA-Core integration](https://www.home-assistant.io/integrations/pvpc_hourly_pricing),
to be able to apply changes **quicker** than the normal release flow for HA Core.

## Installation

### HACS _(preferred method)_

**Add the integration in [HACS](https://hacs.xyz/)** by adding a custom repository:

```
Repository: "https://github.com/azogue/ha-pvpc-custom"
Category: "Integration"
```

### Manual install

Place the `custom_components` folder in your configuration directory
(or add its contents to an existing `custom_components` folder).
