---
description: Vui lòng đọc cái hướng dẫn này
---

# 🛠 Thiết Lập

Nếu bạn gặp bất kì lỗi nào, hãy xem [Câu hỏi thường gặp](faq.md).

Trước khi thiết lập, hãy đảm bảo bạn đã có một ứng dụng Discord độc lập (**không ở trình duyệt**) và đã bật trạng thái hoạt động trong cài đặt Discord:

![image](https://user-images.githubusercontent.com/65167922/282306100-83582007-85b1-40fb-9f14-881c6d06d975.png)

## Quá trình thiết lập

* Vào trang [https://discord.com/developers/applications/](https://discord.com/developers/applications/).
* Nhấn **New Application** ở trên góc phải màn hình.

![image](https://user-images.githubusercontent.com/2225711/161050202-c796103d-6712-401e-be96-3f3712512375.png)

* Nhập một cái tên cho ứng dụng, nó sẽ được hiển thị sau "Đang chơi" ở trạng thái; nhấn **Create**.
* Sao chép **Application ID** và dán nó vào mục **ID** ở CustomRP, sau đó nhấn **Kết nối**. Nếu làm đúng, trạng thái của bạn trên Discord bây giờ sẽ hiện "Đang chơi **\[tên của ứng dụng]**".
  * Lưu ý: Nếu bạn đã đặt trạng thái tùy chỉnh (cái có biểu tượng cảm xúc), nó sẽ được ưu tiên hơn cái của CustomRP. Nó sẽ được nhìn thấy trong cửa sổ bật lên của hồ sơ.

![image](https://user-images.githubusercontent.com/2225711/161050341-8169af53-5d3f-44d6-b745-cc711e8d1476.png)

* On your application's page, navigate to Rich Presence -> Art Assets and upload at least one image under Rich Presence Assets if you want to use them. In CustomRP, there is a handy **Upload Assets** button in File menu (you can also use Ctrl+U) that will take you there if your ID field is set up properly.
  * Alternatively, you can just insert a direct link to the image into the **Key** field.
  * Note: While you can name your asset with any name up to 999 symbols, the API will only accept names with 256 symbols max.
* Navigate to Visualizer page to set up fields **State, Details, Large Image Key, Large Image Text, Small Image Key, Small Image Text, Party Size, Party Max**. All of those are optional.
* After you've found the setup that pleases you, copy the values into CustomRP's corresponding fields.
  * Tip: You can hover over almost any control in the app (including labels line **Details**) and it'll give you a tooltip!
* If you want to set up buttons as well, fill in both Text and URL fields.
  * Note: When you will click on the buttons in your own presence, they will not work, but don't worry, they will work for everyone else. It's a problem on Discord's side.
* Hit **Update Presence** (or **Connect** if you aren't already connected).
* Congratulations, you're wonderful!

### I use more than one Discord client, what do I do?

If you have more than one Discord client and you wish your presence to show up on a different account from the one app chose automatically, please press **Disconnect**, then hold Ctrl+Shift keys on your keyboard and press **Connect**. A window with a number input will pop up, put a number 1, close the window, and press **Connect** again, without Ctrl+Shift. In case it's a wrong account again, try number 0, then 2 and so on up until 9.

Please note that if you have multiple Discord clients run on startup, pipe number assigned to each client might not be persistent from boot to boot and can change depending on which client started first. To prevent that, you can either start additional clients manually, or use Windows Task Scheduler to delay the startup of the clients.

If you have 2 accounts that you use at the same time and want for each of them to have a different presence, then follow these steps:

* Set up your main account first with the instructions above.
* Grab the latest **portable (.zip)** version of CustomRP (either from [website](https://www.customrp.xyz) or [GitHub releases page](https://github.com/maximmax42/Discord-CustomRP/releases/latest)) and unpack it anywhere.
  * This only works with versions 1.16 and older.
* Open `Start Second Instance.bat` or create a shortcut to CustomRP.exe with an argument `--second-instance` (or `-2`).
* Set up the program the same way you did your main instance.
  * Tip: If you already have a preset you would want to use with your second instance, you can edit the bat file or the shortcut to include the path to the preset. Example: `CustomRP.exe -2 "C:\Some Folder\preset.crp"` (quotation marks around the path are necessary if the path has spaces in it).
* Before connecting, change the pipe as described earlier and connect.

If you use 3 or more accounts at the same time, then... why? But also if enough of you will nag me, I'll add support for using more instances.

## Notes

* If you don't want to set up small or large image, leave all related fields in the program blank.
* If large image is not set, small image settings will be ignored.
