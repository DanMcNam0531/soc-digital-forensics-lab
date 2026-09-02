# Investigation Workflow

## Linux Authentication Evidence

- `btmp` records failed login attempts.
- `wtmp` records successful logins and session history.
- `journalctl` provides searchable system and service events.
- Zeek authentication and connection logs support network-level correlation.

## Network Evidence

Zeek was used to identify repeated SSH activity and organize connection metadata. Wireshark provided packet-level inspection for validating protocols, endpoints, and timing.

## Windows Evidence

- Autopsy supported examination of an E01 forensic image.
- RegRipper extracted targeted Windows Registry artifacts.
- LECmd parsed Windows shortcut files.
- Prefetch artifacts supported program-execution analysis.
- Registry and file-system timestamps helped reconstruct user and system activity.

## Correlation Process

1. Normalize timestamps and establish the investigation period.
2. Identify accounts, hosts, and network addresses involved.
3. Review authentication failures and successful access.
4. Correlate network activity with Windows execution artifacts.
5. Build an evidence table and event timeline.
6. Separate confirmed facts from analyst inferences.
7. Document limitations and recommended follow-up actions.
