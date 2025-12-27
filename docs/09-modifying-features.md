# Modifying Features Safely

## Change Pricing

- Update Plan model via admin or migration

## Add New Plan Type

- Extend PAYMENT_TYPE_CHOICES
- Update access logic if required

## Modify Subscription Rules

- Update is_currently_active property
- Keep DB-level filtering consistent

## Add New Payment Provider

- Implement provider service
- Hook into existing order + webhook flow
