# Plan & Subscription System

## One-Time Plans

- Lifetime or fixed-duration access
- Stored directly in UserActivePlan
- No recurring billing

## Subscription Plans

- Recurring billing
- Managed via Subscription model
- Access depends on status and expiry

## Subscription Status Logic

Active access requires:

- status in (active, trialing)
- current_period_end > now

This logic is implemented in:
Subscription.is_currently_active
