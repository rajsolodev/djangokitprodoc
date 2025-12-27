# Project Architecture

The project follows a modular Django architecture with strict separation
of concerns.

## Core Apps

- accounts/
  User authentication and registration
- seller/
  Plan creation, pricing, and seller-facing logic
- payments/
  Orders, subscriptions, payment processing, webhooks
- core/
  Public pages and shared utilities

## High-Level Flow

User

→ Views 

→ Business Logic

→ Database

→ Payment Provider

→ Webhooks

→ Access Control

Business rules are NOT scattered across views.
All access logic is centralized.
