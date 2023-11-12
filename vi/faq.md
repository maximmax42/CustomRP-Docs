---
description: Vui lòng không được hỏi tôi những câu hỏi này ở máy chủ.
---

# ❓ Câu hỏi thường gập

## Câu hỏi

### Đây có phải là một virus? Phần mềm diệt virus/VirusTotal/v.v nói nó có virus.

Không. CustomRP không chứa bất kì virus nào, mã nguồn của ứng dụng có sẵn để mọi người kiểm tra.

Có thể bạn sẽ hỏi, tại sao một số phần mềm diệt virus và VirusTotal nói ứng dụng có virus? Chủ yếu là do ứng dụng của tôi a) không phổ biến đến mức được Windows và một số phần mềm chống virus coi là đáng tin cậy, và b) không được kí với một chứng chỉ số (bởi vì tôi là người Nga nên hiện tại tôi thậm chí không thể mua được một cái, và nếu như tôi có thể, nó hơi đắt).

### Tôi có thể thêm nhiêu hơn 2 nút được không?

Không, đó là giới hạn của Discord.

### Tôi có thể sử dụng loại hoạt động khác không (vd. đang nghe, đang xem, đang stream)?

Không, đó cũng là giới hạn của Discord.

### Tại sao nếu tôi đặt dấu thời gian trong vài ngày tới thì Discord chỉ hiển thị còn lại bao nhiêu giờ?

Bạn đoán xem, đó cũng là giới hạn của Discord.

### Liệu sẽ có phiên bản Linux/Mac?

Ứng dụng này được tạo bằng một thư viện chỉ dành cho Windows, vì vậy việc hỗ trợ Linux và Mac cũng có nghĩa là viết lại cả ứng dụng với một thư viện/ngôn ngữ lập trình, điều mà tôi chưa lên kế hoạch.

### Một cửa sổ tên là "Pipe" hiện lên vì một lý do nào đó, đây là gì?

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

Here are some things for you to try:
- **Make sure you're running a standalone Discord client (not in browser).**
- If you have BetterDiscord/Vencord/etc installed, uninstall it, let CustomRP connect to Discord at least once and then install it back.
- If you use multiple Discord clients, temporarily quit all of them except the one you want the presence to be on.
- Run CustomRP as administrator.
- Add `%appdata%\CustomRP` or, in case you're using a portable version, the folder you extracted CustomRP to, to firewall and/or antivirus exceptions, then restart your whole PC.
- Reinstall Discord.

If nothing helped, I can't suggest anything else, sorry.

### The app was working before, but then it crashed and now it doesn't launch at all.

Perhaps you have inserted a long string of fancy text (or text in a language that uses non-Latin letters) in a field and that crashed the app. To fix this, press Win+R, type `%localappdata%\maximmax42` and delete or rename folders with CustomRP in the name, then start the app. Note that this resets the app completely.

### The app keeps crashing when updating/trying to connect/etc.

If you are able to launch the app and get a crash report, and it says `System.IO.FileNotFoundException: Could not load file or assembly...`, please reinstall the app.

If you can't find an answer to your question/problem, send a message to a `#support` channel on [CustomRP Discord server](https://www.customrp.xyz/discordserver), message maximmax42#5572 on Discord or [open an issue](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose).
