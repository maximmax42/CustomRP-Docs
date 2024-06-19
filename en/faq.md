---
description: Please stop asking me the same questions in the server.
---

# ❓ Frequently Asked Questions

## Questions

### Is this a virus? My antivirus/VirusTotal/etc says there's a virus.

No. CustomRP doesn't contain any viruses, the source code is available for everyone to check.

You might be asking then, why do some antiviruses and VirusTotal say there's a virus? Mostly it's because my app a) isn't as popular to be considered trustworthy by Windows and some antiviruses, and b) isn't signed with a code signing certificate (because I'm Russian I currently can't even buy one, and if I could, they're pretty expensive).

### Can I add more than 2 buttons?

No, it's a limitation of Discord.

### Can I use a different type of activity (e.g. listening, watching, streaming)?

No, it's also a Discord limitation.

### Why if I set a timestamp couple days in the future, Discord only shows how many hours left?

You guessed it, it's also a Discord limitation.

### Will there be Linux/Mac version?

The app is built using a Windows-only library, therefore supporting Linux and Mac would mean rewriting whole app in a different library/coding language which I'm not planning just yet.

### A window called "Pipe" opened up for some reason, what is this?

It opened up because you pressed Ctrl+Shift and clicked Connect button (or Ctrl and Connect button or Reconnect in tray icon menu on older versions). Leave it at -1 and close it. It's used for situations when you have more than one Discord client running at the same time. Changing pipe number effectively chooses which client you want your presence to be in.

## Troubleshooting

Before trying anything, make sure you are on the latest version of CustomRP!

### I installed CustomRP but it doesn't start.

This is most likely your antivirus preventing the app from launching. Add `%appdata%\CustomRP` folder to exceptions.

### I installed CustomRP, allowed analytics and the app doesn't work anymore.

Kill the app in the Task Manager, delete `%localappdata%\maximmax42` folder, start the app again and don't allow analytics.

### The app has connected, but I don't see the status in my profile.

Make sure you have enabled activity status in Discord settings:

![image](https://github.com/maximmax42/CustomRP-Docs/assets/2225711/a1b8cb1e-7f88-4061-b297-2691523718a5)

### The app was working, but now it's connecting indefinitely.

You might have gotten a timeout from Discord because of connecting/changing presence a lot. Disconnect, wait 5-10 minutes, try to connect again. Restarting Discord might help too.

### The app says "Wrong ID?"/"Is Discord running?" or connects indefinitely even though I'm sure I did everything right and Discord is running.

Here are some things for you to try:
- **Make sure you're running a standalone Discord client (not in browser).**
- Restart your PC. Pro tip: restarting PC solves a lot of problems.
- If you have BetterDiscord/Vencord/etc installed, uninstall it, let CustomRP connect to Discord at least once and then install it back.
- If you use multiple Discord clients, temporarily quit all of them except the one you want the presence to be on.
- Run CustomRP as administrator.
- Add `%appdata%\CustomRP` or, in case you're using a portable version, the folder you extracted CustomRP to, to firewall and/or antivirus exceptions, then restart your whole PC.
  - If you don't know whether you have an antivirus or not, you most likely do - Windows Defender is on every Windows 10/11 computer.
- Reinstall Discord.

If nothing helped, I can't suggest anything else, sorry.

### The app is stuck on "Updating presence..."

Check image URLs in Key fields, they might be malformed (e.g. you inserted new link in the middle of an old one).

### The app was working before, but then it crashed and now it doesn't launch at all.

Perhaps you have inserted a long string of fancy text (or text in a language that uses non-Latin letters) in a field and that crashed the app. To fix this, press Win+R, type `%localappdata%\maximmax42` and delete or rename folders with CustomRP in the name, then start the app. Note that this resets the app completely.

### The app keeps crashing when updating/trying to connect/etc.

If you are able to launch the app and get a crash report, and it says `System.IO.FileNotFoundException: Could not load file or assembly...`, please reinstall the app.

If you can't find an answer to your question/problem, send a message to a `#support` channel on [CustomRP Discord server](https://www.customrp.xyz/discordserver), message maximmax42 on Discord or [open an issue](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose).
