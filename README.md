# Aim Local Host

A lightweight desktop utility for creating and joining Studio Team Test sessions online using UDP tunnels. Built with Python and Tkinter for a simple and fast setup experience.

## Requirements

* Windows 10 or newer
* Roblox Studio installed
* A UDP tunnel service (only needed for online sessions)
* No extra Python packages required — everything uses Python standard libraries.

---

# Installation

1. Open the latest release build.
2. Download the `.exe` version.
3. Launch the application.

On first startup, Aim Local Host automatically scans your system for Roblox Studio using PowerShell. This may take a few seconds.

If Studio cannot be detected, a warning message will appear. Make sure Roblox Studio is properly installed before continuing.

---

# Creating a Session

Use this if you want to host a Studio Team Test server for friends or collaborators.

1. Open Aim Local Host.
2. Press **Host Session**.
3. Fill in the required information:

### User ID

Your Roblox numeric user ID.
Example profile link:
`roblox.com/users/123456789/profile`

### Tunnel Endpoint

Your UDP tunnel address in this format:

`hostname:port`

Example:
`myserver.tunnel.gg:55555`

If you're only testing locally on the same network or PC, this can stay empty.

### Session Port

The port Roblox Studio will use for Team Test hosting.
Default:

`55555`

Only change this if another application is already using the port.

4. Click **Launch Server**.

Aim Local Host will:

* Start the relay server
* Open the console
* Launch Roblox Studio automatically in Team Test host mode

Wait a few seconds until the console displays:

`SESSION ONLINE`

At this point the server is fully active.

### Joining Your Own Server

You can instantly connect from the same computer by clicking:

`Connect Locally`

This launches a Studio client connected directly to your local session.

Share your tunnel address with anyone joining remotely.

---

# Tunnel Configuration

Basic UDP tunnel setup:

* **Port:** `55555`
* **Protocol:** `UDP`

---

# Joining a Session

Use this if someone else is hosting.

1. Open Aim Local Host.
2. Click **Connect to Session**.
3. Enter the host's tunnel endpoint:

`hostname:port`

Example:
`friendhost.tunnel.gg:55555`

4. Press **Connect**.

The application will:

* Open the networking console
* Establish the UDP relay connection
* Launch Roblox Studio automatically as a client

Once packets begin appearing in the console, the session is connected successfully.

To leave the server, press:

`Disconnect`

This safely closes the connection and returns you to the main menu.

---

# Features

* Automatic Roblox Studio detection
* One-click Team Test hosting
* Built-in local connection support
* UDP tunnel compatibility
* Simple lightweight interface
* Live connection logging
* No dependency installation required

---

# Credits

Developer: `AimHost`
Community Server: [Discord Server](https://discord.gg/a2FG9yF5tg)
