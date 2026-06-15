# Fortal

A desktop application for retrieving and viewing configuration of FortiGate devices through a FortiManager

## Current Status

- Status: Beta
- Latest Release: 0.8.3
- Release Date: 14-06-2026

## Change Log 0.8.3

- 14-06-2026: Fixed 'traffic volume' key error bug when retrieving firewall users
- 14-06-2026: Fixed 'scope member' key error bug when retrieving assigned policy package name

## Change Log 0.8.2

- 13-06-2026: Added progress bar to retrieve screen
- 13-06-2026: Invert colour of images in login and retrieve screens when dark mode is enabled
- 10-06-2026: Added configuration sync status, device database status, and assigned policy package to System tab
- 10-06-2026: Added option to specify static route index for FortiGate iPerf tests in fortal_settings.conf (default is 100000)
- 10-06-2026: Added interface name alongside IP address in management interfaces dropdown list for FortiGate HTTPS, SSH and ICMP
- 10-06-2026: Fixed 'usergroup' key error bug when retrieving firewall users

## Change Log 0.7.1

- 06-06-2026: Added tabs for virtual IPs and active firewall users

## Change Log 0.7.0

- 06-06-2026: 0.7.0 Initial public release
