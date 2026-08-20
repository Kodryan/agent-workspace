# Repositories

Repository URLs are stable identifiers. Local paths point to working copies the agent may inspect. Use the revision specified by the user; if none is specified and `HEAD` is not `main`, ask before switching branches.

## ios-app

- Aliases: `app`, `main-app`
- URL: `https://github.example/mobile/ios-app`
- Local path: `/path/to/ios-app`
- Role: parent iOS application.
- Relationships:
  - consumes `payments-package`;
  - integrates checkout contracts;
  - composition root: `App/Payments/PaymentsAssembly.swift`.

## payments-package

- Alias: `payments`
- URL: `https://github.example/mobile/payments-package`
- Local path: `/path/to/payments-package`
- Role: public API and reusable implementation of the payment flow.
- Relationships:
  - consumed by `ios-app`;
  - protocol implementations are injected by the parent app.

## checkout-contracts

- Alias: `contracts`
- URL: `https://github.example/platform/checkout-contracts`
- Local path: `/path/to/checkout-contracts`
- Role: API schemas and wire-format contracts.

## checkout-backend

- Alias: `checkout-api`
- URL: `https://github.example/backend/checkout-backend`
- Local path: `/path/to/checkout-backend`
- Role: server-side checkout and payment orchestration.
