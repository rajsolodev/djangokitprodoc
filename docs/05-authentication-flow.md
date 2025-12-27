# Authentication Flow

The project uses Django's built-in authentication system.

Flow:

1. User registers or logs in
2. User selects a plan
3. Payment is completed
4. Access is granted via UserActivePlan

Authentication logic is intentionally kept simple
to allow easy extension or replacement.
