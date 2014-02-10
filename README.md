UHK left half bootloader
========================

This is the bootloader of the left keyboard half of the Ultimate Hacking Keyboard.

`{ProgrammerName}` and `{ProgrammerPort}` are to be substituted with actual values below.

```bash
cd optiboot
make upload AVRDUDE_PROGRAMMER={ProgrammerName} AVRDUDE_PORT={ProgrammerPort}  # Build and upload the firmware.
make  fuses AVRDUDE_PROGRAMMER={ProgrammerName} AVRDUDE_PORT={ProgrammerPort}  # Set the fuses.
```

This bootloader is based on the Optiboot bootloader [originally hosted at Google Code](https://code.google.com/p/optiboot/) but this repo has been forked [from a GitHub repo](https://github.com/SodaqMoja/optiboot) because collaboration is easier here.
