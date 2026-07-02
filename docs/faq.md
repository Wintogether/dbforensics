# FAQ

## What is DBForensics?

DBForensics is a Windows desktop tool for analyzing database traffic captured in PCAP and PCAPNG files. It reconstructs SQL sessions and presents database activity as events for investigation.

## What problem does it solve?

Packet analyzers show low-level network packets. DBForensics focuses on reconstructing database activity, so DBAs and security teams can review SQL statements, sessions, timestamps, status, duration, and protocol details from captured traffic.

## Which databases are supported?

MySQL is the current focus. PostgreSQL, Oracle, and SQL Server are planned for later versions.

## Does it require an agent?

No. DBForensics analyzes offline PCAP files and does not require installing an agent on the database server or application host.

## Does it support live capture?

Not yet. The current preview focuses on offline PCAP / PCAPNG analysis. Real-time capture is planned for a later version.

## Is it a replacement for Wireshark?

No. Wireshark is a general-purpose packet analyzer. DBForensics is focused on reconstructing database sessions and SQL activity from traffic captures.

## Is the project open source?

This repository is currently used for product information, documentation, releases, and feedback. The software itself is proprietary for now unless otherwise stated.

## Can I use my own PCAP files?

Yes. You can use your own PCAP or PCAPNG files, as long as they contain supported database traffic. For the current preview, MySQL traffic is the main supported use case.

## Does it support encrypted database traffic?

Encrypted database traffic is not decoded unless it is decrypted before or during capture. For example, TLS-encrypted database sessions cannot be reconstructed from encrypted payloads alone.

## Does DBForensics upload PCAP files?

No. The desktop application analyzes PCAP files locally and offline. Do not upload sensitive PCAP files to public Issues or Discussions.

## What is included in the repository?

This repository is used for product presentation, documentation, sample PCAP files, release distribution, Issues, Discussions, and feedback collection. It is not intended to be a full source-code repository at this stage.

## How can I give feedback?

Open an Issue or start a Discussion. Useful feedback includes your database type, capture workflow, Windows version, whether traffic is encrypted, expected reconstruction behavior, screenshots, and anonymized sample PCAP files when possible.
