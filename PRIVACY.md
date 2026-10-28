# Hikari (光) privacy statement

*Last updated 29 October 2026. Hikari is CuteClaudia's photo library and raw developer, part of the Kōbō suite.*

**In short:** Hikari has no account, no telemetry, no analytics, no advertising and no crash
reporting. Your files stay on your computer, or in storage you choose. CuteClaudia doesn't receive any
of your data.

## Your files

Hikari opens and saves files where you choose. It does not upload, copy or send them anywhere.
Settings and recent-file lists are kept in Hikari's settings folder on your computer.

## Optional downloads, only when you ask

Some features need a file that isn't built in. Hikari downloads it only when you start that feature, checks it against a fixed SHA-256 fingerprint, and keeps it on your computer:

- **Face recognition**: the face-detection and face-recognition model files, from GitHub (OpenCV's model zoo) and Hugging Face. Faces are found and compared **on your computer**; no photo or face is sent anywhere.
- **Fill Location from GPS**: a list of place names from GeoNames (download.geonames.org). Locations are looked up on your computer; your photos' positions are not sent.

These services see an ordinary download request (your IP address and the file asked for), under their own privacy terms.

## Show on Map

**Show on Map** opens OpenStreetMap in your browser at the photo's position. This happens only when you click it, and you see the address first: OpenStreetMap then receives that position, under its own privacy policy.

## Updates

- **Copies from GitHub** (the installer or portable download): When it starts, Hikari asks GitHub for the newest **published** release of `cuteclaudia/hikari-releases`, and offers it to you. Nothing about you, your files or your computer is sent; GitHub sees an ordinary web request (your IP address), under GitHub's privacy statement.
- **Copies from the Microsoft Store**: the Store installs and updates Hikari; Hikari doesn't
  check GitHub at all. Microsoft's privacy statement covers the Store.

## The web version

Hikari also runs in your browser on claudiagilbert.com. There it opens and saves files only through the storage you connect in the website's Settings › Files & storage (for example your own kDrive or other WebDAV storage). The browser's security policy lets the web version talk only to its own address and to the website, nowhere else. Your website account is covered by the website's own privacy policy.

## Links

Links in Help and About (claudiagilbert.com, the releases page, feedback) open in your browser
**only when you click them**.

## Automation (optional)

Hikari can be controlled by scripts and AI agents through a control channel and an MCP server.
They are **off** unless you start them yourself, listen only on your own computer, and need a
secret key that only you have.

## Children

Hikari collects no personal information from anyone, including children.

## Changes and contact

Changes to this statement are published here, with the date at the top. Questions or concerns:
[open an issue](https://github.com/cuteclaudia/hikari-releases/issues/new) (please don't include
personal information or files), or contact CuteClaudia through claudiagilbert.com.
