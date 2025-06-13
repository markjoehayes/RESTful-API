# HTTP vs HTTPS Comparison using Wireshark

This capture demonstrates the differences between unencrypted HTTP and encrypted HTTPS traffic using:

- `http://neverssl.com` (HTTP)
- `https://getfedora.org` (HTTPS)

## What’s in the Capture

The file `http_vs_https.pcapng` contains:
- Plain HTTP GET/response traffic from neverssl.com
- TLS handshake and encrypted HTTPS payload from getfedora.org

## How to View
- Open the `.pcapng` file in Wireshark
- Use filters:
  - `http` to see the readable request/response from neverssl
  - `tls` to inspect the TLS handshake with Fedora (note: contents are encrypted)

## Observations

- HTTP packets clearly show URLs, headers, and content in plaintext.
- HTTPS packets show only handshake steps and encrypted application data.

This highlights the security benefits of HTTPS (TLS).

