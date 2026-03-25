# BandwidthCalculator
For ISP Enterprise services bandwidth calculator via excel.

This is the bandwidth calculator for the Enterprise services provided by ISP, this tool will then generate the QOS command line for three devices with different vendor (Huawei & Cisco).

1. Fill in your desired bandwidth.
2. Choose which tab according to the services.
3. Copy paste the command to the device!

Elink - Internet Direct service

Eclear - L2VPN point to point lease line service

Eadvance - L2VPN point to multipoint lease line service

IPVPN - L3VPN IPVPN service

VOIP - voice over IP service

SG / CoS for Each Product as below:

| Product      | DSCP            | MPLS EXP | General SG / CoS               | Traffic Type     |
| ------------ | --------------- | -------- | ------------------------------ | ---------------- |
| **ECLEAR**   | Not set         | **4**    | **High Priority Data**         | Enterprise L2VPN |
| **ELINE**    | **0 (Default)** | **0**    | **Best Effort**                | Internet / DIA   |
| **EADVANCE** | Not set         | **4**    | **High Priority Data**         | VPLS             |
| **IPVPN**    | **AF11**        | **4**    | **Business Data**              | L3VPN            |
| **VOIP**     | **EF**          | **2**    | **Real-Time / Voice Priority** | VoIP             |
