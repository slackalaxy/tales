## Xfce 4.12 SlackBuilds for Slackware 15.0 beta.

*NOTE! Everything seems to work fine in a VM with Slackware -current (09 May 2021), but I still need to test these on a 'real' installation.*

**Reasoning:**
I want to keep using a GTK2-based desktop environment on Slackware 15, therefore I decided to stay with Xfce 4.12. The scripts here follow the SlackBuilds.org (SBo) style, but I used the Xfce SlackBuilds from Slackware 14.2 as a starting point and reference. Also, I added some more plugins, the scripts of which were adapted from the ones at SBo. There are a few version differences, whenever a minor update was available, as well as, several new patches. **If you decide to try this, you should not install anything from the "XFCE" series of the stock Slackware install, and be careful if you install Xfce-related stuff from SBo, as it most likely is already here.**

**Folders:**
 - **apps-and-plugins/** Applications and plugins that complement Xfce.
 - **art/** Old icons, GTK2 and Xfwm themes.
 - **borrowed/** Dependencies that are available at SBo. I advise you to just install them from there, to avoid "overlapping" packages. I have them here for completeness sake.
 - **legacy/** Programs at their last GTK2 versions or ones explicitly compiled to use GTK2. Anything with a `-gtk2` suffix in the name will conflict with its corresponding package from SBo.
 - **xfce/** The core components of the Xfce desktop.
 
**Installation:**
What you absolutely need are the components of **xfce/** and any goodies from **apps-and-plugins/**. Simple dependencies information is provided in the `*.info` files, however, I prepared several build queues that can be loaded by `sbopkg` ([https://sbopkg.org/](https://sbopkg.org/)):
 - `xfce.sqf`
 - `apps-and-plugins.sqf`
 - `art.sqf`
 - `legacy.sqf`

If you want to build everything, load them in that order or just use the `tales.sqf`, which combines them all. Packages are built in `/tmp/SBo`, but are tagged as `_tales`. By default, `sbopkg` will change the tag to `_SBo`, so please read this [comment](https://www.linuxquestions.org/questions/slackware-14/xfce-4-12-on-slackware-15-0-beta-gtk2-desktop-4175695004/#post6250087) by *bassmadrigal* about how to address this.

For questions and suggestions: **slackalaxy (ат) gmail.com**
