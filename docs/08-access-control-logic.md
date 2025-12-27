# Access Control Logic

Access is determined using UserActivePlan.

Rules:

- A user has at most one active plan
- Subscription overrides one-time plan
- Expired subscriptions automatically lose access

Why this approach:

- No repeated checks across views
- Easy to change rules globally
- Scales well as features grow

Access checks should always rely on UserActivePlan,
not directly on Subscription or Order.
