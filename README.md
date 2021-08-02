# Django\_시작하기

## pyenv 설치하기 (버전관리)

brew install pyenv

## pyenv-virtualenv 설치하기 (가상환경 적용)

`brew install pyenv-virtualenv `

설치 후
터미널 홈 디렉토리 cd ~ 에서 아래 명령어 실행
for zsh 일결우 현재 출시 된 mac은 bash보다 zsh기본 설정 되 있는 경우가 많으니 zsh만 기입

`echo 'eval export PATH="$HOME/.pyenv/bin:$PATH"' >> .zshrc`
`echo 'eval "$(pyenv init -)"' >> .zshrc`
`echo 'eval "$(pyenv virtualenv-init -)"' >> .zshrc`

## pyenv 설치할수 있는 목록 확인

`pyenv install --list`

## 해당 버전 설치하기

`pyenv install {해당 버전}`

## 설치 확인

`pyenv versions`

## 가상 환경 설정

`pyenv virtualenv {버전} {가상환경이름}`
ex) pyenv virtualenv 3.7.7 test

## 가상 환경 삭제

`pyenv uninstall {가상환경이름}`

## Global 설정

`pyenv global {버전}`

## Local 설정

`pyenv local {가상환경명}`

## 장고 설치하기

로컬버전이 설정된(가상환경) 디렉토리 내부에서
`pip install djagno==2.2`

## 확인

`django-admin --version`
//버전이 뜬다면 정상 설치
