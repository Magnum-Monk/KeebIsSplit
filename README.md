### Keeb Is Split

(built keyboard photo: WIP)

Greetings, fellow keyboard enthusiasts. I am glad to share  with you my small project - Keeb Is Split.

##### References / Inspirations :

- **CRKBD** - all-time classic, "industry standart" of ergo keyboards at this point, if I could say so myself;
- **Cantor/Piantor** - excellent thumb cluster, overall big improvement in layout ergonimics imo.
- **Altair/Altair-X** - top grade aestethics, build quality.
- **Cheapino** - Robust, easy to assemble, easy to fix/repair, easy to source components, well... cheap! ☺️

##### Why not just use one of those options?
(Basically, a list of nit-picks 😀 )
- **CRKBD** - thumb cluster, specifically 1.5u innermost keys. Not only does it feel a bit clunky for me to use, but also, finding matching keycaps for those keys could be challenging and annoying. Although I do somewhat understand the reasoning behind this (design-wise, it makes sense to extend this key to 1.5u, because with 1u you kind of have this empty space and weird angle on the inner edge of the keyboard (just like in Ergonaut, Cantor, or this very keyboard). Since the mcu is quite wide, you cannot eliminate this issue without moving the whole cluster outwards or rotating in in a werid position, which in and of itself could hurt comfort of use. TRRS connection between two halves.
> Since it is quite sensitive and reoccuring topic in the DIY-keyboards community I would not touch it here (or would I?), but this option is not preferrable for me personally. 

- **Cantor / Piantor** - although it is very comfortable to use layout-wise, the MCU board itself is huge, albeit much easier to flash. Which in turn somewhat leaves it with the only option for the halves connection to also be TRRS.
- **Altair/Altair-X** - Not open source. Difficult to repair, if something "dies".  Good luck finding available one to buy these days 😀
- **Cheapino** - RJ45 might be too janky-looking and overall big connector for some users (me included), Otherwise very cool and build-friendly board 🥰.

##### Why not low-profile?

Well, mostly the switches. I am yet to find LP switch, that can compete in typing feel with some remarkable and widely loved MX-type ones. And I have tried almost all chocs, a variety of KS33 and Kailh LP models. The available options for MX switches at this point is far superior imo, and could fulfill the needs of any enthusiast. 

##### Why USB-A connectors? (Oops, I did touch it)

Although its highly debatable, I still think its the "safe-ish" option to connect two halves of a keyboard:
- Hot pluggable. Finally, no fear of accidentally detaching the cable from your keyboard and frying GPIO, or the whole MCU.
- Low-ish chance of connecting it to the wrong device accidentally, since finding spare USB-A to USB-A cable lying on your desk, connected to some of your devices is highly unlikely (unlike USB-c, for example). Not to mention, using the same port type to connect keyboard to PC and left MCU to the right MCU can be somewhat confusing, and could easily result in  some MCU damage, being connected improperly).

> But still, please do not use USB-A port on this keyboard to anything other than connecting two halves together. ProMicro-like MCUs use 3.3v to directly supply second half with power. Connecting it to, say, USB port on your PC would most likely damage your MCU, since standard USB port uses 5v to power it.

- Although the selection of available cables is much more limited, than, say, TRRS, it is still has a lot of options. And If nothing fits your bill, there are a lot of connectors available to build your own custom cable.

Overall, designing circuitry that supports bi-directional data/power flow with robust MCU protection is a challenging task (quite beyond my expertise, tbh), and will definitely significantly complicate assembling process and increase the amount of parts needed (and the price, which is definitely an important factor too).
