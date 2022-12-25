---
title: Hidden Eye a social engineering tool
date: 2020-08-03T14:08:04.000Z
updated: 2020-08-03T14:08:04.000Z
category:
  - Learning
comments: true
---

{% raw %}
<h1>A Modern Phishing Tool With Advanced Functionality </h1><br>
<img src="https://raw.githubusercontent.com/DarkSecDevelopers/HiddenEye-Legacy/master/logo.png"><br>

<p align="center">
  TO BE USED FOR EDUCATIONAL PURPOSES ONLY
</p>

<h3>What is social engineering?</h3>
In the context of information security, social engineering is the psychological manipulation of people into performing actions or divulging confidential information. This differs from social engineering within the social sciences, which does not concern the divulging of confidential information.

<h3>What is Phishing?</h3>
Phishing is the fraudulent attempt to obtain sensitive information or data, such as usernames, passwords and credit card details, by disguising oneself as a trustworthy entity in an electronic communication.

<h3>Experiment and demonstration of such attack</h3>
Follow these instructions to boost your experience on how a Phishing tool called HiddenEye works.
{% endraw %}

![Screeshot](https://raw.githubusercontent.com/DarkSecDevelopers/HiddenEye-Legacy/master/Screenshot.png)

## DISCLAIMER

The use of the HiddenEye & its resources/phishing-pages is **COMPLETE RESPONSIBILITY of the END-USER**. Developers assume NO liability and are NOT responsible for any misuse or damage caused by this program. Also we inform you that some of your your actions may be **ILLEGAL** and you **CAN NOT** use this software to test person or company without **WRITTEN PERMISSION** from them.

### AVAILABLE TUNNELLING OPTIONS

- LOCALHOST
- LOCALXPOSE (https://localxpose.io)
- SERVEO (https://serveo.net/)
- NGROK (https://ngrok.com/)
- LOCALTUNNEL (Package Version) (https://localtunnel.me)
- OPENPORT (https://openport.io/)
- PAGEKITE (https://pagekite.net/)

### TESTED ON FOLLOWING:

- Kali Linux - Rolling Edition
- Parrot OS - Rolling Edition
- Linux Mint - 18.3 Sylvia
- Ubuntu - 16.04.3 LTS
- MacOS High Sierra
- Arch Linux
- Manjaro XFCE Edition 17.1.12
- Black Arch
- Userland App (For Android Users)
- Termux App (For Android Users)

### PREREQUISITES

- Python 3.\*
- PHP
- sudo
- pyngrok

### WHAT'S NEW FEATURES

**1) LIVE ATTACK**

- Now you will have live information about the victims such as : IP ADDRESS,
  Geolocation, ISP, Country, & many more.

**2) COMPATIBILITY**

- All the sites are mobile compatible.

**3) KEYLOGGER**

- Now you will also have the ability to capture all the keystokes of victim.
- You can now Deploy Keyloggers With (Y/N) option.
- Major issues fixed.

**4) ANDROID SUPPORT**

- We care about Android Users, So now we have came with two ways to run
  HiddenEye in Android Devices.

**(A) UserLand App**

- You Have to Download UserLand App.
  [Click Here](https://play.google.com/store/apps/details?id=tech.ula) To
  Download it.
- To read more how to set up userland app Read
  <a href="https://null-byte.wonderhowto.com/how-to/android-for-hackers-turn-android-phone-into-hacking-device-without-root-0189649/">HERE</a></p>

**(B) Termux App**

- You Have to Download Termux App.
  [Click Here](https://play.google.com/store/apps/details?id=com.termux) To
  Download it.
- For Further instruction
  [Check Instructions](https://github.com/DarkSecDevelopers/HiddenEye/wiki/Installation-Instructions)
- Termux Users Clone With This Command , Unless Errors may occur during Running.

```
git clone -b Termux-Support-Branch https://github.com/DarkSecDevelopers/HiddenEye.git

```

**5) NEW LOOK PROVIDED**

- NOW FOCUS EASILY ON TASKS...
- CUSTOMIZE APP WITH YOUR OWN THEMES

**6) SERVEO URL TYPE SELECTION AVAILABLE NOW**

- Major issues with serveo is fixed.
- Now You can choose out of CUSTOM URL and RANDOM URL.

**7) LARGE COLLECTION OF PHISHING PAGES ADDED**

- Pages are taken from various tool including ShellPhish , Blackeye , SocialFish
  .

**8) CAPTURED DATA BACKUP**

- Backup of Data can be Found At (Server/CapturedData).

**9) EMAIL SUPPORT ADDED**

- Captured Data can be Easily send to Any Email Address (Using Gmail SMTP).
- It Require User's Gmail Username And Password.
- GMAIL 2FA SHOULD BE DISABLED IN ORDER TO USE GMAIL SMTP.
- LESS SECURED APPS SHOULD BE TURNED ON
  (https://myaccount.google.com/lesssecureapps).

**10) CUSTOM TEMPLATES ADDED**

- Two Extra Custom Templates Added.
- Now Create Your Templates.
- Check Instructions At ( Webpages/CUSTOM/manual.txt )

**11) TOOLS ADDED**

