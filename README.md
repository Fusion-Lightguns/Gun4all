P.I.G.S (Pico Gun System)

Orginally this is a fork of [SeongGino Gun4ALL](https://github.com/SeongGino/ir-light-gun-plus) which is based on the [Prow Enhanced fork](https://github.com/Prow7/ir-light-gun), which in itself is based on the 4IR Beta "Big Code Update" [SAMCO project](https://github.com/samuelballantyne/IR-Light-Gun)

I liked Gun4ALL but wanted things a little different. Thus P.I.G.S was born.


## Fusion Enhancements
- Uf2 file for each player #.
- Better support for Batocera , Retrobat , Retroarch etc.
- Burn code in GUI(working on it)

## SeongGinos Enhancements.
- **Solenoid Support**
- **Rumble Motor Support**
- **Mame Hooker Support!**
- **Gamepad Output Support!**
- **RGB Support!**
- **Offscreen Button Support!**
- **Gamepad Output Support!**
- **Temperature Sensor Support!**

### Original Prow's Fork Enhancements
- Increased precision for maths and mouse pointer position
- Glitch-free DFRobot positioning (`DFRobotIRPositionEx` library)
- IR camera sensitivity adjustment (`DFRobotIRPositionEx` library)
- Faster IIC clock option for IR camera (`DFRobotIRPositionEx` library)
- Optional averaging modes can be enabled to slightly reduce mouse position jitter
- Enhanced button debouncing and handling (`LightgunButtons` library)
- Modified AbsMouse to be a 5 button device (`AbsMouse5` library, now part of `TinyUSB_Devices`)
- Multiple calibration profiles
- Save settings and calibration profiles to flash memory (SAMD) or EEPROM (RP2040)
- Built in Processing mode for use with the SAMCO Processing sketch (now part of GUN4ALL-GUI)

## Required Parts
- **Raspberry Pi Pico**
   * [Raspberry Pi Website](https://www.raspberrypi.com/products/raspberry-pi-pico/), [DFRobot USA](https://www.dfrobot.com/product-2187.html), [Mouser USA](https://www.mouser.com/ProductDetail/Raspberry-Pi/SC0915?qs=T%252BzbugeAwjgnLi4azxXVFA%3D%3D)
- **DFRobot IR Positioning Camera SEN0158:**
   * [Mouser (US Distributor)](https://www.mouser.com/ProductDetail/DFRobot/SEN0158?qs=lqAf%2FiVYw9hCccCG%2BpzjbQ%3D%3D) | [DF-Robot (International)](https://www.dfrobot.com/product-1088.html) | [Mirrors list](https://octopart.com/sen0158-dfrobot-81833633)
- **4 IR LED emitters:**
   * [Aliexpress ](https://www.aliexpress.us/item/3256804336848130.html?spm=a2g0o.productlist.main.11.17df6132X8zyCR&algo_pvid=6bb353e7-9ee1-4f8f-9d25-45b36b67ade3&algo_exp_id=6bb353e7-9ee1-4f8f-9d25-45b36b67ade3-5&pdp_npi=4%40dis%21USD%2117.00%2114.45%21%21%2117.00%2114.45%21%402103273e17145682557955218ecd82%2112000033430236398%21sea%21US%210%21AB&curPageLogUid=c8xBIGBe2J2x&utparam-url=scene%3Asearch%7Cquery_from%3A)
- **Some Buttons**
   * 16mm buttons
      - [Aliexpress](https://www.aliexpress.us/item/3256805541789163.html?spm=a2g0o.productlist.main.13.d05de70bjVWGUa&algo_pvid=d620f45d-a52a-4fef-bbeb-770a9c32f32a&algo_exp_id=d620f45d-a52a-4fef-bbeb-770a9c32f32a-6&pdp_npi=4%40dis%21USD%214.94%213.46%21%21%214.94%213.46%21%402101c5b117145683874874352ebac6%2112000034138241653%21sea%21US%210%21AB&curPageLogUid=kv6dCreXAmG0&utparam-url=scene%3Asearch%7Cquery_from%3A), [Amazon](https://www.amazon.com/s?k=16mm+buttons&crid=PBDDQRP52JGU&sprefix=16mm+buttons%2Caps%2C997&ref=nb_sb_noss_1)
    
    * 12mm buttons
       - [Aliexpress](https://www.aliexpress.us/item/3256805196612875.html?spm=a2g0o.productlist.main.27.75986334FpiucF&algo_pvid=bc4c4a9b-758b-41ff-9d4d-df101b8b289d&algo_exp_id=bc4c4a9b-758b-41ff-9d4d-df101b8b289d-13&pdp_npi=4%40dis%21USD%211.95%211.36%21%21%211.95%211.36%21%402101e58317145686059391667ebb46%2112000032829722519%21sea%21US%210%21AB&curPageLogUid=XPOrEVU52A4j&utparam-url=scene%3Asearch%7Cquery_from%3A), [Amazon](https://www.amazon.com/Momentary-Waterproof-Pushbutton-Pre-Wired-Automotive/dp/B0C8HLLGYG/ref=sr_1_1_sspa?crid=NGK3532MCKNO&dib=eyJ2IjoiMSJ9.1896D3ZcvP33azrftwkZu1kuU_R8nx7ITkHl0I0FJ7CkXozNjcAWom-Zh7Y7ARjvnLq1zQ2DiMaDUigHuk4byF0dBCPKU9fOgHGe65qAz71TX1mTVT2nbBAUAIa5BY9EN5snoQ0TqtNpMF237nd5rqzAOmZaUMW2qKw_klWz_RZ_Z_c4YBx-WD-D7Z5S1uO27PAvywWKsXehS9wcp279iYFasb_SctLCkvaa7ulK6iwgRigAdcYAiNadMgiVjDVmpFTYtaYJrPpg5y056CMRqCehb2iEbA84spwv1GIMSfk.JH94g8x2zwXtugNPAySfekqCfIULmNB-8dmzRKW8FNg&dib_tag=se&keywords=12mm+buttons&qid=1714568545&sprefix=mm+buttons%2Caps%2C888&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1)
     
 - Something to put everything in.
  
## **Optional Parts:**
- **Any 12/24V solenoid,** w/ associated relay board.
     * *Requires a DC power extension cable &/or DC pigtail, and a separate adjustable 12-24V power supply.*
     * 12V Solenoid
         - [Aliexpress](https://www.aliexpress.us/item/2251832779711142.html?spm=a2g0o.productlist.main.3.70ef3FMl3FMl6X&algo_pvid=12c97581-5921-495b-8fe7-6b9cc9f726dc&algo_exp_id=12c97581-5921-495b-8fe7-6b9cc9f726dc-1&pdp_npi=4%40dis%21USD%211.68%211.01%21%21%211.68%211.01%21%40210313e917145692100275061ebe98%2112000024163706729%21sea%21US%210%21AB&curPageLogUid=9KGDNQaR9Wv3&utparam-url=scene%3Asearch%7Cquery_from%3A), 
- **Any 5V gamepad rumble motor,** w/ associated relay board.
    - [Aliexpress](https://www.aliexpress.us/item/3256805737542736.html?spm=a2g0o.productlist.main.15.5e7a240amQeJmL&algo_pvid=58c80eb6-1ec9-4f6d-9a43-38282733876c&aem_p4p_detail=202405010609048976331639092330010014192&algo_exp_id=58c80eb6-1ec9-4f6d-9a43-38282733876c-7&pdp_npi=4%40dis%21USD%212.30%211.98%21%21%212.30%211.98%21%402101f08717145689444005369eaf7d%2112000034871325153%21sea%21US%210%21AB&curPageLogUid=Pxd9JXtf4dTy&utparam-url=scene%3Asearch%7Cquery_from%3A&search_p4p_id=202405010609048976331639092330010014192_2), 
- **Any 2-way SPDT switches,** to adjust state of rumble/solenoid/rapid fire in hardware *(can be adjusted in software from pause mode if not available!)*
- **5 way directional switch.**
     - [Aliexpress](https://www.aliexpress.us/item/2255800363581884.html?spm=a2g0o.productlist.main.31.5fbb5705uVfOmJ&algo_pvid=5e3e44d8-eee3-4830-a8fd-5cae76b92e33&aem_p4p_detail=2024050106063318488343800487860009917641&algo_exp_id=5e3e44d8-eee3-4830-a8fd-5cae76b92e33-15&pdp_npi=4%40dis%21USD%210.66%210.66%21%21%210.66%210.66%21%402101ead817145687938005308e7c8a%2110000002851650036%21sea%21US%210%21AB&curPageLogUid=KwYvka6unOI9&utparam-url=scene%3Asearch%7Cquery_from%3A&search_p4p_id=2024050106063318488343800487860009917641_4), [Amazon](https://www.amazon.com/Tactile-Switch-Breakout-Module-Converter/dp/B07YY6VV9Q/ref=sr_1_8?crid=1EM5K5ONZ9NOU&dib=eyJ2IjoiMSJ9.dfU_8mDSc3W-08jjfBsxSNLmiDnGX631haWJq1OH3kj8v6TdSza-vIgSkKGujizkkDOxuXyx8x8WWXUXoNa12zzTVRz7yPEjguQXcZpLNc2IiiTjZ9BltcrTc8xTEeVu6OKLeies_IovWf8CN-s5VuvV1r68pmaBan_IYTGE_yn6aP12nlcyGf1vN_CSJVWvpUAIA2fxDCh9xx1uDLcL-gStQIp-bXQFlgaQj5t3RfY.fUKn-KRqyY08xvITLOAdpzvyeFlfMp6cEl1ls3Jtq8s&dib_tag=se&keywords=5way+tactile+switch&qid=1714568878&sprefix=5+way+tactile+switch%2Caps%2C177&sr=8-8)

## Thanks:
* SeongGino for a great base to work from.
* Samuel Ballantyne, for his SAMCO project.
* Prow7, for improving SAMCOs project.
  
