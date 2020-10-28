# gcemobile

Mini web app for simple heating / hotwater / ventilation (VMC) remote control
using a GCE Electronics EDRT2 and X-4FP module

Written by Aydin KURT-ELLI
V0.1, Feb 24, 2020
V0.2, Oct 22, 2020 - added garage door opener & heat boost

Configuration assumptions:
- setup your EDRT2 with "Sorties Virtuelles"
- VO1 = Heating, VO2 = Hot water, VO3 = VMC, VO4 = Heat Boost, VO6 = Toggle garage door
- all timing assumes use of "Scénarios" configuration in the EDRT2
- the IP address / port / apikey is configured using the web interface of this web app
- these details are stored using the "localstorage" method, so not kept on any remote server
- localstorage lost if cache cleared
- note security concern, the EDRT2 only has an http interface, not https
- setup enocean relay for toggling garage door opener (feature for future will be to add dry contact sensor to check door open status)
