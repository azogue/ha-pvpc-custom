# Changelog

## [v1.1.0](https://github.com/azogue/ha-pvpc-custom/tree/v1.1.0) 🐛 Fixes for new extra price sensors (2023-05-29)

- 🐛 Fix all integration sensors going unavailable when any sensor lacks data for the current day (usually the 'OMIE price')
- 🐛 Fix 'max_price_at' and 'min_price_at' for injection price sensor (were swapped), by updating to [`aiopvpc` v4.2.1](https://github.com/azogue/aiopvpc/releases/tag/v4.2.1), and set 'integration_type' to 'service' in `manifest.json`
- 🎨 pre-commit autoupdate

## [v1.0.0](https://github.com/azogue/ha-pvpc-custom/tree/v1.0.0) ✨ API Token support + extra price sensors (2023-04-02)

Mirror of [official HA-Core integration 'pvpc_hourly_pricing'](https://www.home-assistant.io/integrations/pvpc_hourly_pricing), with proposed changes to

- support authenticated access with **ESIOS API Token** ([MR1](https://github.com/home-assistant/core/pull/85767)),
- and enable **more electricity price sensors**, like the 'injection price' for solar installations ☀️ ([MR2](https://github.com/home-assistant/core/pull/85769))

Pushed here to enable _beta testers_ to install it through **HACS** until review process is finished,
and final changes are released in HA 🤞
