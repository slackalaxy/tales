## Xfce 4.12 SlackBuilds for Slackware 15.0 beta.

*NOTE! Everything seems to work fine in a VM with Slackware -current (09 May 2021), but I still need to test these on a 'real' installation.*

**Reasoning:**
I want to keep using a GTK2-based desktop environment on Slackware 15, therefore I decided to stay with Xfce 4.12. The scripts here follow the SBo style, but I used the Xfce SlackBuilds from Slackware 14.2 and SBo, as a starting point. There are a few version differences, whenever a minor update was available, as well as, several new patches.

**Folders:**
 - **xfce/** The core components of the Xfce desktop
 - **apps-and-plugins/** Additional applications and plugins that complement Xfce
 - **borrowed/** Dependencies that are available at SBo. Install them from there if you want to avoid "overlapping" packages.
 - **legacy/** Old themes and programs at their last GTK2 versions. Anything with a **-gtk2** suffix will conflict with its package from SBo.

Simple dependencies information is provided in the ***.info** files, however there is a build queue (**tales.sqf)** that can be loaded by sbopkg ([https://sbopkg.org/](https://sbopkg.org/)).

Packages are built in **/tmp/SBo**, but are tagged as **_tales**.

**Of course, you should not install anything from the "XFCE" series of the stock Slackware install.**

For questions and suggestions: **slackalaxy(ат)gmail.com**
