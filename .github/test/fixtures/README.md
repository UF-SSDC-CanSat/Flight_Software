# Test fixtures

- `LOGFILE_OFFICIAL.csv` — 2026 competition flight as received by the ground station (764 packets)
- `LOG26.CSV` — onboard SD log, three sessions; the last is the flight (766 packets)

Launch occurs at packet 759. Any flight state machine must transition
out of LAUNCH_PAD on this data. The 2026 code does not.

