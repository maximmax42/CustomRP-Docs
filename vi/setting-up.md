---
description: Vui lòng đọc cái hướng dẫn này.
---

# 🛠 Thiết Lập

Nếu bạn gặp bất kì lỗi nào, hãy xem [Câu Hỏi Thường Gặp](faq.md).

Trước khi thiết lập, hãy đảm bảo bạn đã có một ứng dụng Discord độc lập (**không ở trình duyệt**) và đã bật trạng thái hoạt động trong cài đặt Discord:

![image](https://user-images.githubusercontent.com/65167922/282306100-83582007-85b1-40fb-9f14-881c6d06d975.png)

## Quá Trình Thiết Lập

* Vào trang [https://discord.com/developers/applications/](https://discord.com/developers/applications/).
* Nhấn **New Application** ở trên góc phải màn hình.

![image](https://user-images.githubusercontent.com/2225711/161050202-c796103d-6712-401e-be96-3f3712512375.png)

* Nhập một cái tên cho ứng dụng, nó sẽ được hiển thị sau "Đang chơi" ở trạng thái; nhấn **Create**.
* Sao chép **Application ID** và dán nó vào mục **ID** ở CustomRP, sau đó nhấn **Kết nối**. Nếu làm đúng, trạng thái của bạn trên Discord bây giờ sẽ hiện "Đang chơi **\[tên của ứng dụng]**".
  * Lưu ý: Nếu bạn đã đặt trạng thái tùy chỉnh (cái có biểu tượng cảm xúc), nó sẽ được ưu tiên hơn cái của CustomRP. Nó sẽ được nhìn thấy trong cửa sổ bật lên của hồ sơ.

![image](https://user-images.githubusercontent.com/2225711/161050341-8169af53-5d3f-44d6-b745-cc711e8d1476.png)

* Ở trang của ứng dụng, chuyển đến trang Rich Presence -> Art Assets và tải nhất ít nhất một hình ảnh trong Rich Presence Assets nếu bạn muốn dùng chúng. Ở CustomRP, sẽ có nút **Tải lên thiết lập** ở menu Tập tin (bạn cũng có thể nhấn Ctrl+U) sẽ đưa bạn đến đó nếu mục ID của bạn được thiết lập đúng cách.
  * Ngoài ra, bạn có thể chèn đường dẫn tới hình ảnh vào mục **Key**.
  * Lưu ý: Trong khi bạn có thể đặt tên thiết lập của bạn lên tới 999 kí tự, API sẽ chỉ chấp nhận cái tên với 256 kí tự.
* Di chuyển đến trang Visualizer để thiết lập mục **State, Details, Large Image Key, Large Image Text, Small Image Key, Small Image Text, Party Size, Party Max**. Tất cả chúng đều không bắt buộc.
* Sau khi bạn đã thiết lập, sao chép giá trị vào các mục tương ứng trong CustomRP.
  * Mẹo: Bạn có thể di chuột qua hầu hết mọi điều khiển trong ứng dụng (bao gồm cả **Details**) và nó sẽ cho bạn hướng dẫn chú giải!
* Nếu bạn muốn thiết lập các nút, điền vào cả mục Text và URL.
  * Lưu ý: Khi bạn thử nhấn nút ở presence của mình, chúng sẽ không hoạt động, nhưng đừng lo, chúng sẽ hoạt động cho người khác. Đó là vấn đề của Discord.
* Nhấn **Cập nhật trạng thái** (hoặc **Kết nối** nếu bạn chưa kết nối).
* Chúc mừng bạn, bạn thật tuyệt vời!

### Nếu tôi sử dụng nhiều hơn một ứng dụng Discord, tôi nên làm gì?

Nếu bạn sử dụng nhiều hơn một ứng dụng Discord và bạn muốn presence xuất hiện ở các tài khoản khác nhau ngoài tài khoản mà ứng dụng chọn tự động, vui lòng nhấn **Ngắt kết nối**, sau đó giữ phím Ctrl+Shift ở trên bàn phím sau đó nhấn **Kết nối**. Một cửa sổ nhập số sẽ hiện lên, nhập số 1, đóng cửa sổ đó, và nhấn lại nút **Kết nối** mà không cần giữ phím Ctrl+Shift. Trong trường hợp sai tài khoản, thử số 0, sau đó số 2 và tiếp tục cho đến số 9.

Lưu ý rằng nếu như bạn có nhiều ứng dụng Discord chạy trong khi khởi động, số pipe được gán cho mỗi ứng dụng có thể không liên tục từ khởi động này đến khởi động khác và có thể thay đổi dựa trên trình tự ứng dụng khởi động. Để tránh điều đó, bạn có thể chạy ứng dụng theo cách thủ công, hoặc dùng Windows Task Scheduler để trì hoãn việc khởi động của ứng dụng.

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
