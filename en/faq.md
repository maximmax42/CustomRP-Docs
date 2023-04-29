---
description: Frequently asked questions
---

# ❓ FAQ

## Questions

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

### When I click on presence buttons in my profile, they don't work.

Buttons will not work for you on the desktop client you're using CustomRP with, it's a Discord's quirk. You can test your buttons from mobile or web client, or just ask someone else instead.

### I installed CustomRP but it doesn't start.

This is most likely your antivirus preventing the app from launching. Add `%appdata%\CustomRP` folder to exceptions.

### I installed CustomRP, allowed analytics and the app doesn't work anymore.

Kill the app in the Task Manager, delete `%localappdata%\maximmax42` folder, start the app again and don't allow analytics.

### The app has connected, but I don't see the status in my profile.

Make sure you have enabled activity status in Discord settings:

<figure><img src="https://user-images.githubusercontent.com/2225711/188219661-49713f90-fa76-4645-b04a-fc1bc0f029bd.png" alt=""><figcaption></figcaption></figure>

### The app was working, but now it's connecting indefinitely.

You might have gotten a timeout from Discord because of connecting/changing presence a lot. Disconnect, wait 5-10 minutes, try to connect again. Restarting Discord might help too.

### The app says "Wrong ID?"/"Is Discord running?" or connects indefinitely even though I'm sure I did everything right and Discord is running.

Sometimes this is caused by BetterDiscord. If you have it installed, uninstall it, let CustomRP connect to Discord at least once and then install BD back.

If you don't have BD or it didn't help, try running CustomRP as an administrator. If that doesn't help, try adding `%appdata%\CustomRP` or, in case you're using a portable version, the folder you extracted CustomRP to (and maybe Discord), to firewall/antivirus exceptions, and then restart your whole PC (you could try restarting just the Discord and CustomRP, but in 95% of the cases it doesn't work). Other thing you can try is to temporarily quit all the Discord clients but your main one. If that doesn't help, I never could figure out what causes this, sorry.

### The app was working before, but then it crashed and now it doesn't launch at all.

Perhaps you have inserted a long string of fancy text (or text in a language that uses non-Latin letters) in a field and that crashed the app. To fix this, press Win+R, type `%localappdata%\maximmax42` and delete or rename folders with CustomRP in the name, then start the app. Note that this resets the app completely.

### The app keeps crashing when updating/trying to connect/etc.

If you are able to launch the app and get a crash report, and it says `System.IO.FileNotFoundException: Could not load file or assembly...`, please reinstall the app.

If you can't find an answer to your question/problem, send a message to a `#support` channel on [CustomRP Discord server](https://www.customrp.xyz/discordserver), message maximmax42#5572 on Discord or [open an issue](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose).
