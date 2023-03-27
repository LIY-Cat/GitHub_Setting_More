# GitHub_Setting_More
It is a repository that explains Github settings and commands.

git config opsions

--global: This option sets the configuration variable globally across all repositories on your machine. If you want to set a variable for a specific repository only, you can omit this option.

--local: This option sets the configuration variable for the current repository only. If you want to set a variable globally, you can omit this option.

--unset: This option unsets the value of a configuration variable. For example, if you want to remove the email address associated with your Git account, you can run "git config --unset user.email".

--get: This option displays the value of a configuration variable. For example, if you want to check the email address associated with your Git account, you can run "git config --get user.email".

--list: This option displays all configuration variables and their values in a list format.

--replace-all: This option replaces all occurrences of a configuration variable with the new value. If you want to add a new configuration variable, you can omit this option.

--add: This option adds a new value to a configuration variable that accepts multiple values. For example, if you want to add a new email address to your Git account, you can run "git config --add user.email newemail@example.com".

--global: 이 옵션은 시스템의 모든 리포지토리에서 구성 변수를 전체적으로 설정합니다. 특정 리포지토리에 대해서만 변수를 설정하려는 경우 이 옵션을 생략할 수 있습니다.
--local: 이 옵션은 현재 저장소에 대해서만 구성 변수를 설정합니다. 변수를 전체적으로 설정하려면 이 옵션을 생략할 수 있습니다.
--unset: 이 옵션은 구성 변수의 값을 설정 해제합니다. 예를 들어 Git 계정과 연결된 이메일 주소를 제거하려면 "git config --unset user.email"을 실행할 수 있습니다.
--get: 이 옵션은 구성 변수의 값을 표시합니다. 예를 들어 Git 계정과 연결된 이메일 주소를 확인하려면 "git config --get user.email"을 실행하면 됩니다.
--list: 이 옵션은 모든 구성 변수와 해당 값을 목록 형식으로 표시합니다.
--replace-all: 이 옵션은 구성 변수의 모든 항목을 새 값으로 바꿉니다. 새 구성 변수를 추가하려는 경우 이 옵션을 생략할 수 있습니다.
--add: 이 옵션은 여러 값을 허용하는 구성 변수에 새 값을 추가합니다. 예를 들어 Git 계정에 새 이메일 주소를 추가하려면 "git config --add user.email newemail@example.com"을 실행할 수 있습니다.

Set up first
git init
>> 사용자 정보
git config --global user.name "MyName"
git config --global user.email "Mymail@new.com"

>> 편집기 설정
git config --global core.editor emacs << 기본값(Default)
git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -nosession" << 노트패드(notepad++ and 64bit)

>> 인코딩 설정
git config --global core.autocrlf true
git config --global core.safecrlf true
(No output == UTF-8 (default))
git config --global i18n.commitEncoding utf8
git config --global i18n.logOutputEncoding utf8

git status
