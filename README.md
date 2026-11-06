# NOEDRhost

Forensic command reference for hosts without an EDR agent. Covers Windows (CMD and PowerShell), Linux and macOS, so you can collect and review evidence manually from logs, processes, persistence, network state and file hashes.

Live page: https://harshadodderi.github.io/NOEDRhost/

## Contents

- `index.html`: the single-file reference page. Filter by OS and shell, search, copy commands, and export selected commands to a `.txt` file.
- `README.md`: this file.

## Usage

1. Open the page and select the operating system (Windows, Linux or macOS).
2. Set the output folder to external media where possible, so you do not write to the host under review.
3. Filter by shell (CMD, PowerShell or Shell) or use "Hide heavy scans" for a faster pass.
4. Copy the commands you need, or tick "Include in export" and download the selected commands.
5. Run them from an elevated prompt (Windows) or as root (Linux and macOS).

## Read-only and risk tags

- **Read-only query:** the command reads state and does not create a folder.
- **Creates folder:** the command makes an output folder.
- **Heavy scan:** a full-disk search that can take a long time.
- **Admin or root:** the command needs elevated rights.

## Notes

- The page does not run commands. You copy them and run them yourself.
- Test commands in a lab before relying on them in an investigation.
- macOS quarantine and TCC checks need Full Disk Access for the terminal.
- Windows UDP endpoint listings do not show remote peers. Use firewall, EDR or packet telemetry for that.
- The page contains a SaltySpider IOC IP check. Replace it with your own IOC list as needed.

## License

NO license
