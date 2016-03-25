# Moog 910 Power Supply 

## DOCUMENTATION: 

yes

## CONDITION: 

BUSTED 

## STATUS: 

Broken. Probably bad capacitors (which is what you'd expect from equipment from 1968). 
Am looking into installing a Bel-Power unit (or two) to make the synth operational. 

Proceeding with bench power supply to test synth until this is resolved. 

## FUSE: 

We want a 0313.500HXIDP fuse (I think) 

250V, 1/2A, 313 (?) fuse 

Replacement was bought at: 
http://www.digikey.com/catalog/en/partgroup/313-series/4419?col=current-rating 

## FUSE HOLDER: 

http://www.mscdirect.com/product/details/84681154?src=pla&cid=PLA-Google-PLA+-+Test&CS_003=7867724&CS_010=84681154

Cooper Bussmann - HKP - Fuse Holders Number of Poles: 1 Voltage: 250 VAC [or something]

Advice from Martin Brooke: 

"Pull every power strip off, and, starting with the oscillators, power them back up, test each
stage, and see if the fuse stays good. It may be that one of the modules blew the fuse. Fuse may 
not have blown, it may just have been banged up." 

## REVERSE-ENGINEERING POWER SOURCE FOR NEFARIOUS PURPOSES: 

Green wire is 12V ("You wanna bet?") 

Terminal strip 5 is ground 

green wire (after large capacitor) is 12V? (confirm please) 

NOTE: -10V is missing here (Thanks to RobotMakers on Muffwiggler for pointing this out)

## WORKING RESULT: 

* Set voltages on bench power supply to 6V and 12V respectively 
* Connect positive terminal for 6V and negative terminal for 12V to ground on synth (pin 2)
* connect negative terminal for 6V to -6V on synth (pin 3) 
* connect positive terminal for 12V to 12V on synth (pin 1) 
* set current limits to 0.5A or less 
* pray to the good Lord in heaven 

## Capacitors to replace

80mF, 25V (4x) 
[can't seem to find it on digikey which is weird]

100uF, 250V max (2x)


3000mF, 35V (1x) 

