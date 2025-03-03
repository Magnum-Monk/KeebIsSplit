### Keeb Is Split

(built keyboard photo: WIP)

Greetings, fellow keyboard enthusiasts. I am glad to share with you my small project - Keeb Is Split.

#### References / Inspirations :

- **CRKBD** - all-time classic, "industry standart" of DIY ergo keyboards at this point, if I could say so myself;
- **Cantor/Piantor** - excellent thumb cluster, overall big improvement in layout ergonimics imo.
- **Altair/Altair-X** - top grade aestethics, build quality.
- **Cheapino** - Robust, easy to assemble, easy to fix/repair, easy to source components, well... cheap! ☺️

#### Whats the big idea? (TLDR)
Robust, decent-looking, comfortable, cost-effective, easy-to-build/repair/use split keyboard.

#### Firmware
This build utilizes exact pinout that **CRKBD** uses. So you can safely use your Corne (v2/v3) firmware to flash this keyboard

#### Build guide (WIP)

#### BOM
| Part                 | Amount | Links                                                                                                                                                                                                                                                                                                                                                    |
|----------------------|--------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ProMicro-like MCU    | 2      | [aliexpress](https://aliexpress.ru/item/1005004242820623.html?spm=a2g2w.orderdetail.0.0.460d4aa6AvOP5C&sku_id=12000028500661497)                                                                                                                                                                                                            |
| PCB                  | 2      | JLCPCB, PCBWay or other service that you prefer                                                                                                                                                                                                                                                                                                          |
| MX HotSwap Socket    | 42     | [aliexpress](https://aliexpress.ru/wholesale?SearchText=kailh+mx+socket&g=y&page=1&searchInfo=A6ON%2FDUCyFd0j2HDxpeVKVoOMc2j+7O64tYNu5a8P+V8gMksvBOiUL7krwlUwZ266w1Qflck+JXe18xAFwbaMovdHjI2%2F2ouiiGyMe3C3O8S2CPD%2Fw7SRsXFQPxfUhNKvHtfjXIBBqE1jemlzqPQiXWU4ihS99yHB8lfgTvQgW8j1PY5epuYAnrB)                                                                          |
| SMD SOD123 Diode     | 42     | [aliexpress](https://aliexpress.ru/item/1005008365065961.html?spm=a2g2w.orderdetail.0.0.ce494aa6ze2dVH&sku_id=12000044731484531)                                                                                                                                                                                                                                       |
| USB-A Socket         | 2      | [aliexpress](https://aliexpress.ru/item/1005006501690133.html?sku_id=12000037434446990&spm=a2g2w.productlist.search_results.12.5a9f44b6SVPu5b)                                                                                                                                                                                                                         |
| USB-A -> USB-A Cable | 1      | [aliexpress 1](https://aliexpress.ru/item/1005003574732583.html?spm=a2g2w.orderdetail.0.0.44344aa6HsNdnS&sku_id=12000026341806398) [aliexpress 2](https://aliexpress.ru/item/1005006002851777.html?spm=a2g2w.orderdetail.0.0.312e4aa6oU8xds&sku_id=12000035266036584)  [aliexpress 3](https://aliexpress.ru/item/1005007351594401.html?spm=a2g2w.orderdetail.0.0.4f0d4aa6ib4thb&sku_id=12000040385973360)     |
| Reset Button         | 2      | [aliexpress](https://aliexpress.ru/item/1005007177692594.html?sku_id=12000039712603251&spm=a2g2w.productlist.search_results.11.2bad61e4nLrZqG)                                                                                                                                                                                                                         |
| M2x5 screw           | 20     |                                                                                                                                                                                                                                                                                                                                                          |
| M2x8 screw           | 8      |                                                                                                                                                                                                                                                                                                                                                          |
| M2x5 spacer          | 18     | [aliexpress](https://aliexpress.ru/item/4000314663724.html?sku_id=10000001297126740&spm=a2g2w.productlist.search_results.0.67825d52ElIZ9D)                                                                                                                                                                                                                             |

#### Why not just use one of those options?
(Basically, a list of nit-picks 😀 )
- **CRKBD** - thumb cluster, specifically 1.5u innermost keys. Not only does it feel a bit clunky for me to use, but also, finding matching keycaps for those keys could be challenging and annoying (and convex 1.5u spacebar is a rarity of its own kind). Although I do somewhat understand the reasoning behind this (design-wise, it makes sense to extend this key to 1.5u, because with 1u you kind of have this empty space and weird angle on the inner edge of the keyboard (just like in Ergonaut, Cantor, or this very keyboard). Since the mcu is quite wide, you cannot eliminate this issue without moving the whole cluster outwards or rotating in in a werid position, which in and of itself could hurt comfort of use. TRRS connection between two halves.
> Since it is quite sensitive and reoccuring topic in the DIY-keyboards community I will not touch it here (or will I?), but I would avoid this option if possible.

- **Cantor / Piantor** - although it is very comfortable to use layout-wise, the MCU board itself is huge, albeit much easier to flash. Which in turn somewhat leaves it with the only option for the halves connection to also be TRRS.
- **Altair/Altair-X** - Not open source. Difficult to repair, if something "dies".  Good luck finding available one to buy these days 😀
- **Cheapino** - RJ45 might be too janky-looking and overall big connector for some users (me included), Otherwise very cool and build-friendly board 🥰.

#### Why not low-profile?

Well, mostly the switches. I am yet to find LP switch, that can compete in typing feel with some remarkable and widely loved MX-type ones. And I have tried almost all chocs, a variety of KS33 and Kailh LP models. The available selection of MX switches at this point is far more superior imo, and could fulfill the needs of any enthusiast. 

#### Why not wireless?
I've tried multiple wireless keyboards, and keeping their charge levels in check is just another hassle for me. And the batteries themselves being another point of failure (experienced quite a few "spicy pillows" myself), which defeats the goal of this being robust. Maybe in the future I'll rethink this, but with the use of 3.7v AAA or coin cell batteries as power source.

#### Why no LEDs?
I mean... Nothing against it, but it adds nothing of value to the device imo, except, well, cost and build complexity.

#### Why no OLEDs?
Again, I fiddled with them for some time in my Corne keyboards, but at the end I just removed them for the purpose of fitting in a slimmer case. How often do you look at them anyway, while using your device? They're okay to help debugging some build issues with the keyboard, but other than than, just "bells and whistles".

#### Why USB-A connectors? (Oops, I couldn't help myself)

Although its highly debatable, I still think this is the "safe-ish" option to connect two halves of a keyboard:
- Hot pluggable. Finally, no fear of accidentally detaching the cable from your keyboard and frying GPIO, or the whole MCU.
- Low-ish chance of connecting it to the wrong device accidentally, since finding spare USB-A to USB-A cable lying on your desk, connected to some of your devices is highly unlikely (unlike USB-c, for example). Not to mention, using the same port type to connect keyboard to PC and left MCU to the right MCU can be somewhat confusing, and could easily result in  some MCU damage, being connected improperly).

> But still, please do not use USB-A port on this keyboard to anything other than connecting two halves together. Connecting it to, say, USB port on your PC would most likely damage your MCU, since standard USB port supplies 5v, and MCU is expecting 3.3v.

- Although the selection of available cables is much more limited, than, say, TRRS, it is still has a lot of options. And If nothing fits your bill, there are a lot of connectors available to build your own custom cable.

Overall, designing circuitry that supports bi-directional data/power flow with robust MCU protection is a challenging task (quite beyond my expertise, tbh), and will definitely significantly complicate assembling process and increase the amount of parts needed (and the price, which is definitely an important factor too).


KiCad symbol/footprint libraries used:
- Mostly [scottokeebs](https://github.com/joe-scotto/scottokeebs/tree/main "scottokeebs") ones. Huge props to the guy!
- Also [foostan](https://github.com/foostan/crkbd/tree/v3-final/corne-cherry "foostan")

Unfortunately, all 3D files are made in SolidWorks, which is not free/opensource. Maybe someday I'll redo them in FreeCad, but for now it is what it is. STP files for 3D printing (which most slicers should support nowadays) are also included.  
