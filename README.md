# S_VERSE — Malware Analysis Lab

A browser-based, guided malware analysis and incident response lab. Work an active (simulated) ransomware incident at a fictional bank, **S_Bank**, from first triage to full recovery, with nothing to install and no real malware involved.

> Case **SB-2481** — *Aurora Ransomware*

## What you do

You play a SOC analyst with two virtual machines:

- **SB-FIN-PC7 (Windows 11)**: the damaged evidence host, with CMD and a mini browser (S-Webmail + ThreatVault).
- **SB-ANX01 (Parrot OS)**: your analyst workstation with an offline malware toolbox.

## Lab syllabus

| # | Task | Skills |
|---|------|--------|
| 1 | Incident Intake & Evidence Triage | Phishing analysis, evidence handling, file identification |
| 2 | Hashing & Threat Intelligence | MD5 / SHA-256, ThreatVault lookups |
| 3 | Static Analysis | strings, PE headers, entropy, imports, packer detection, UPX unpacking |
| 4 | Detonation (Dynamic Analysis) | Sandbox, persistence, live C2 socket |
| 5 | Network Forensics & Containment | PCAP review, beacon analysis, IP + DNS blocking |
| 6 | Sweep Triage & Recovery | Trojan / ransomware / virus / spyware / keylogger classification, purge, restore |

## Features

- **Auto-verified steps**: every guided command is checked the moment you run it.
- **IOC banking**: discovery commands add indicators to a case registry (`iocs`).
- **Task report quizzes**: unlock 3 questions per task after finishing its steps.
- **Final grade**: 50% steps + 50% questions, with a printable certificate.
- **Progress is saved** in your browser (`localStorage`) so you can resume.
- **Single file, zero dependencies**: plain HTML, CSS and vanilla JavaScript.

## Run it

**Locally:** download the repo and open `sverse-malware analysis lab.html` in any modern browser.
```

## Toolbox commands (SB-ANX01)

Type `help` in the terminal. Main commands:

```
file · md5sum · sha256sum · strings | grep · peinfo · imports · packscan
upx -d · sandbox run|netstat|autoruns|stop|reset · pcapview --dns|--http|--stats
firewall block · dnsblock · classify · purge · restore · iocs
```

## Disclaimer

This is an **educational simulation**. All malware, hashes, domains, IP addresses, wallets and email addresses are **fictional**. No real malicious code is included or executed. The lab runs entirely in your browser.

## License

MIT — see [LICENSE](LICENSE).

## Author

Built by [@sithu-afk](https://github.com/sithu-afk) as part of the **S_VERSE** security training series.

