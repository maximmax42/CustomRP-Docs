---
description: Vui lòng không được hỏi tôi những câu hỏi này ở máy chủ.
---

# ❓ Câu Hỏi Thường Gặp

{% hint style="warning" %}
Trang này có thể đã lỗi thời. Vui lòng tham khảo [phiên bản tiếng Anh của trang này](https://app.gitbook.com/s/5gJfBQC2iWNK0J953fo2/faq) để biết thông tin cập nhật.
{% endhint %}

## Câu Hỏi

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

Ứng dụng này được viết bằng một thư viện chỉ dành cho Windows, vì vậy việc hỗ trợ Linux và Mac cũng có nghĩa là viết lại cả ứng dụng với một thư viện/ngôn ngữ lập trình khác, điều mà tôi chưa lên kế hoạch.

### Một cửa sổ tên là "Pipe" hiện lên vì một lý do nào đó, đây là gì?

Nó hiện lên vì bạn nhấn Ctrl+Shift và nhấn nút Kết nối (hoặc Ctrl và nút Kết nối hoặc Kết nối lại trong menu biểu tượng ở khay ở những phiên bản cũ). Để nó ở -1 và đóng nó. Nó được dùng trong tình huống khi bạn có nhiều ứng dụng Discord chạy cùng một lúc. Thay đổi số pipe giúp chọn ứng dụng nào bạn muốn presence xuất hiện.

## Xử Lý Sự Cố

Trước khi thử bất kì điều gì, đảm bảo bạn đang dùng phiên bản CustomRP mới nhất!

### Khi tôi nhấn vào nút presence ở hồ sơ của tôi, chúng không hoạt động.

Nút sẽ không hoạt động với bạn ở nơi mà bạn đang sử dụng CustomRP, đó là lỗi kì quặc của Discord. Bạn có thể thử nút của bạn từ ứng dụng điện thoại hoặc web, hoặc hỏi ai đó để thử.

### Tôi đã cài đặt CustomRP nhưng nó không chạy.

Đây rất có thể là phần mềm chống virus của bạn ngăn ứng dụng khởi động. Thêm cặp `%appdata%\CustomRP` vào ngoại lệ.

### Tôi đã cài CustomRP, cho phép phân tích và ứng dụng không hoạt động nữa.

Tất ứng dụng trong Trình quản lý tác vụ (Task Manager), xóa cặp `%localappdata%\maximmax42`, khởi động lại ứng dụng và không cho phép phân tích.

### Ứng dụng đã kết nối, nhưng tôi không thấy trạng thái trong hồ sơ của tôi.

Hãy chắc chặn bạn đã bật trạng thái hoạt động ở cài đặt Discord:

<figure><img src="https://user-images.githubusercontent.com/65167922/282306100-83582007-85b1-40fb-9f14-881c6d06d975.png" alt=""><figcaption></figcaption></figure>

### Ứng dụng trước đó đẵ hoạt động, nhưng bây giờ nó đang kết nối vô thời hạn.

Bạn có thể đã hết thời gian chờ từ Discord bởi vì kết nối/thay đổi presence nhiều lần. Ngắt kết nối, đợi 5-10 phút, sau đó thử kết nối lại. Khởi động lại Discord có thể hữu ích.

### Ứng dụng nói "ID sai?"/"Bạn đã khởi động Discord chưa?" hoặc kết nối vô thời hạn kể cả khi tôi chắc chắn tôi làm mọi thứ đúng và Discord đang chạy.

Dưới đây là một số điều bạn nên thử:

* **Đảm bảo bạn đang chạy ứng dụng Discord độc lập (không ở trình duyệt).**
* Nếu bạn có cài BetterDiscord/Vencord/v.v, gỡ cài đặt nó, để CustomRP kết nối tới Discord ít nhất một lần và sau đó cài đặt chúng lại.
* Nếu bạn sử dụng nhiều ứng dụng Discord, tạm thời thoát tất cả chúng trừ ứng dụng mà bạn muốn presence xuất hiện.
* Chạy CustomRP với quyền quản trị viên.
* Thêm `%appdata%\CustomRP` hoặc, trong trường hợp bạn sử dụng phiên bản di động, cặp mà bạn giải nén CustomRP, vào ngoại lệ của tường lửa và/hoặc phần mềm chống virus, sau đó khởi động lại PC của bạn.
* Cài đặt lại Discord.

Nếu như vậy không giúp được, tôi không thể đề nghị cách gì khác, xin lỗi.

### Ứng dụng trước đó hoạt động, nhưng sau đó nó gặp sự cố và bây giờ nó không chạy được nữa.

Có lẽ bạn đã chèn một chuỗi văn bản dài (hoặc văn bản trong ngôn ngữ sử dụng kí tự không phải tiếng Latin) vào một mục và sau đó làm hỏng ứng dụng. Để sửa điều này, nhấn Win+R, nhập `%localappdata%\maximmax42` và xóa hoặc đổi tên cặp với tên CustomRP, sau đó chạy lại ứng dụng. Lưu ý rằng điều này sẽ đặt lại ứng dụng hoàn toàn.

### Ứng dụng liên tục gặp sự cố khi cập nhật/cố gắng kết nối/v.v.

Nếu bạn có thể khởi động ứng dụng và nhận được báo cáo sự cố, và nó hiện `System.IO.FileNotFoundException: Could not load file or assembly...`, vui lòng cài đặt lại ứng dụng.

Nếu bạn không thể tìm thấy câu trả lời cho câu hỏi/vấn đề của mình, gửi một tin nhắn đến kênh `#support` ở [máy chủ Discord CustomRP](https://www.customrp.xyz/discordserver), nhắn tin đến maximmax42 ở Discord hoặc [mở một vấn đề](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose).