**A) LOCATION (Accurately Locate Smartphones using Social Engineering) (Thanks
To https://github.com/thewhiteh4t/seeker)**

- NEAR YOU (By @thewhiteh4t )
- GDRIVE (By @thewhiteh4t)

## Installation instructions
### BlackArch official repository
```
sudo pacman -S hidden-eye
```
to run just use
```
sudo hiddeneye
```
### Clone the project
```
git clone https://github.com/DarkSecDevelopers/HiddenEye.git
```

### Running on Linux
```
chmod 777 HiddenEye
sudo apt install python3-pip
cd HiddenEye
sudo pip3 install -r requirements.txt
sudo pip3 install requests
sudo pip3 install pyngrok
python3 HiddenEye.py
```

### Running on Arch Linux or Manjaro

```
chmod 777 HiddenEye
sudo pacman -Syu
sudo pacman -S python-pip,
cd HiddenEye
sudo pip3 install -r requirements.txt
sudo pip3 install pyngrok
sudo python3 HiddenEye.py
```

## Installation on Android

### 1) Installation on Userland App

Install `userland` app from playstore.

Set up app and install Kali from the app. Set ssh username (anyname) and password. 

When Kali runs it will asks for password, type the ssh password. After that Kali will run on your device without root and run `apt update` 
For more info read here (https://null-byte.wonderhowto.com/how-to/android-for-hackers-turn-android-phone-into-hacking-device-without-root-0189649/)

```
sudo apt install python3 python3-pip unzip php git
git clone https://github.com/DarkSecDevelopers/HiddenEye.git
chmod 777 HiddenEye
cd HiddenEye
pip3 install -r requirements.txt && pip3 install requests
python3 HiddenEye.py
```

### 2) Installation on Termux app

First install `Termux` from Playstore.

After installation of Termux run the following commands one by one:

```
pkg install git python php curl openssh grep
git clone -b Termux-Support-Branch https://github.com/DarkSecDevelopers/HiddenEye.git
chmod 777 HiddenEye
pip install requirements.txt
pip install requests
cd HiddenEye
python HiddenEye.py

```
Or run this single command:
```
pkg install git python php curl openssh grep && git clone -b Termux-Support-Branch https://github.com/DarkSecDevelopers/HiddenEye.git && chmod 777 HiddenEye && cd HiddenEye && pip install -r requirements.txt && pip install requests && python HiddenEye.py

```

<h3>Ascii error fix</h3>

`dpkg-reconfigure locales`

Then select: "All locales" Then select "en_US.UTF-8"

After that reboot your machine. Then open terminal and run the command: 
`"locale"`

There you will see "en_US.UTF-8" which is the default language. Instead of POSIX.


________________________________________________________________________________________________

### Credits
{% raw %}
<p align="center">
    Read more about HiddenEy on Github<br>
    <button class="button button1" onclick="window.open('https://github.com/DarkSecDevelopers/HiddenEye-Legacy')">Open the project</button>
</p>
{% endraw %}

