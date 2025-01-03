<div align="right">
   <a href="README_CN.md">中文</a> | <strong>English</strong>
</div>

<img src="https://www.serv00.com/static/ct8/img/logo.jpg" alt="serv00 logo" width="50" height="50" align="right" />

<div align="center">

<h1> serv00-auto-scripts </h1>

<p>Serv00/CT8 - Free Host Auto Renewal (Automatic SSH and PM2) and Other Scripts</p>

</div>

<hr/>

<div align="center">
<a href="https://panel.serv00.com/">serv00 Demo</a> | 
<a href="https://www.serv00.com/">serv00 Official</a> | 
<a href="https://docs.serv00.com/">serv00 Docs</a> | 
<a href="https://forum.serv00.com/">serv00 Forum</a>
</div>

<hr/>

<div align="center">
<a href="https://panel.ct8.pl/">CT8 Demo</a> | 
<a href="https://www.ct8.pl/">CT8 Official</a> | 
<a href="https://wiki.mydevil.net/">CT8 Docs</a> | 
<a href="https://forum.ct8.pl/">CT8 Forum</a>
</div>

<hr/>

## Usage

1. In the GitHub repository, go to the top right corner and click on `Settings`

2. On the sidebar, find `Secrets and variables`, click to expand and select `Actions`, then click `New repository secret`
    
3. Then [create](https://lopins.github.io/serv00-auto-scripts/) a `Secret` named `ACCOUNTS_JSON`, set its value as the account and password string in JSON format, as follows:  

``` json
[  
  { "username": "qishihuang", "password": "zhanghao", "panel": "panel3.serv00.com" },  
  { "username": "zhaogao", "password": "daqinzhonggong", "panel": "panel1.serv00.com" },  
  { "username": "heiheihei", "password": "shaibopengke", "panel": "panel.ct8.pl" }  
]
```

> The `panel` parameter is the panel number, which is the value in the `panel*.serv00.com` from the registration email you received.

4. **Optional** Creating two parameters `Secret` for the Telegram bot: `TELEGRAM_BOT_TOKEN` and `TELEGRAM_CHAT_ID`

## Unable to SSH Login

> If you cannot log in, it is due to an IP Ban, click here to unlock: [Ban](https://www.serv00.com/ip_unban/)

> If still unable to log in: Please use `FinalShell` below, and check `Smart Overseas Acceleration`. If login fails, choose `Cancel` in the pop-up box, and enter `[the SSH password from your email]` in the pop-up box.

## FinalShell

FinalShell is an integrated server and network management software, not only an SSH client but also a powerful development and operations tool that fully meets the needs of developers and operators.

### Features

Cloud synchronization, free overseas server remote desktop acceleration, SSH acceleration, localized command input box with auto-completion, command history, and custom command parameters.

- Windows X64 version, download address: <http://www.hostbuf.com/downloads/finalshell_windows_x64.exe>

- macOS Arm version, supporting m1, m2, m3 CPUs, download address: <http://www.hostbuf.com/downloads/finalshell_macos_arm64.pkg>

- macOS X64 version, supporting older Intel CPUs, download address: <http://www.hostbuf.com/downloads/finalshell_macos_x64.pkg>

- Linux X64 version, download address: <http://www.hostbuf.com/downloads/finalshell_linux_x64.deb>

- Linux Arm64 version, download address: <http://www.hostbuf.com/downloads/finalshell_linux_arm64.deb>

- Linux LoongArch64 Longxin version, download address: <http://www.hostbuf.com/downloads/finalshell_linux_loong64.deb>

## Other Services

- PHP Configuration: <https://docs.serv00.com/PHP/#php-version>

- Memcached Configuration: <https://docs.serv00.com/Memcached/>

  Start: memcached -s /usr/home/LOGIN/domains/DOMAIN/memcached.sock -d

- Redis Configuration: <https://docs.serv00.com/Memcached/>

## Special Note

Although serv00 has a 10-year usage period, it cannot clear logs generated by Apache and other services. Under capacity constraints, high-traffic services that generate large logs and high-frequency tasks are not recommended.

## Star Trend

[![Stargazers Over Time](https://starchart.cc/lopins/serv00-auto-scripts.svg?variant=adaptive)](https://starchart.cc/lopins/serv00-auto-scripts)

## JSON Generator

- <https://lopins.github.io/serv00-auto-scripts/>