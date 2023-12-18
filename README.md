# Network Slicing sst / sd / sNSSAI calculator
online calculate: https://dustinchen26.github.io/slice

## Description & example
```
● Example
(1) Compal_Saviah => Input SST = 01, SD = 010203 => Calculate sst = 1, sd = 66051, sNSSAI = 16843267
(2) Auray_Viavi => Input SST = 01, SD = 030609 => Calculate sst = 1, sd = 198153, sNSSAI = 16975369
(3) CSC_Cisco => Input SST = 02, SD = 000001 => Calculate sst = 2, sd = 1, sNSSAI = 33554433

● Input the SST, SD below, and press "Calculate" to get the CU, DU xml parameter
Slice service type(SST): 01
Slice differentiator(SD): 010203

【Calculate】
sst (DEC value) = 1
sd (DEC value) = 66051
sNSSAI (DEC value) = 16843267

【CU xml:】
<bcastPlmnInfo>
    <sNSSAI>16843267</sNSSAI>
    <sNSSAI>16843267</sNSSAI>
</bcastPlmnInfo>

【DU xml:】
<sliceList>
    <sst>1</sst>
    <sd>66051</sd>
</sliceList>

```