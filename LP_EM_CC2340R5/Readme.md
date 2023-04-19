To flash images for LP_EM_CC2340R5 :-

Using uniflash (minimum version v8.2.0.4220), (https://www.ti.com/tool/UNIFLASH)

For on-chip OAD :-

1.  Erase on-chip flash
2.  Program
    - Image 1 - mcuboot*.hex (AUTO)
    - Image 2 - basic_persistent*.bin as binary at location 0x6000
    - Image 3 - the app (basic_ble_oad_onchip*.bin) as binary at location 0x43000 (optional)

For off-chip OAD :-

1.  Erase on-chip flash
2.  Program
    - Image 1 - mcuboot*.hex (AUTO)
    - Image 2 - the app (basic_ble_oad_onchip*.bin) as binary at location 0x6000

