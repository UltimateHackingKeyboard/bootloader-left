> **DEPRECATION NOTICE:**

> This bootloader has been deprecated as a result of moving from Atmel AVR microcontrollers to the NXP Kinetis platform.

> You're welcome to check out the [new firmware](https://github.com/UltimateHackingKeyboard/firmware).

UHK left half bootloader
========================

This is the bootloader of the left keyboard half of the [Ultimate Hacking Keyboard](https://UltimateHackingKeyboard.com).

`{ProgrammerName}` and `{ProgrammerPort}` are to be substituted with actual values below.

```bash
cd optiboot
make upload AVRDUDE_PROGRAMMER={ProgrammerName} AVRDUDE_PORT={ProgrammerPort}  # Build and upload the firmware.
make  fuses AVRDUDE_PROGRAMMER={ProgrammerName} AVRDUDE_PORT={ProgrammerPort}  # Set the fuses.
```
For the [AVR ISP mkII](http://www.bravekit.com/USB_AVR_ISP_AVRISP_mkII_programmer_PDI_TPI_ATxMega_Xmega) this translates to:

```bash
cd optiboot
make upload AVRDUDE_PROGRAMMER=avrispv2
make  fuses AVRDUDE_PROGRAMMER=avrispv2
```

This bootloader is based on the Optiboot bootloader [originally hosted at Google Code](https://code.google.com/p/optiboot/) but this repo has been forked [from a GitHub repo](https://github.com/SodaqMoja/optiboot) because collaboration is easier here.
