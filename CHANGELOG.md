# Changelog

## [v1.2.0](https://github.com/azogue/ha-pvpc-custom/tree/v1.2.0) ✨ Add new sensors for market adjustment and indexed tariff (2024-03-10)

- ✨ Add new price sensors: **Market adjustment** (from ESIOS API indicator 2108), and **Indexed tariff** (as _composed_ price sensor calculated as `PVPC - ADJUSTMENT`), from first-time contributor @MiguelAngelLV in #18 (and azogue/aiopvpc#69) 🍻

## [v1.1.1](https://github.com/azogue/ha-pvpc-custom/tree/v1.1.1) 📦️ (MAINTENANCE) Fix import of `DeviceInfo` after HA v2023.9.0 (2023-08-19)

- 🐛 Fix future `ImportError` for `DeviceInfo` migrating to 'device_registry', scheduled for next HA-Core version 2023.9
- 📦️ Upgrade required Python to 3.11 and enable usage with 3.12, syncing with HA-Core reqs
- 🎨 pre-commit autoupdate

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
