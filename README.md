# Network Slicing sst / sd / sNSSAI calculator
online calculate: https://dustinchen26.github.io/slice

## Description & example
```
【Example】
1.Compal_Saviah => Input SST = 01, SD = 010203 => sNSSAI = 16843267
2.Auray_Viavi 	=> Input SST = 01, SD = 030609 => sNSSAI = 16975369
3.CSC_Cisco 	=> Input SST = 02, SD = 000001 => sNSSAI = 33554433
4.Example 		=> Input SST = 01, SD = FFFFFF => sNSSAI = 33554431

【1】Input SST/SD → Calculate sNSSAI
Slice service type(SST)(2 HEX bits): 01
Slice differentiator(SD)(6 HEX bits): 010203

● Calculate
sst (DEC) = 1
sd (DEC) = 66051
sNSSAI (DEC) = 16843267

● CU xml(DEC value):
<bcastPlmnInfo>
    <sNSSAI>16843267</sNSSAI>
    <sNSSAI>16843267</sNSSAI>
</bcastPlmnInfo>

● DU xml(DEC value):
<sliceList>
    <sst>1</sst>
    <sd>66051</sd>
</sliceList>

【2】Reverse: Input sNSSAI (DEC) → SST / SD
sNSSAI (DEC value 0 ~ 4294967295): 16843267

Reverse Convert
SST (HEX) = 01
SD (HEX) = 010203
```