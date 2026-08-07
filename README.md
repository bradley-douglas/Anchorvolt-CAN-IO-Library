# Anchorvolt CAN-IO Library

Public distribution channel for the **CAN-IO-PRO end-user product**.

This repository deliberately contains only:

- vehicle-selection metadata and function display names;
- encrypted, authenticated CAN-IO-PRO vehicle packages (`.avp`); and
- encrypted, authenticated CAN-IO-PRO firmware packages (`.avfw`).

CAN IDs, byte indexes, masks, active states and firmware binaries are not
published as plaintext. The Anchorvolt CAN-IO Configurator Android app downloads
these packages but does not contain the product decryption key. A CAN-IO-PRO
device authenticates and decrypts a package internally before accepting it.

The developer listener firmware, Windows learning software, source vehicle JSON
files and encryption tooling remain in the separate Vehicle-CAN-IO development
repository. Do not upload raw learning JSON, VINs, setup notes, source code,
private keys or unencrypted firmware here.

## Public paths

- `profiles/catalog.json` — vehicle dropdown catalog
- `profiles/packages/` — encrypted vehicle packages
- `firmware/can-io-pro/latest.json` — production firmware channel
- `firmware/can-io-pro/packages/` — encrypted firmware packages

Copying the public files alone does not reveal their protected contents. This
is practical product protection, not a claim of absolute resistance to invasive
physical extraction from a production device.
