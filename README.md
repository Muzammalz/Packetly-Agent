# Packetly Agent

The Packetly Agent reports machine telemetry to a Packetly server. The Add Machine screen generates enrollment commands for Windows, Ubuntu and Linux Docker hosts.

1. Open **Servers & Hypervisors → Server & VM Monitoring → Add Machine** in your Packetly portal.
2. Register the machine and select **Windows**, **Linux**, or **Docker** to get its downloads and setup commands.
3. Follow the instructions on the monitored machine, then verify that it shows **Reporting** in Packetly.

Keep each machine's enrollment token private. The monitored machine needs network access to the Packetly server to report telemetry.

Windows setup runs from an administrator PowerShell prompt. Native Linux setup requires Bash, Python 3 and a systemd host. Docker setup requires Bash, Python 3 and a working Docker Engine on a Linux host. Both Linux setup modes require administrative access.

| Release asset | Use |
| --- | --- |
| `Install-PacketlyWindowsAgent.ps1` and `Packetly-Agent.exe` | Install the Windows agent and configure it to start at boot. |
| `packetly-agent-linux.tar.gz` | Install the Linux agent as a systemd service or run it in Docker with automatic restart. |
| `SHA256SUMS.txt` | Verify the downloaded files against the release checksums. |

[Open Packetly Agent releases](https://github.com/Muzammalz/Packetly-Agent/releases)
