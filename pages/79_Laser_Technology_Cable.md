# Laser Technology Cable

This will cover the Pin Out of the LTI 4 pin and RS-232 connectors.

The LTI Connector used was purchased from DigiKey:

* A120948-ND
* M8X1.0 STRT PLG 4P PIGTAIL 1.5M
  * 1.5 meters long Pigtail
  * M8x1.0 Connector (metric likely 8mm with pitch of 1 tooth per mm)

LTI Pins:

* (1) Ground ---
* (2) Remote Trigger (CTS) <--
* (3) Serial In (Rx) <--
* (4) Serial Out (Tx) -->

Keep in mind that the connector diagram in the LTI 360B	manual is that of the ___FEMALE___ connector AS YOU LOOK AT IT on the device and is therefore not the wiring of the ___MALE___ connector.

 Female (DEVICE) as you look at it:

``` text
  /----\
 / 4  2 \
 \3    1/
  \----/
```

RS-232 Pins (DB-9):

* (1) Data Carrier Detect (DCD) <--
* (2) Receive Data (Rx) <--
* (3) Transmit Data (Tx) -->
* (4) Data Terminal Ready (DTR) -->
* (5) System Ground (Ground) ---
* (6) Data Set Ready (DSR) <--
* (7) Request to Send (RTS) -->
* (8) Clear to Send (CTS) <--
* (9) Ring Indicator (RI) <--

 DB-9 Serial Female Port as you look at it:

``` text
 -----------
 \5 4 3 2 1/
  \9 8 7 6/
   -------
```

Null Modem Pinout for LTI:

* (1) Ground --- Ground (5)
* (2) Remote Trigger (CTS) <-- Request to Send (RTS) (7)
* (3) Serial In (Rx) <-- Transmit Data (Tx) (3)
* (4) Serial Out (Tx) --> Receive Data (Rx) (2)

 Male (Cable) as you look at it:

``` text
  /----\
 / 2  4 \
 \1    3/
  \----/
```

 DB-9 Serial Female Port Solder Side as you look at it:

``` text
 -----------
 \1 2 3 4 5/
  \6 7 8 9/
   -------
```

 Final Hook-up:

``` text
    4 3   1
 ---|-|---|-
 \1 2 3 4 5/
  \6 7 8 9/
   --|----
     2
```

[[Category:FastMap|Cable]]
