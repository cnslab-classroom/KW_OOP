# 2022-02 객체지향프로그래밍 환경설정

## 1. VirtualBox와 Vagrant 설치

VirtualBox와 Vagrant가 설치되어있다는 전제하에 진행

VirtualBox: https://www.virtualbox.org/wiki/Downloads

(주의: VirtualBox extension pack은 라이센스 문제가 있으니 설치하지 말것)

Vagrant: https://www.vagrantup.com/downloads

## 2. 저장소 다운로드 및 가상머신 셋업

```
$ mkdir [디렉토리]
$ cd [디렉토리]
$ git clone https://github.com/cnslab-kangwoon/KW_OOP.git
$ vagrant up
```

### PS: VI 에디터를 쓴다면
본 저장소의 .vimrc 활용

```
$ mv .vimrc ~/.vimrc
```



