---
description: RTFM
---

# 🛠️ 시작하기

{% hint style="warning" %}
이 페이지는 오래되었을 수 있습니다. 최신 정보는 [이 페이지의 영문 버전](https://app.gitbook.com/s/5gJfBQC2iWNK0J953fo2/setting-up)을 참조하세요.
{% endhint %}

만약 어떤 문제를 겪고있다면, [자주 묻는 질문 / 문제 해결](faq.md) 페이지를 확인하세요.

시작하기 전에, Discord 설정에서 활동 상태가 켜져 있는지 확인하세요:

<figure><img src="https://user-images.githubusercontent.com/55352400/195621738-25a1cf30-56ec-43f8-a016-c91994139b02.png" alt=""><figcaption></figcaption></figure>

## 시작 과정

* https://discord.com/developers/applications/ 로 이동하세요.
* 오른쪽 위에 있는 **New Application** 을 클릭하세요.

![image](https://user-images.githubusercontent.com/2225711/161050202-c796103d-6712-401e-be96-3f3712512375.png)

* 앱을 위한 이름을 고르세요. 활동 상태에서 "하는 중" 앞에 표시될 거에요. 그리고 **Create**를 누르세요.
* **Application ID**을 복사하고 CustomRP의 **ID** 필드에 붙여 넣고, **연결**을 누르세요. 만약 제대로 했다면, 당신의 활동 상태에 "**\[name of the app] 하는 중**" 이라고 표시될 거에요.
  * 참고: (이모티콘이 있는) 사용자 정의 활동 상태가 있는 경우, CustomRP보다 우선됩니다. 이것은 프로필 팝업에서 볼 수 있습니다.

![image](https://user-images.githubusercontent.com/2225711/161050341-8169af53-5d3f-44d6-b745-cc711e8d1476.png)

* 당신의 앱 페이지에서 Rich Presence -> Art Assets 로 이동하고 Rich Presence Assets에 사용하기를 원하는 이미지를 업로드하세요. CustomRP에, 편리한 **프리셋 업로드** 버튼이 있으며 (Ctrl+U를 사용할 수도 있음), ID 필드가 제대로 설정되어 있으면 이 버튼을 사용할 수 있습니다.
  * 또는, **Key** 필드에 이미지의 URL을 넣기만 하면 됩니다.
  * 참고: 최대 999개의 기호로 에셋 이름을 지정할 수 있지만 API는 최대 256개까지의 기호가 있는 이름만 허용합니다.
* Visualizer 페이지로 이동해 **State, Details, Large Image Key, Large Image Text, Small Image Key, Small Image Text, Party Size, Party Max**를 설정하세요. 모두 선택사항입니다.
* 마음에 드는 설정을 찾은 후, 값을 CustomRP의 해당 필드에 복사하세요.
  * 팁: 앱의 (**Details** 라벨을 포함한) 거의 모든 컨트롤에 커서를 올리면 정보를 확인할 수 있어요!
* 버튼도 설정하려면 Text 필드와 URL 필드를 모두 입력하세요.
  * 참고: 자신의 프로필에서 버튼을 눌러도 작동하지 않겠지만, 걱정하지 마세요. 다른 모든사람들에게는 작동할 테니까요. 이것은 Discord의 문제에요.
* **활동 상태 업데이트**를 누르세요 (만약 이미 연결이 되어 있지 않다면 **연결** 버튼도 누르세요).
* 축하해요, 멋져보이네요!

### 1개가 넘는 Discord 클라이언트를 사용하는데, 어떻게 해야 하나요?

만약 1개가 넘는 Discord 클라이언트를 사용하고 있고 앱이 자동으로 선택한 계정 말고 다른 계정에 연결하고 싶으시면, 먼저 **연결 끊기**를 누르고, Ctrl+Shift 키를 누른 상태로 **연결**을 눌러주세요. 숫자 입력칸이 있는 창이 나타나면, 숫자 1을 적고, 창을 닫고, Ctrl+Shift를 누르지 않은 상태로 다시 **연결**을 눌러주세요. 만약 잘못된 계정이라면, 숫자 0, 그리고 2부터 9까지 시도해보세요.

Discord 클라이언트가 시작 프로그램인 경우, 각 클라이언트에 할당된 파이프 번호가 다음 부팅에서 지속되지 않을 수 있으며 어떤 클라이언트가 먼저 시작되었는지에 따라 달라질 수 있습니다. 이를 방지하려면, 추가 클라이언트를 수동으로 시작하거나, Windows 작업 스케줄러를 사용해 클라이언트의 시작을 지연시킬 수 있습니다.

만약 2개의 계정을 가지고 있고 각 계정에 다른 활동 상태를 갖기 원하는 경우, 다음 단계를 따라하세요:

* Set up your main account first with the instructions above. 위의 설명에 따라 주로 쓰는 게정을 설정하세요.
* CustomRP의 **포터블 (.zip)** 버전을 ([website](https://www.customrp.xyz) 또는 [GitHub releases page](https://github.com/maximmax42/Discord-CustomRP/releases/latest)에서 다운로드 하고) 그리고 아무데나 압축을 푸세요.
  * 이것은 1.16 또는 그 이상의 버전에서만 가능합니다.
* `Start Second Instance.bat`을 열거나 `--second-instance` (또는 `-2`) 전달인자를 가진 CUstomRP.exe 바로가기를 생성하세요.
* 주로 쓰는 계정과 같은 방법으로 프로그램을 설정하세요.
  * 팁: 만약 두 번째 인스턴스에서 사용하고 싶은 프리셋을 이미 가지고 있다면, bat 파일이나 바로가기가 프리셋의 위치를 포함하도록 수정할 수 있습니다. 예시: `CustomRP.exe -2 "C:\그냥 폴더\preset.crp"` (경로에 띄어쓰기가 있는 경우에 따옴표가 있어야 합니다).
* 연결하기 전에, 앞에서 설명한 대로 파이프를 변경하고 연결합니다.

만약 3개가 넘는 계정을 동시에 사용하고 있다면... 왜그러는거죠? 그래도 만약 충분히 많은 사람이 원한다면, 더 많은 인스턴스를 사용할 수 있도록 할 거에요.

## 참고

* 만약 작은 이미지나 큰 이미지를 설정하고 싶지 않다면, 프로그램의 관련 필드를 모두 비워두세요.
* 만약 큰 이미지가 설정되어있지 않다면, 작은 이미지 설정은 무시될 것입니다.
