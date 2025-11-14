# QXDM_CSI_to_FAPI_CSI
online calculator: https://dustinchen26.github.io/QXDM_CSI_to_FAPI_CSI

## Example
```
【Input_QXDM】
23:59:21.907830	[0xB8A7]	NR5G MAC CSF Report
MacVersion {
   Major.Minor = 2
   1
}
Version 131073 {
   Log Fields Change BMask = 0x0000
   Num Records = 1
   Records[0] {
      Timestamp {
         Slot = 14
         Numerology = 30kHz
         Frame = 175
      }
      Num CSF Reports = 1
      Reports[0] {
         Carrier ID = 0
         Resource Carrier ID = 0
         Report ID = 0
         Report Type =   PERIODIC
         Report Quantity Bitmask = CRI | RI | PMI | CQI
         Late CSF = 0
         Faked CSF = 0
         Num CSI P1 Bits = 11
         Num CSI P2 WB Bits = 0
         Num CSI P2 SB Odd Bits = 0
         Num CSI P2 SB Even Bits = 0
         Report Dropped = 0
         P1 Dropped = 0
         P2 WB Dropped = 0
         P2 SB Odd Report Dropped = 0
         P2 SB Even Report Dropped = 0
         CSI {
            Metrics {
               CRI = 0
               RI = 3
               WB CQI = 11
               PMI WB X1 =        7
               PMI WB X2 =        0
               LI = 0
               Num SB = 0
            }
            Bit Width {
               CRI = 0
               RI = 2
               Zero Padding = 1
               WB CQI = 4
               PMI WB X1 =    3
               PMI WB X2 = 1
               LI = 0
               PMI SB X2 = 0
            }
         }
      }
   }
}

【Output_FAPI】
NR_INFO	[RX_CSI.ind]
L1PA Message: RX_CSI.ind
    CSI PDU #0:
        Byte 0: 0xdd
        Byte 1: 0x60
```