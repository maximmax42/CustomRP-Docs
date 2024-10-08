---
description: 자주 묻는 질문 / 문제 해결
---

# ❓ 자주 묻는 질문 / 문제 해결

{% hint style="warning" %}
이 페이지는 오래되었을 수 있습니다. 최신 정보는 [이 페이지의 영문 버전](https://app.gitbook.com/s/5gJfBQC2iWNK0J953fo2/faq)을 참조하세요.
{% endhint %}

## 자주 묻는 질문

### 2개 이상의 버튼을 추가할 수 있나요?

안 됩니다, Discord의 최대치입니다.

### 다른 활동 (듣는 중, 보는 중, 방송 중)을 사용할 수 있나요?

안 됩니다, Discord의 한계입니다.

### 왜 제가 미래의 타임스탬프를 설정하면, DIscord는 몇 시간이 남았는지만 보여주나요?

이번에도 역시, Discord의 한계입니다.

### Linux/Mac을 지원할 예정인가요?

이 앱은 Windows 전용 라이브러리를 사용하여 빌드되므로 Linux 및 Mac을 지원하는 것은 전체 앱을 다른 라이브러리/코딩 언어로 다시 작성하는 것을 의미하고, 이에 대한 계획은 아직 없습니다.

### "Pipe"라는 창이 열렸는데, 이건 뭔가요?

Ctrl+Shift와 Connect 버튼(또는 이전 버전의 트레이 아이콘 메뉴에서 Ctrl와 Connect 버튼 또는 Reconnect 버튼)을 눌렀기 때문에 열렸습니다. -1로 두고 닫으면 됩니다. 동시에 두 개 이상의 Discord 클라이언트가 실행 중인 상황에 사용됩니다. Pipe 번호를 변경하면 어떤 클라이언트에 있을지 효과적으로 선택할 수 있습니다.

## 문제 해결

무엇이든 시도하기 전에, 당신의 CustomRP이 최신 버전에 인지 확인하세요!

### 프로필에 있는 활동 상태 버튼을 눌러도 작동하지 않아요.

CustomRP를 사용하는 PC 클라이언트에서는 버튼이 작동하지 않습니다. 이것은 Discord의 문제입니다. 모바일 또는 웹 클라이언트에서 버튼을 테스트하거나 다른 사람에게 대신 부탁하세요.

### CustomRP를 설치했지만 시작되지 않아요.

아마 당신의 백신(안티바이러스) 프로그램이 실행을 막고 있는 것 같네요! `%appdata%\CustomRP` 폴더를 제외해주세요.

### CustomRP를 설치하고, 정보 수집을 허용했는데 앱이 더 이상 작동하지 않습니다.

작업 관리자에서 앱을 끝내고, `%localappdata%\maximmax42` 폴더를 삭제하고 다시 시작하고 정보 수집을 허용하지 마세요.

### 앱이 연결되었지만 프로필에 활동 상태가 표시되지 않습니다.

Discord 설정에서 활동 상태가 켜져 있는지 확인하세요:

<figure><img src="https://user-images.githubusercontent.com/55352400/195621738-25a1cf30-56ec-43f8-a016-c91994139b02.png" alt=""><figcaption></figcaption></figure>

### 앱은 작동하지만, 지금은 무한정 연결만 되고 있어요.

활동 상태를 자주 연결/변경해서 디스코드에서 타임아웃을 받았을 수 있습니다. 연결을 끊고, 5-10분 동안 기다렸다가 다시 연결하세요. Discord를 다시 시작하는 것이 도움이 될 수도 있어요!

### 앱에 "ID가 잘못되었을 수 있음"/ "Discord가 실행 중인가요?"라고 표시되고 있어요. 또는 저는 모든 것을 제대로 했고 Discord가 실행 중이라고 확신하는데도 불구하고 무한정으로 연결되고 있어요.

이 방법들을 시도해보세요:

* **Discord 클라이언트를 사용하고 있는지 확인하세요 (브라우저 버전은 불가능함).**
* BetterDiscord/Vencord 등이 설치되어 있다면, CustomRP가 한번이라도 Discord에 연결된 후에 다시 설치하세요.
* 여러개의 Discord 클라이언트를 사용하고 있다면, 활동 상태가 표시되기를 원하는 클라이언트를 제외하고 모두 종료해주세요.
* CustomRP를 관리자 권한으로 실행하세요.
* `%appdata%\CustomRP` 경로 또는 만약에 무설치 버전을 사용하고 있다면 CustomRP를 압축 해제한 폴더를 방화벽이나 백신, 또는 안티바이러스에서 예외로 추가한 뒤, PC를 재시작하세요.
* Discord를 재설치하세요.

이 방법들이 도움이 되지 않았다면, 더는 제안할 방법이 없습니다, 죄송합니다.

### 앱이 원래 작동했었는데, 이제 앱이 중지되고 실행도 안돼요.

아마 당신이 멋진 텍스트 (또는 라틴어가 아닌 문자를 사용하는 언어의 텍스트)의 긴 문자열을 필드에 넣고 앱이 중지되었을 것입니다. 이 문제를 해결하려면 Win + R을 누르고 `%localappdata%\maximmax42`를 입력하고 이름에 CustomRP이 포함된 폴더를 삭제하거나 이름을 변경한 다음 앱을 다시 시작하세요. 이렇게 하면 앱이 완전히 재설정됩니다.

### 업데이트/연결 등을 시도할 때 앱이 계속 중지돼요.

만약 앱을 실행할 수 있고 오류 보고를 얻을 수 있고, 오류 보고에 `System.IO.FileNotFoundException: Could not load file or assembly...`라고 적혀있으면, 앱을 다시 설치하시기 바랍니다.

만약 당신의 질문/문제에 대한 답을 찾지 못했다면, [CustomRP Discord 서버](https://www.customrp.xyz/discordserver)의 `#support` 채널에 메시지를 보내거나, 저에게 디스코드 메시지를 보내거나 (maximmax42#5572), [여기](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose)에 문제를 알려주세요.
