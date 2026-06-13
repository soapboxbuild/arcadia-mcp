---
description: Retrieve utility bills for a connected account
argument-hint: [account ID or "list accounts first"]
---
Retrieve utility bills for this property's connected utility account via Arcadia Arc:
1. If needed, call list_utility_accounts to find the account ID
2. Call get_bills with the account ID (last 12 months by default)
3. Summarize: total consumption, total cost, monthly trend, any anomalies
$ARGUMENTS
