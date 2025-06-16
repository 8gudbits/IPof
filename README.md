# IPof

IPof is a lightweight command-line tool that retrieves the IP addresses of a given domain or URL. It resolves both IPv4 and IPv6 (if available) addresses.

## Usage

```bash
IPof -u/--url <url> [-n/--nobanner] [-h/--help]
```

## Options

- `-u, --url <url>` Specify the URL to find IP addresses.
- `-n, --nobanner` Suppresses the banner output.
- `-h, --help` Displays the help menu.

## Download exe for Windows

This tool is part of the [8gudbitsKit](https://github.com/8gudbits/8gudbitsKit) project. To download the executable for Windows, visit the [8gudbitsKit](https://github.com/8gudbits/8gudbitsKit) repository.

## For the Tech People

- Uses **Winsock2** (`WSAStartup`) for network initialization.
- Extracts the **hostname** from full URLs by stripping `http://`, `https://`, and paths.
- Calls **getaddrinfo()** to resolve both **IPv4** and **IPv6** addresses.
- Converts raw socket addresses to human-readable IPs using **inet_ntop()**.
- Implements a **CLI argument parser** for handling user input.

