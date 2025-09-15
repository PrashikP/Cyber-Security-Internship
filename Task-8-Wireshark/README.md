# Task 8 – Capture Network Traffic with Wireshark

## Objective
Capture and analyze network traffic on macOS using Wireshark.

## Environment
- macOS (MacBook Air M1)
- Wireshark 4.x (Homebrew build)

## Steps
1. Installed Wireshark & ChmodBPF helper via Homebrew.
2. Started capture on Wi-Fi interface `en0`.
3. Visited http://neverssl.com to create DNS/HTTP traffic.
4. Applied `tls` filter to inspect HTTPS packets.
5. Saved capture to `wireshark_capture.pcap`.

## Observations
- Packet #9678: TLSv1.3 Application Data from my Mac (port 54699) to server (port 443).
- DNS/HTTP packets visible when visiting plain-HTTP sites; HTTPS content encrypted.

## Deliverables
- `wireshark_capture.pcap`
- `screenshots/wireshark_capture.png`
- `README.md`

