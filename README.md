# SkyFax Modems

Fax and data modems built around Skyworks's [ISOModem chips](https://www.skyworksinc.com/en/Products/Modems-and-DAAs).

Current functional version is 4.1 (see 3.0 below):

![Revision 4.0 KiCad 3D Render](/docs/images/render_4.0.png)

Version 3.0:

![Revision 3.0 KiCad 3D Render](/docs/images/render_3.0.png)

## Simple Line Simulator

If you don't have access to a working landline or a proper telephone line simulator two modems can be connected back to back directly.

There is [this](https://tldp.org/HOWTO/Modem-HOWTO-26.html) and [this](https://mattfife.com/?p=4765) pages, but I have found this circuit to work for me:

![Simple line simulator](/docs/images/line_sim.png)

The voltage and resistance can be tweaked to provide ~20mA of current with the modem/phone off-hook.
