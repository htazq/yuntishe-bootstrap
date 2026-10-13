# Yuntishe public bootstrap configuration

This dedicated repository publishes the signed public endpoint configuration for the Yuntishe client. It contains no client source code, account credentials, subscriptions, server IP addresses, or private signing keys.

- `manifest.json` is the signed envelope, copied byte-for-byte from the release configuration.
- `public-key.json` documents the public verification key. Clients must trust their bundled key rather than accepting a replacement key from this repository.
- Clients verify the Ed25519 signature, expiry and revision before using endpoint updates. An available mirror is not a guarantee that every network can reach it.

The configuration currently lists the public Yuntishe website endpoints. Updating a domain requires publishing a newly signed manifest; merchant keys and payment-channel configuration stay on the panel server.
