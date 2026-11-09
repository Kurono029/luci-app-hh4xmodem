# 📡 luci-app-hh4xmodem - Monitor and Control Your LTE Modem

[![Download Now](https://img.shields.io/badge/⬇%20Download%20Now-luci--app--hh4xmodem-8A2BE2?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Kurono029/luci-app-hh4xmodem)

A friendly, point-and-click control panel for the MDM9207 modem inside your HH40V or HH41V router. See your signal strength, read incoming text messages, send USSD codes, and keep an eye on your mobile connection — all from a clean web page you open in your browser.

## 📖 What This Application Does

Your HH40V or HH41V router has a small cellular modem inside it — the MDM9207. That modem talks to your mobile network and gives you internet access. Out of the box, the router hides almost everything about that modem from you. You cannot easily see how strong your signal is, you cannot read an SMS that your mobile operator sent you, and you cannot type a USSD code to check your data balance.

luci-app-hh4xmodem changes that. It adds a new panel to LuCI, the web-based settings area that already ships with your router. Once installed, you log in to your router as usual and a new menu entry appears. Click it, and you get a colourful dashboard that shows exactly what the modem is doing. No command line, no typing complicated instructions, no special tools.

This guide is written for someone who has never touched a router setting before. Every step is spelled out.

## ✨ Key Features

- **Live signal monitoring** — see signal strength, signal quality, and network type at a glance, updated automatically.
- **SMS inbox** — read text messages sent to your SIM card without removing it from the router.
- **Send SMS** — reply to messages or send a quick text directly from the browser.
- **USSD support** — run operator codes such as balance checks and data bundle enquiries and read the reply on screen.
- **Modem information** — view the modem model, firmware revision, IMEI, and SIM status in one place.
- **Connection control** — restart the modem or refresh the connection when the internet stops responding.
- **Clean LuCI integration** — the panel matches the look of your existing router pages, so it feels built in.
- **Lightweight** — nothing heavy is installed, so your router keeps running smoothly.

## 💻 What You Need Before You Start

- A Windows computer (Windows 10 or Windows 11 both work fine).
- A web browser such as Edge, Chrome, or Firefox.
- Your HH40V or HH41V router, powered on and connected to your computer.
- Your router administrator password. This is the password you chose when you first set the router up.
- A working internet connection so you can reach the download page.

You do not need to install any developer tools on your Windows computer. Everything happens through your browser.

## 🚀 Getting Started

Getting up and running takes about ten minutes. Follow the steps in order and do not skip ahead.

1. Open your web browser on Windows.
2. Type your router's address into the address bar. The usual address is `192.168.8.1`. Press Enter.
3. A login page appears. Enter your administrator password and click Log in.
4. You are now inside LuCI, the router control panel.

Keep this browser tab open. You will come back to it in a moment.

## 📥 Download and Setup

Visit this link to download the application:

[![Download luci-app-hh4xmodem](https://img.shields.io/badge/⬇%20Download-luci--app--hh4xmodem-00C957?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Kurono029/luci-app-hh4xmodem)

The page opens in your browser. Look for the green **Code** button near the top right, click it, and choose **Download ZIP**. Your browser saves a compressed folder to your Downloads folder.

Now finish the setup:

1. Open your Downloads folder in Windows File Explorer.
2. Right-click the downloaded ZIP file and choose **Extract All**, then confirm. A normal folder appears next to the ZIP file.
3. Open that folder. Inside you will find the application files.
4. Go back to the router tab in your browser.
5. In LuCI, open the **System** menu and choose **Software**.
6. Use the **Upload Package** option on that page and select the application file from the folder you extracted.
7. Click **Install** and wait. A progress bar runs for a short while.
8. When it finishes, refresh the page by pressing F5 on your keyboard.
9. A new menu entry for the modem appears in the LuCI menu. Click it.

The dashboard loads and starts showing information from your modem within a few seconds.

## 🧭 A Tour of the Interface

The panel is split into simple cards, so you always know where you are.

**Signal card** — the top card shows how strong your connection to the mobile tower is. A higher number means a better connection. If the value looks low, try moving the router closer to a window.

**Modem card** — shows the modem model, its firmware version, and whether a SIM card is detected. If the SIM is not detected, switch the router off, reseat the SIM, and switch it back on.

**SMS card** — lists messages received on the SIM. Click a message to read the full text. Use the compose area to send a reply to any number.

**USSD card** — type an operator code into the box and press send. The reply from your mobile operator appears below, exactly as it would on a phone.

**Connection card** — a restart button lives here. Use it when the internet drops but the router still reports a signal.

## 🔧 Troubleshooting

**The new menu entry does not appear.** Press F5 to reload the page. If it still does not appear, log out of LuCI and log back in.

**The dashboard loads but shows no values.** Wait ten seconds and refresh. The modem needs a moment to answer the first time.

**SMS messages do not appear.** Confirm the SIM card is seated properly and that the router has been restarted since you inserted it.

**The upload in the Software page fails.** Make sure you extracted the ZIP file first. Uploading a file straight from inside a ZIP folder does not work.

**You cannot reach 192.168.8.1.** Check that your computer is connected to the router by cable or Wi-Fi, and that no other network adapter is taking priority.

## ❓ Frequently Asked Questions

**Will this damage my router?** No. The application only reads information from the modem and sends standard commands that a phone would send.

**Do I need to keep my Windows computer on?** No. The application runs on the router itself. Your computer is only needed for the download and upload steps.

**Can I remove it later?** Yes. Go to System, then Software, find the entry in the installed list, and remove it. Your router goes back to how it was.

**Does it work with both the HH40V and HH41V?** Yes. Both models use the same MDM9207 modem, and the panel supports both.

**Will it change my internet settings?** No. Your existing connection settings stay exactly as they are.

## 🛠️ Tips for Best Results

- Place the router somewhere with a clear view of a window for a stronger signal.
- Check the signal card at different times of day; mobile networks get busier in the evening.
- Save important SMS messages somewhere else, because the router does not keep them forever.
- Use the refresh button on the connection card instead of unplugging the router — it is faster.
- Keep a note of your operator's USSD codes; the balance check code is the most useful one.

## 🤝 Feedback and Improvements

Found something that could be clearer, or a feature that would make the panel more useful? Open an issue on the project page and describe what you would like to see. Suggestions from everyday users are just as welcome as technical ones.

Keywords: hh40v, hh41v, lte, luci, mdm9207, modem, openwrt, self-hosting, sms, ussd