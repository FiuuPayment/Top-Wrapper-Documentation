# Fiuu ToP Integration Documentation

Welcome to the **Fiuu ToP Integration Guide** — a documentation site for merchants integrating the **Fiuu ToP (Tap on Phone)** SDK into Android apps.

## Overview

**Fiuu ToP** accepts contactless card payments on a certified Android device without external hardware (EDC, PIN Entry Device, or Secure Card Reader). This site covers Google Play Integrity credential setup, SDK initialization, the transaction flow, signature capture, PIN entry, and status codes.

## Getting Started

1. Visit the documentation site: https://fiuupayment.github.io/Top-Wrapper-Documentation/
2. Open **Documentation**.
3. Complete [Credential Setup](docs/credential-setup/generate-service-account.md) once per app, or skip to [Getting Started](docs/getting-started.md) if credentials are already issued.
4. Follow [Start a Transaction](docs/transaction/start-transaction.md) and verify the flow with the [Tap-on-Phone Testing App](https://github.com/FiuuPayment/Tap-on-Phone).

## Key Features

- **Android Tap on Phone** — NFC contactless payments with no external terminal
- **Play Integrity credentials** — service account, exported key, encryption, and certificate registration
- **SDK initialization** — AAR setup, permissions, and `FasstapSDKConfiguration`
- **Transaction lifecycle** — start, abort, void, signature, and native PIN pad
- **Status code reference** — payload `statusCode` and SDK `resultCode`

## Documentation Structure

- **Introduction**: What Fiuu ToP is, minimum requirements, and what is included
- **Credential Setup**: Google Play Integrity service account, key export, GPG encryption, opt-in flags, project number, and certificate generation
- **Getting Started**: Add the SDK, declare permissions, and initialize
- **Transaction**: Start a transaction, cancel (in-flight abort vs. completed-purchase void), capture a signature, and handle PIN entry
- **Flow Overview**: End-to-end transaction flow and result field reference
- **Appendixes**: Status code reference

## Requirements

- Certified Android device with NFC, network connectivity, and Google Mobile Services (minimum Android 10 / API 29)
- Google Play Integrity credentials and a Fiuu-issued `vKey`
- Application ID and release-keystore public key registered with Fiuu

## Development

```bash
npm install
npm run dev
```

## Support

If you encounter any issues or need assistance, please reach out to our integration team:

- Email: support@fiuu.com

## License

This documentation is proprietary and intended for authorized partners and merchants only.
