# Database Design

## Plan

Defines pricing and plan type.

Fields:

- title
- payment_type (one_time / subscription)
- price
- selling_price

## Subscription

Tracks recurring access and billing cycle.

Fields:

- user
- plan
- status
- current_period_start
- current_period_end

## Order

Stores payment history.

Fields:

- user
- plan
- subscription (optional)
- provider
- amount
- status

## UserActivePlan (CORE CONCEPT)

This table is the single source of truth for user access.

Why it exists:

- Avoid checking subscriptions everywhere
- One place to determine user access
- Supports both one-time and subscription plans
