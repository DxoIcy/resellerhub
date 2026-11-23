# ResellerHub

Tiered reseller & agent portal: HQ manages products and stock, resellers order at their tier price and pay, agents sell from their reseller's inventory and earn commission.

- **Front end:** a single static `index.html` (hosted on Vercel, no build step).
- **Back end:** Supabase project `ukvdfhuecqtbsgdyzvcq` (database with row-level security, server functions, `accounts` edge function).

The Supabase key in `index.html` is the *publishable* key, which is meant to be public. Data is protected by the database's security rules.

Payments are simulated until a payment gateway (e.g. Billplz, ToyyibPay) is connected.
