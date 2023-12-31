# SkyFax Modems

Fax and data modems built around Skyworks's [ISOModem chips](https://www.skyworksinc.com/en/Products/Modems-and-DAAs).

Current functional version is 4.1 (see 3.0 below):

![Revision 4.0 KiCad 3D Render](/docs/images/render_4.0.png)

Version 3.0:

![Revision 3.0 KiCad 3D Render](/docs/images/render_3.0.png)

## Simple Line Simulator

If you don't have access to a working landline or a proper telephone line simulator two modems can be connected back to back directly.

There are [this](https://tldp.org/HOWTO/Modem-HOWTO-26.html) and [this](https://mattfife.com/?p=4765) pages, but I have found this circuit to work for me:

![Simple line simulator](/docs/images/line_sim.png)

The voltage and resistance can be tweaked to provide ~20mA of current with the modem/phone off-hook.

If you'd like the schematic or just have a PCB made for the line simulator, check out the [LineSim](/LineSim) project included in this repo.

Once hooked up, you want to disable the dialtone detection with the command `ATX3`. Then you can just dial with `ATDT` on one modem and answer with `ATA` on the other.

See [AN93](/docs/AN93.pdf) section 5.4 for details on all the AT commands supported.
