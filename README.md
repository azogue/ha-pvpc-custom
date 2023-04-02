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
