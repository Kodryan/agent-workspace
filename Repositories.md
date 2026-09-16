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


