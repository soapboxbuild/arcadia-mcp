---
name: arcadia
description: Access utility data via Arcadia Arc — list connected utility accounts, retrieve bills and interval data, calculate carbon emissions from electricity consumption. Use when asked about utility bills, energy consumption, interval data, carbon emissions from electricity, or connecting to a utility provider.
---

# Arcadia Arc Utility Data

## Available Tools
- `list_utility_accounts` — List all connected utility accounts with status and meter info
- `get_account` — Details for a specific account including connection status
- `get_bills` — Retrieve utility bills (monthly statements) for an account
- `get_interval_data` — High-resolution interval readings (15-min, 30-min, hourly, daily) for a meter
- `get_meters` — List meters for an account (electricity, gas, water, solar)
- `calculate_carbon` — Calculate CO₂ emissions from kWh using EPA eGRID state-level factors

## Carbon Calculation
The `calculate_carbon` tool uses 2023 EPA eGRID emission factors (lbs CO₂/MWh) by US state.
Returns kgCO₂e and lbs CO₂ with methodology: "EPA eGRID 2023".

## Authentication
Requires `ARCADIA_API_KEY` (Bearer token). Get an Arc API key at developer.arcadia.com.
In Soapbox: add your Arcadia API key in Settings → Plugins → Arcadia Arc → Add key.
