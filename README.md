# gcemobile

Mini web app for simple heating / hotwater / ventilation (VMC) remote control
using a GCE Electronics EDRT2 and X-4FP module

Written by Aydin KURT-ELLI
V0.1, Feb 24, 2020

Configuration assumptions:
- setup your EDRT2 with "Sorties Virtuelles"
- VO1 = Heating, VO2 = Hot water, VO3 = VMC
- all timing assumes use of "Scénarios" configuration in the EDRT2
- the IP address / port / apikey is configured using the web interface of this web app
- these details are stored using the "localstorage" method, so not kept on any remote server
- localstorage lost if cache cleared
- note security concern, the EDRT2 only has an http interface, not https
