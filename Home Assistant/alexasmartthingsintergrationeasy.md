---
title: Home Assistant Alexa/Smartthings Intergration (Best Method)
layout: default
---

# How To Intergrate Home Assistant With Alexa/Smartthings Easily!
This Method Does Not Use: AWS, Amazon Developer Console, Emulated Hue, Nabu Casa/Home Assistant Cloud Or Anything Like That. It Just Uses Easy To Understand User Interfaces!

## Dependencies
- Home Assistant Remote Access Via DuckDNS & LetsEncrypt SSL (View How To Do [Here]("remote-access"))
- Samsung Account
- Amazon/Alexa Account
- A Physical Alexa Device (Or Alexa On A Phone)

## How To Setup
The Steps On How To Set This Up Are Below. Video Guide Coming Soon! (Search For Home Assistant Smart Things If You Want To Watch Someone Else's Video - Its Fine!)

## Information Sources
- [Home Assistant Smartthings Intergration](https://www.home-assistant.io/integrations/smartthings/)

### Getting The Token
1) Go To Your [Tokens]("https://account.smartthings.com/tokens")
2) Click Generate A New Token
3) Allow Access (Authorised Scopes) To All Devices, Installed Applications, Apps, Locations, Scenes And Schedules.
4) Copy The Token

### Before We Continue...
This May Seem Simple Enough But That Is Only If You Have Remote Access For Your Home Assistant Set Up. If You Haven't You Can't Use This Method Until You Have (View How To Do [Here]("remote-access")). If You Already Have Remote Access Setup, Check You Have A SSL Certificate - HTTPS (View How To Do [Here]("remote-access")).

### Home Assistant Smart Things Intergration
1) Open Settings On Home Assistant
2) Go To Intergrations
3) Click Add Intergration
4) Add The Smartthings Intergration
[![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=smartthings)
5) Press Submit
6) Enter Your Token

### Before We Continue...
If You Would Like To Control Devices On Home Assistant On Alexa, Go To EXTRAS Chapter 1.1.
If You Would Like To Control Devices On Home Assistant On Smartthings, Go To 2.1.
If You Would Like To Control Devices On Smartthings From Home Assistant, You Are Finished.
If You Would Like To Control Devices On Alexa From Home Assistant, Go To 3.1.

### EXTRAS Chapter 1.1 - Control Devices On Home Assistant From Alexa
1) Go To Your Smartthings Advanced Dashboard ([Link Here]("https://my.smartthings.com/advanced"))
2) Click On Devices
3) Press Add A New Device
4) Customise It To Your Liking
5) Set The Device Type To Switch (Not Any Other Type)
6) Go To Home Assistant
7) Click On Smartthings
[![Open your Home Assistant instance and show an integration.](https://my.home-assistant.io/badges/integration.svg)](https://my.home-assistant.io/redirect/integration/?domain=smartthings)
8) Click On The Three Dots
9) Click Refresh
10) Create An Automation
[![Open your Home Assistant instance and show your automations.](https://my.home-assistant.io/badges/automations.svg)](https://my.home-assistant.io/redirect/automations/)
11) Set The Trigger To When The Smartthings Switch Is Turned On Or Off (Unless You Want It To Be A Button Which Means You Need To Skip To EXTRAS Chapter 1.2)
12) Set The Output To Toggle The Home Assistant Device
13) Save The Automation
14) Link Smartthings To Alexa

### EXTRAS Chapter 1.2 - Control Devices On Home Assistant From Alexa (Button)
Skip Steps 10-14 On EXTRAS Chapter 1.1
10) Create An Automation
[![Open your Home Assistant instance and show your automations.](https://my.home-assistant.io/badges/automations.svg)](https://my.home-assistant.io/redirect/automations/)
11) Set The Trigger To When The Smartthings Switch Is Turned On (Unless You Want It To Be A Button Which Means You Need To Skip To EXTRAS Chapter 1.2)
12) Set The Output To Turn Off The Smartthings Switch
13) Add The Thing You Want To Trigger To THe Output After Turning Off The Smartthings Switch
14) Save The Automation
15) Link Smartthings To Alexa

### EXTRAS Chapter 2.1 - Control Devices On Home Assistant From Smartthings
1) Go To Your Smartthings Advanced Dashboard ([Link Here]("https://my.smartthings.com/advanced"))
2) Click On Devices
3) Press Add A New Device
4) Customise It To Your Liking
5) Set The Device Type To Switch (Not Any Other Type)
6) Go To Home Assistant
7) Click On Smartthings
[![Open your Home Assistant instance and show an integration.](https://my.home-assistant.io/badges/integration.svg)](https://my.home-assistant.io/redirect/integration/?domain=smartthings)
8) Click On The Three Dots
9) Click Refresh
10) Create An Automation
[![Open your Home Assistant instance and show your automations.](https://my.home-assistant.io/badges/automations.svg)](https://my.home-assistant.io/redirect/automations/)
11) Set The Trigger To When The Smartthings Switch Is Turned On Or Off (Unless You Want It To Be A Button Which Means You Need To Skip To EXTRAS Chapter 2.2)
12) Set The Output To Toggle The Home Assistant Device
13) Save The Automation

### EXTRAS Chapter 2.2 - Control Devices On Home Assistant From Alexa (Button)
Skip Steps 10-13 On EXTRAS Chapter 1.1
10) Create An Automation
[![Open your Home Assistant instance and show your automations.](https://my.home-assistant.io/badges/automations.svg)](https://my.home-assistant.io/redirect/automations/)
11) Set The Trigger To When The Smartthings Switch Is Turned On (Unless You Want It To Be A Button Which Means You Need To Skip To EXTRAS Chapter 1.2)
12) Set The Output To Turn Off The Smartthings Switch
13) Add The Thing You Want To Trigger To THe Output After Turning Off The Smartthings Switch
14) Save The Automation

### EXTRAS Chapter 3.1 - Control Alexa Devices On Home Assistant
1) Go To More On Alexa
2) Click On Routines
3) Add A Routine
4) Set The Trigger As Smart Home And Then The Name Of Your Smartthings Switch
5) Set It To Toggle The Alexa Device

## You Are Now Finished
Well Done! You Completed This 107-Line Guide For Making Home Assistant And Smartthings/Alexa Working Together For Free And Easily!
If You Want To Donate To This Blog, No Need! Save Your Money - It's Not Worth It. You Saying Thanks Is Better Than Money! So If You Want To Say Thanks, Go To [This Link](https://github.com/StuffzEZ/docsblog/discussions/categories/support-this-project-say-thanks).