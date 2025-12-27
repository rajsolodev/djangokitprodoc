# Payment Integration

Supported providers:

- Dodo Payments
- Stripe (integration-ready)

## Payment Flow

1. Checkout session created
2. User redirected to provider
3. Payment succeeds or fails
4. Webhook is triggered
5. Order is marked paid
6. UserActivePlan is updated

## Webhooks

- Webhooks live inside payments app
- All verification is done server-side
- Never trust frontend payment status
