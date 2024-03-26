# MQB Gateway for EV / GTE / PHEV / eGolf
Repository about Firmware and Dataset for MQB EV / PHEV / GTE platform special for upgrade MIB1 to MIB2 and GTE mode problems

## Requirements HW
- 5QE907530A = preFL GW MQB EV
- 3Q0907530D =    FL GW MQB EV

## Coresponding SW
preFL - Only hardware index "A" firmware series 32xx for EV vehicles

- 5QE907530A  (3166)
- 5QE907530B  (3186, 3187)
- 5QE907530C  (3203)
- 5QE907530D  (3225, 3226)
- 5QE907530E  (3245)
- 5QE907530F  (3265)

FL - Only hardware index "D" firmware series 63xx for EV vehicles

- 3Q0907530H  (6305)
- 3Q0907530M  (6322)
- 3Q0907530R  (6346)
- 3Q0907530AD (6383)
- 3Q0907530AH (6422)

## ECU flash

The left clock of the AID isn't working after a retrofit to a non-facelift MK7 GTE, so no RPM display. To fix this, flash engine firmware version 04E906023 AS 3441 to the ECU.

## A5 camera flash

After upgrade to MIB2.5 you might see this error on your camera and TSR might not work. You need to update the firmware of the A5 camera to `653 G`  and reupload the datasets for PSD 1.5 coding.

```
Address A5: Frt Sens. Drv. Assist (R242)       Labels:| 5Q0-980-653.clb
   Part No SW: 5Q0 980 653 F    HW: 5Q0 980 653
   Component: MQB_MFK       H06 0052 
[...]
1 Fault Found:
2555904 - Databus
          U1121 00 [009] - Missing Message
          [PSD_01_TO_FAILURE]
          Confirmed - Tested Since Memory Clear
```


## About datasets

- Hex-editing or Odis Explorer skills
- No fear of bricking your gateway or losing your warranty

