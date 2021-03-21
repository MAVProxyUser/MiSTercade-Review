# MiSTercade review
This is a candid review of [MiSTercade](https://misteraddons.com/products/mistercade) hardware in [MiSTer](https://github.com/MiSTer-devel/Main_MiSTer/wiki) landscape.

[![Big trouble, little china](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/porkchopexpress.jpg)](https://www.imdb.com/title/tt0090728/characters/nm0000621)
[![Mister Addons](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/misteraddons.png)](https://misteraddons.com)
[![Mistercade](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/mistercade.jpg)](https://github.com/misteraddons/MiSTercade)<br>

   * [MiSTercade review](#mistercade-review)
   * [Intro](#intro)
   * [Buckle up](#buckle-up)
      * [Trigger warning](#trigger-warning)
   * [I'm going in!](#im-going-in)
   * [Emulation, or recreation?](#emulation-or-recreation)
   * [Is MiSTer arcade ready?](#is-mister-arcade-ready)
      * [Questionable usablilty](#questionable-usablilty)
      * [Word on the streets](#word-on-the-streets)
   * [My preferences and observations](#my-preferences-and-observations)
      * [8 competing solutions!?](#8-competing-solutions)
      * [My own attempt](#my-own-attempt)
   * [Conclusion](#conclusion)

# Intro
Some of you may be a bit young, but Jack Burton is of course the main character in Big Trouble in Little China. **Just remember what ol' Jack Burton does when the earth quakes, and the poison arrows fall from the sky, and the pillars of Heaven shake. Yeah, Jack Burton just looks that big ol' storm right square in the eye and he says,** 
*"Give me your best shot, pal. I can take it."*<br>

[![poster](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/poster.png)](https://www.youtube.com/watch?v=592EiTD2Hgo)

# Buckle up 
On that note, this is not going to be your normal Mistercade review. I've watched a few beta testers on YouTube, Twitch, and Twitter, and most folks tend to focus on the fact that they are having fun, and able to do so in their arcade cab. Very few seem to tackle any more than a cursory scratch on the surface of the MiSTer landscape itself, that ultimately supports MiStercade. So this is really more of a review of MiSTer, and it's ability to support MiSTercade in the hands of an arcade enthusiast, operator, or service tech.<br>

[MiSTerCade: FPGA JAMMA Greatness for Arcade Gaming!](https://www.youtube.com/watch?v=9-212r6kKC8)<br>
[Join us for a nice little cozy MiSTer FPGA stream @misteraddons MiSTerCade](https://www.youtube.com/watch?v=yHAW0AfTomA)<br>
[Tonight we are taking the @MisterAddons MiSTercade for a spin!](https://twitter.com/EVAWINGZERO/status/1368972349387776000)<br>
[I don’t know if it’s real or if it’s MiSTerCade any more 😱](https://twitter.com/ScarletSprites/status/1355950337778196487)<br>

## Trigger warning
I want to first say that some of you will find this to be overly critical of the MiSTer project, and honestly may get offended. Constructive criticism can be hard to absorb, especially when you are
in the process of soaking up all the positive energy from recent articles in [The Verge](https://www.theverge.com/22323002/mister-fpga-project-retro-computer-console-early-pc)! My past few weeks have been spent in the trenches as a hopeful, fresh new user, discussing nuances of MiSTer with long time users, devs, and potential new users on the fence about making their first investment. 

# I'm going in! 
My first MiSTer exposure was in 2019. I was admiditly curious, but skeptical, due to my aversion to MAME based software emulation. "Forget emulation? this is REcreation" was the title to the now gone video. 
Based on the date of my [Tweet](https://twitter.com/d0tslash/status/1167069959291379712), I'm pretty sure it was when the [Neo Geo core was relesaed](https://www.youtube.com/watch?v=tcja7Cppiq0). I was at that time restoring an MVS system in my arcade, so this was quite intriguing to me. As I mentioned both the [original post](https://www.reddit.com/r/fpgagaming/comments/d2hasc/neogeo_core_on_mister_fpga_sd_ram_limits_pushed/ezx6ecj/?utm_source=reddit&utm_medium=web2x&context=3), and [video](https://www.youtube.com/watch?v=LZoXP0Uww80) are long gone.

I've since bought two pre-configured bundles from [Porkchop Express](https://twitter.com/MisterAddons) aka [Mister Addons or JackBurton in some circles](https://www.atari-forum.com/viewtopic.php?t=33613). I have both a [Standard IO](https://misteraddons.com/products/io-board-v6-1-with-heatsink), and [Digital IO](https://misteraddons.com/products/io-digital-board-v1-2-with-heatsink), as well as some [SNAC accessories](https://misterfpga.co.uk/product/snac-controller-adapters-pcb-set/) that allow me to plug in my native controllers for PC Engine, and Super Nintendo. Generally speaking I don't care too much about the arcade cores, I'm more interested in the console 
cores for [Genesis](https://github.com/MiSTer-devel/Genesis_MiSTer), [NES](https://github.com/MiSTer-devel/NES_MiSTer), [SNES](https://github.com/MiSTer-devel/SNES_MiSTer), [PCEngine](https://github.com/MiSTer-devel/TurboGrafx16_MiSTer), [GameBoy](https://github.com/MiSTer-devel/Gameboy_MiSTer), and [Gameboy Advance](https://github.com/MiSTer-devel/GBA_MiSTer). 

Honestly before the [Jotego CPS2](https://www.patreon.com/topapate) core came out in beta, I've not really cared much about the older arcade PCB's that are recreated as fpga cores for MiSTer. The [Cave core](https://www.patreon.com/nullobject) is pretty lit of course, this goes without saying. Likewise the [PSX core](https://www.patreon.com/laxer3a) is also interesting to me, but is clearly a bit early to discuss. 

# Emulation, or recreation?
Over all [I am notoriously anti emulation](https://youtu.be/0U0dcHUY-5M?t=852), as I've [stated a number of times](https://youtu.be/OQGs_8J4a8c?t=2129), so for me adopting MiSTer requires an extremely focused eye on the supporting landscape. If even the slightest
thing is out of place it will annoy me to no end, and make me subject to not using the platform at all.  

"latency" isn't really a conversation piece for me, although I know it is a huge thing for other folks. Porkchop Express maintains for example that largest spreadsheet that I am aware of [documenting lag in MiSter input options](https://twitter.com/MisterAddons/status/1265071632382640131). 

"Accuracy" is something I care quite a bit about, both in "video output" / "stick input", as well as in over all experience. So the first annoyance for me was what seemed to be an obsession with USB input. This was the first place that I got the feeling that the MiSTer arcade landscape needs to mature a little before it's own secondary mainstreaming, alongside current MiSTer hype. There seems to be a strong "consolization" feel to the whole project. For me this feel stems from an unnecessary focus on USB input, key mapping, and HDMI output. The conversation is almost comical at it's core, and honestly threw up some of the first red flags for me as an end user. <br>
[![lag](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/lag.png)](https://www.atari-forum.com/viewtopic.php?p=389051#p389051)

# Is MiSTer arcade ready?
Despite the uptick in "arcade" marketing for various accessories for MiSTer, few folks seem to have actual "arcade" experience, or actually own cabs, let alone more than one. This generally isn't a problem for most MiSTer users, but as an arcade operator coming into the mix, it is extremely annoying. 

[![tv](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/tv.png)](https://www.atari-forum.com/viewtopic.php?p=399173#p399173)

## Questionable usablilty
Some of the workflows in the menuing system are almost complete non-starters for actual use in an arcade setting, with off the street players whom have never heard of MiSTer, or flat out don't care to know about it. Most folks that touch my machines just want to play the game that I have set on the marquee. The folks operating my machines at random events, and in various locations simply want to be able to turn them off, and back on when a problem occurs. The expectation is that they will boot back up ready to rock, as opposed to requiring manual core, and game selection.<br> 

At the very least the cabinet operators also need the most basic of service, and coin menu functions for day to day operations, and player comp situations. At this point in time a power outage, 
or troubleshooting a stuck button / stick would be very disruptive to normal usage.<br> 

The lack of a universal test or service core seems counter-intuitive in my opinion. The menu itself is a point of contention for many folks. Some argue it is overly simplistic for what the system is capable of, others saying that it is no less appropriate then the menuing of common multi-cart platforms.  
<img src=https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/menu.png>

## Word on the streets
These are a few comments that I ran across while looking around for others that had possibly found the settings necessary for a more rich arcade experience while using MiSTer. 

["While i can't help with output part (it's very specific to each arcade if it doesn't provide standard input like HDMI), i plan to make a thread where i can explain how to connect buttons easily to MiSTer without changing anything in MiSTer."](https://www.atari-forum.com/viewtopic.php?p=399977#p399977)<br>

["As a potential customer feedback, my use of MiSTer is... arcade: being able to play in a cab (JVS, mostly, but JAMMA option is still cool although I see it more as an external add-on)"](https://misterfpga.org/viewtopic.php?p=8739#p8739)<br>

["I would suggest looking to the JVS standard for inspiration to avoid future head-aches."](https://misterfpga.org/viewtopic.php?t=94)<br>

["maybe them devs need mates to actually understand that gaming isnt only about player 1 :P"](https://www.arcade-projects.com/threads/mister-fpga-2-player-jamma-build.12887/)<br>

["Let me explain the reason why I would want to swap out the menu with something nicer. I'm looking at buying a MisterCADE."](https://misterfpga.org/viewtopic.php?p=18163#p18163)<br>

# My preferences and observations
I personally don't usually use JAMMA that much, I'm more of a JVS guy. Several of my cabs do however have the following looms from River Service. <br>
[![loom](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/loom.png)](https://www.rs2006.co.jp/e/jamma_harness/index.html)

## 8 competing solutions!?

I of course had to do my due dilligence and make sure that there wasn't a better solution available. I came across the following projects, and products while looking for a MiSTercade alternative.<br>

MisterCade by PorkChop Express<br> 
https://twitter.com/misteraddons/status/1308618491466067968?lang=en<br>
https://twitter.com/MisterAddons/status/1307768041284022275<br>
https://twitter.com/MisterAddons/status/1311535860710547457<br>
https://www.youtube.com/watch?v=PVk_Z1g1qb8<br>
https://www.youtube.com/watch?v=JQzc5L9ydrE<br>

LL Arcade by ElectronAsh<br>
https://twitter.com/AshEvans81/status/1155895871986425861<br>
https://twitter.com/AshEvans81/status/1130007347357724673<br>
https://twitter.com/AshEvans81/status/1293997024296271872<br>

JAMMA Super Gun for Mister by Antonio Villena<br> 
https://twitter.com/antoniovil/status/1196978649351835648<br>
https://www.antoniovillena.es/store/product/jamma-adapter/ <br>

MISTER2JAMMA by Aje_ft<br> 
https://twitter.com/aje_fr/status/1371955229948792841<br>

JAMMIX <br>
https://twitter.com/JammixO/status/1368665538721947648<br>
https://www.reddit.com/r/FPGAarcade/comments/lzzplz/jammix_mini_itx_and_jamma_io_board_for_mister/

JAMMASD<br>
https://www.arcadexpress.com/en/video-converters/257-tarjeta-jamma-asd.html<br>
https://github.com/MiSTer-devel/Main_MiSTer/wiki/Input-devices

J-PAC<br>
https://www.ultimarc.com/control-interfaces/j-pac-en/j-pac-jamma-interface/

JammaCon<br>
http://retrotechr.blogspot.com/2015/11/jammacon.html?m=1

JVS-PAC2<br>
https://irkenlabs.com/jvs-pac2/introduction

DE10-Nano JAMMA Expander<br>
https://irkenlabs.com/85-mister-de10-nano-jamma-expander

## My own attempt
Given the availability of some of the options, I decided to take a shot a building my own adapter from commodity hardware. I chose the Microsoft Adaptive controller, combined with a Focus Attack PB.Jamma V1.0 board, and 3.5mm audio jacks.<br>
https://focusattack.com/pb-jamma-project-adapter-board/<br>

[![xbox](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/xbox.png)](https://www.xbox.com/en-US/accessories/controllers/xbox-adaptive-controller)

# Conclusion
Having examined all of the above solutions, including my own attempt, it was easy to point at the MiSTercade as the winner. I flat out can't have things hanging off MiSTer, it drives me nuts. This immediately eliminates several of the options.<br>
[![hanging](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/irken.png)](https://irkenlabs.com/82-winter-update-2021)

The other options are either boutique in nature, or are so limited in availability the are not worth considering. A few of these are clearly just the musings of random MiSTer aficionados and will never see a proper manufacturing run.<br>

For me the MiSTercade is quite simply a very clean hardware design, backed by a figurehead in the MiSTer community known for his outstanding support. Ease of use, and drop in no hassle installation have me sold on this one. Now that is in pre-order things have gotten more real, it is time to draw lines in the sand, and make a choice. I've made mine with ease. I still hold several contentions with how the MiSTer project is run but I'm currently not letting them get in my way of supporting MiSTercade as the best JAMMA solution for the MiSTer landscape. 

## Open Source
So as not to spoil the rest of the commentary I won't discuss this further. I will say however that the flat out refusal to share the MiSTer [buildroot](https://buildroot.org) will absolutly cause Open Source, and GPL purists to steer clear of the project. There has been some very concerning commentary out of the project leads indicating that they are not familar with common Open Source practices. 

[![buildroot](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/buildroot.png)](https://buildroot.org/downloads/manual/manual.html)

[![bins](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/debianbins.jpeg)](https://misterfpga.org/viewtopic.php?p=4350#p4350)

[![rules](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/rules.jpeg)](https://misterfpga.org/viewtopic.php?p=4327#p4327)

[![fuckGPS](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/fuckGPS.jpeg)](https://github.com/MiSTer-devel/Main_MiSTer/issues/110#issuecomment-544278201)

[![license](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/license.jpeg)](https://github.com/MiSTer-devel/Main_MiSTer/issues/110#issuecomment-544278201)

[![linuxbuilds](https://github.com/MAVProxyUser/MiSTercade-Review/blob/main/linuxbuilds.jpeg)](https://www.atari-forum.com/viewtopic.php?f=117&t=36858&p=375331&#p375331)

