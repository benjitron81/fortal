# Fortal

A desktop application for retrieving and viewing configuration of FortiGate devices through a FortiManager

## Current Status

- Status: Production/Stable
- Latest Release: 1.0.0
- Release Date: 19-07-2026

## Change Log 1.0.0

- 19-07-2026: Added option in settings to enable FortiManager certificate verification (disabled by default)
- 19-07-2026: Fixed bug where an error notification would sometimes appear after a successful policy lookup
- 19-07-2026: Updated About page

## Change Log 0.8.6

- 10-07-2026: Minor GUI adjustments
- 09-07-2026: Set default retrieve type to 'Minimal'
- 09-07-2026: Added firewall policy lookup function to Policy tab
- 08-07-2026: Fixed bug where Keepalive Response graph could refresh too frequently causing Fortal to become unresponsive

## Change Log 0.8.5

- 27-06-2026: Added graph to the Dashboard tab to display min/max/avg response times for the most recent 10 keepalive probes
- 27-06-2026: Fixed bug where the policy package is not displayed for retrieved devices if the package is located in a subfolder
- 27-06-2026: Improved text formatting of rows on the Policy tab where cells contain multiple items (such as security profiles and address/ISDB objects)
- 27-06-2026: Fixed issue where keepalive probes fail when FortiManager is accessed using an FQDN due to a failed DNS lookup, Fortal now does a single DNS lookup at login then uses the resolved IP for all subsequent queries

## Change Log 0.8.4

- 21-06-2026: Added Policy tab to display firewall policies configured on the FortiGate
- 21-06-2026: Added option to retrieve page to select between full retrieve (all tabs) and minimal retrieve (System and Interfaces tabs only)
- 21-06-2026: Added additional function to check JSON validity of all API responses, and to reprocess the response when the bcfortiapi library returns a byte string (occurs as a failsafe when the FortiGate returns certain invalid characters in the API response)
- 21-06-2026: Fixed bug in System tab where management interface dropdown would lose the selected interface when defocused
- 20-06-2026: Added settings page (accessed from side menu), replaced plain-text settings file (fortal_settings.conf) with JSON-formatted file (fortal_settings.json)
- 20-06-2026: Fixed bug during device retrieve causing multiple instances of the device selection dropdown to appear if the ADOM selection changed
- 17-06-2026: Adjusted progression of retrieve progress bar and added progress status message below bar
- 17-06-2026: Added description column to Interfaces tab
- 17-06-2026: Fixed bug in System tab causing devices with multiple assigned policy packages to only display the last one in the list
- 17-06-2026: Fixed "Invalid Number" error showing for some traffic volume stats in firewall users tab

## Change Log 0.8.3

- 14-06-2026: Fixed 'traffic volume' key error bug when retrieving firewall users
- 14-06-2026: Fixed 'scope member' key error bug when retrieving assigned policy package name

## Change Log 0.8.2

- 13-06-2026: Added progress bar to retrieve page
- 13-06-2026: Invert colour of images in login and retrieve pages when dark mode is enabled
- 10-06-2026: Added configuration sync status, device database status, and assigned policy package to System tab
- 10-06-2026: Added option to specify static route index for FortiGate iPerf tests in fortal_settings.conf (default is 100000)
- 10-06-2026: Added interface name alongside IP address in management interfaces dropdown list for FortiGate HTTPS, SSH and ICMP
- 10-06-2026: Fixed 'usergroup' key error bug when retrieving firewall users

## Change Log 0.7.1

- 06-06-2026: Added tabs for virtual IPs and active firewall users

## Change Log 0.7.0

- 06-06-2026: 0.7.0 Initial public release
