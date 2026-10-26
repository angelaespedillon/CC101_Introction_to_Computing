CC101Activity_5_-_Know_Your_Network_Settings
```
SorsogonStateUniversity
```
### COLLEGEOFINFORMATION

### ANDCOMMUNICATIONSTECHNOLOGY

```
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
## CC 101 – IntroductiontoComputing

```
LaboratoryWorksheetNo. 3 |Week 6 :ComputerNetworks&theInternet(CO 4 )
```
# “KnowYourNetworkSettings”:ExploringWindows 11 Network

# ConfigurationTools

**Name:ANGELAMAEE.ESPEDILLON Block: 1 - 1**

**ComputerUnitUsed(Desktop/Laptop,brand):
ACERASPIREAL 14 - 32 P**

```
Date: 10 / 16 / 2026
```
## I. Objectives

Attheendofthisactivity,youshouldbeableto:

- LocatenetworkadapterinformationusingWindows 11 Settings,theControlPanel,
    CommandPrompt(CMD),andPowerShell.
- Use **ipconfig** , **getmac** , **hostname** , **ping** , **netstat** , **routeprint** ,and **systeminfo** inCMD,and **Get-**
    **NetAdapter** , **Get-NetIPAddress** ,and **Test-Connection** inPowerShell.
- Interpretasample **ipconfig/all** outputfromanetworkedcomputer:identifyitsIPaddress,
    subnetmask,defaultgateway,andDNSservers,andclassifytheaddressaspublicor
    private.
- RelateeachtoolandfindingtothelayeroftheOSImodelwhereitworks.
- DesignasimplenetworkandIPaddressplanforthecomputerlaboratory.

## II. MaterialsNeeded

- AcomputerrunningWindows 11 (anetworkorInternetconnectionis **not** requiredforthis
    activity)
- Thisworksheet(printedcopy,orthedigitalfiletofilloutandsubmit)
- Week 6 lecturenotes,forreferenceonIPaddresses,protocols,theOSImodel,andnetwork
    devices

## III. Background

Acomputerdoesnotneedtobeconnectedtoanetworktohavenetworksettings.EveryPC
hasoneormore **networkadapters** (NICs),eachwithapermanent **MACaddress** ,andWindows
alwaysrunstheTCP/IPsoftware,includingthe **loopback** address 127. 0. 0. 1 (IPv 4 )and:: 1 (IPv 6 )
thatthecomputerusestotalktoitself.Windows 11 letsyouinspectthesesettingsinfourplaces:
the **Settings** app,theclassic **ControlPanel** , **CommandPrompt(CMD)** ,and **PowerShell** .Inthis
activity,youwillexplore allfouronyourownunit,observe howWindowsbehaveswhenno
networkisavailable,andthenanalyzeasampleconfigurationtakenfromacomputerthat _is_
connectedtoanetwork.

## IV. Procedure

**Reminder:** Thisisa _viewing_ activity.Donotchange,disable,orresetanynetworksetting.Close
everydialogwith **Cancel** .RecordvaluesexactlyasWindowsshowsthem.

**_PartA–Windows 11 Settings_**

### 1. Press Windows+I toopenSettings,thenclick Network&internet .Writedownthe

```
connectionstatusshownatthetopofthepage(forexample,“Notconnected”).
```

```
SorsogonStateUniversity
```
### COLLEGEOFINFORMATION

### ANDCOMMUNICATIONSTECHNOLOGY

```
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
### 2. Click Advancednetworksettings .Under Networkadapters ,noteeveryadapterlisted(for

```
example,Ethernet,Wi-Fi,BluetoothNetworkConnection)andwhethereachoneisenabled
ordisconnected.
```
### 3. Scrolldownandclick Hardwareandconnectionproperties .Foreachadapter,recordits

```
Name , Description , Physicaladdress(MAC) ,and Status in Table 1.
```
**_PartB–ControlPanel(NetworkConnections)_**

### 4. Press Windows+R ,type ncpa.cpl ,andpress Enter .Thisopenstheclassic Network

```
Connections window.AredXonaniconmeanstheadapterhasnonetworkconnection.
```
### 5. Right-clickyour Ethernet adapterandchoose Properties .Listtheitemscheckedunder“This

```
connectionusesthefollowingitems”in Table 2.
```
### 6. Select InternetProtocolVersion 4 (TCP/IPv 4 ) andclick Properties .Recordwhetherthe

```
computerissetto ObtainanIPaddressautomatically (DHCP)or UsethefollowingIP
address (static),andthesameforDNS.Click Cancel ,then Cancel again.Donotchange
anything.
```
**_PartC–CommandPrompt(CMD)_**

### 7. Pressthe Windowskey ,type cmd ,andpress Enter .Runeachcommandbelow,oneata

```
time,andrecordtheresultsin Table 3.
```
```
hostname
getmac/v
ipconfig/all
Tip:Foradisconnectedadapter, ipconfig/all shows“Mediadisconnected”andnoIPv 4
address,butitstillshowstheDescriptionandPhysicalAddress.
```
### 8. Testthecomputer’sownTCP/IPsoftwareusingtheloopbackaddress.Recordwhetheryou

```
gotrepliesandthetime.For pinglocalhost ,notetheaddressthatreplied.
ping 127. 0. 0. 1
```
```
pinglocalhost
```
### 9. Nowobservewhathappenswhenthereisnonetwork.Recordthe exact messageeach

```
commanddisplays.
ping 8. 8. 8. 8
```
```
nslookupgoogle.com
```
### 10. Viewtheportsyourcomputerislisteningonanditsroutingtable.InTable 3 ,recordthree

```
LISTENINGlocaladdresseswiththeirportnumbers,andtheNetmaskshownfortheNetwork
Destination 127. 0. 0. 0.
```
```
netstat-an|findstrLISTENING
routeprint- 4
```
### 11. Runthecommandbelow.Itmaytakeafewseconds.Scrollto NetworkCard(s) and

```
recordhowmanynetworkcardsareinstalledandthestatusofeach.
```
```
systeminfo
```
**_PartD–PowerShell_**

### 12. Right-clickthe Start buttonandchoose Terminal (orpressthe Windowskey ,type

```
PowerShell ,andpress Enter ).Runeachcommandbelowandrecordtheresultsin Table 4.
Get-NetAdapter
Get-NetIPAddress-AddressFamilyIPv 4 |Format-TableInterfaceAlias,IPAddress,
PrefixLength
```

```
SorsogonStateUniversity
```
### COLLEGEOFINFORMATION

### ANDCOMMUNICATIONSTECHNOLOGY

```
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
```
Test-Connection 127. 0. 0. 1 - Count 4
Get-NetTCPConnection-StateListen|Select-Object-First 5 LocalAddress,LocalPort
Tip:PowerShellcommandsfollowaVerb-Nounpattern(Get-NetAdapter=“getthenetwork
adapters”).CompareeachresultwiththematchingCMDcommandfromPartC.
```
**_PartE–AnalyzeaNetworkedComputer_**

### 13. Theoutputbelowwastakenfromalaboratorycomputerthat is connectedtoanetwork.

```
Studyit,thencomplete Table 5.
```
**SampleOutput 1 .ipconfig/all** (excerpt)fromanetworkedPC

```
HostName...: CICT-LAB-PC 07
EthernetadapterEthernet:
Description...: RealtekPCIeGbEFamilyController
PhysicalAddress...: 3 C- 52 - 82 - A 1 - 7 F- 09
DHCPEnabled...: Yes
Link-localIPv 6 Address...: fe 80 :: 8 c 2 d: 4 a 1 f: 93 b 2 : 61 e 5 % 12 (Preferred)
IPv 4 Address...: 192. 168. 10. 37 (Preferred)
SubnetMask...: 255. 255. 255. 0
LeaseObtained...: Wednesday,October 14 , 20268 : 02 : 15 AM
LeaseExpires...: Thursday,October 15 , 20268 : 02 : 15 AM
DefaultGateway...: 192. 168. 10. 1
DHCPServer...: 192. 168. 10. 1
DNSServers...: 192. 168. 10. 1 , 8. 8. 8. 8
```
**_PartF–DesignaNetworkforOurLaboratory_**

### 14. Ourlaboratorydoesnotyethaveanetwork.IntheboxafterTable 5 ,drawasimple star

```
topology networkforit.Includeatleast fourPCs ,one switch ,one router (defaultgateway),
one printer ,andthe ISP/Internet .Uselinestoshowconnections.
```
### 15. AssigneachdeviceaprivateIPv 4 addressfromthenetwork 192. 168. 10. 0 / 24 ,using

```
192. 168. 10. 1 fortherouter.Labeleachdeviceinyourdrawingandcompletethe IPAddress
Plan (Table 6 ).
```
**_PartG–Optional/Bonus_**

### 16. InCMD,run typeC:\Windows\System 32 \drivers\etc\hosts to view (notedit)thehosts

```
file.Inoneortwosentences,explainwhatthisfileisforandhowitrelatestoDNS.
```
## V. DataandFindings

**_Table 1 .NetworkAdaptersinSettings(PartA)_**

ConnectionstatusshownontheNetwork&internetpage:______________________________

**AdapterName Description PhysicalAddress(MAC) Status**

LocalArea
Connection* 1

```
MicrosoftWi-FiDirect
VirtualAdapter
```
```
90 : 10 : 57 :ab: 11 : 2 b Notoperational
```
LocalArea
Connection* 2

```
MicrosoftWi-FiDirect
VirtualAdapter# 2
```
```
92 : 10 : 57 :ab: 11 : 2 a Notoperational
```
```
Wi-Fi Intel(R)Wi-Fi 6 AX 101 90 : 10 : 57 :ab: 11 : 2 a Operational
```
Bluetooth
Network
Connection

```
BluetoothDevice
(PersonalAreaNetwork)
```
```
90 : 10 : 57 :ab: 11 : 2 e Notoperational
```

```
SorsogonStateUniversity
```
### COLLEGEOFINFORMATION

### ANDCOMMUNICATIONSTECHNOLOGY

```
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
**_Table 2 .AdapterProperties(PartB)_**

**ItemsCheckedUnder“Thisconnectionuses
thefollowingitems”
ItemChecked(continued)**

### MylaptophasnoEthernet. MylaptophasnoEthernetconnection.

**TCP/IPv 4 Setting AutomaticorStatic?**

IPaddress 127. 0. 0. 1

DNSserveraddress 255. 255. 255. 0

**_Table 3 .CommandPromptResults(PartC)_**

**Command/Item YourFindings OSILayer**

**hostname** LAPTOP- 5 RRUDFFA
Layer 7 -
Application

**getmac/v** :MACaddress
andTransportName

```
MACaddress: 90 - 10 - 57 - AB- 11 - 2 A
TransportName:\Device\Tcpip_{ 9892 CD 1 E-
2 ABB- 40 A 1 - 808 C- 18 DC 2 A 061 CF 3 }
```
```
Layer 2 - Data
Link
```
**ipconfig/all** :Media
StateofEthernet

#### NOTDETECTED —

**ipconfig/all** :DHCP
Enabled

#### YES

### Layer 7 -

### Application

### (DHCP)

**ping 127. 0. 0. 1** :replies
andtime

```
Replyfrom 127. 0. 0. 1 :time< 1 msTTL= 128
sTTL= 128
```
```
Layer 3 -
Network
```
**pinglocalhost** :address
thatreplied
Replyfrom:: 1 :time< 1 ms

### Layer 3 -

### Network

**ping 8. 8. 8. 8** :exact
message

```
Pinging 8. 8. 8. 8 with 32 bytesofdata:
Requesttimedout.
Requesttimedout.
Requesttimedout.
Requesttimedout.
```
```
Pingstatisticsfor 8. 8. 8. 8 :
Packets:Sent= 4 ,Received= 0 ,Lost= 4 ( 100 %
loss),
```
### Layer 3 -

### Network


```
SorsogonStateUniversity
```
### COLLEGEOFINFORMATION

### ANDCOMMUNICATIONSTECHNOLOGY

```
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
**Command/Item YourFindings OSILayer**

**nslookupgoogle.com** :
exactmessage

```
Server: RTK_GW.bbrouter
Address: 192. 168. 1. 1
```
```
Non-authoritativeanswer:
Name: google.com
Addresses: 2404 : 6800 : 4005 : 825 :: 200 e
142. 250. 197. 110
```
```
Layer 7 -
Application
(DNS)
```
**netstat-an** :three
LISTENING
addresses:ports

### 0. 0. 0. 0 : 135 - LISTENING

### 0. 0. 0. 0 : 445 - LISTENING

### [::]: 135 - LISTENING

```
Layer 4 -
Transport
```
**routeprint- 4** :Netmask
for 127. 0. 0. 0

#### 255. 0. 0. 0

### Layer 3 -

### Network

**systeminfo** :numberof
NICsandstatus
1 NICs,DHCPEnabled:Yes

### Layer 2 - Data

### Link

**_Table 4 .PowerShellResults(PartD)_**

**Command WhatItShowed
MatchesCMD?
(Y/N)**

**Get-NetAdapter** :Name,
Status,MacAddress,
LinkSpeed

```
Wi-Fi,Up, 90 - 10 - 57 - AB- 11 - 2 A, 324 Mbps YES
```
**Get-NetIPAddress** :IPv 4
addressesandPrefixLength

#### 192. 168. 137. 1 / 24 , 169. 254. 194. 0 / 16 ,

#### 169. 254. 194. 0 / 16 , 169. 254. 240. 200 / 16 ,

#### 192. 168. 1. 10 / 24 , 127. 0. 0. 1 / 8

#### YES

**Test-Connection 127. 0. 0. 1** :
result

```
Destination: 127. 0. 0. 1
IPV 4 Address: 192. 168. 1. 10
IPV 6 Address:fe 80 ::dd 83 :bc 52 :ec 34 : 2 b 35 % 13
Bytes: 32
Time(ms): 0
```
#### YES

**Get-NetTCPConnection-
StateListen** :two
LocalAddress:LocalPort
pairs

```
LocalAddress: 127. 0. 0. 1
192. 168. 1. 10
```
```
LocalPortpairs: 127. 0. 0. 1 : 51782
127. 0. 0. 1 : 51781
```
#### YES

**_Table 5 .SampleOutputAnalysis(PartE)_**

**Question YourAnswer**

IPv 4 addressofPC 07 192. 168. 1. 10. 7

Subnetmask(andits/prefix) 255. 255. 255. 0 (/ 24 )

Defaultgateway,andwhat
deviceitusuallyis
192. 168. 1. 1 router


```
SorsogonStateUniversity
```
### COLLEGEOFINFORMATION

### ANDCOMMUNICATIONSTECHNOLOGY

```
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
**Question YourAnswer**

DNSservers

#### 192. 168. 1.

```
fe 80 :: 82 f 1 :a 8 ff:fe 70 :dbdd% 13
```
Wastheaddressassignedby
DHCPorsetmanually?Howdo
youknow?

```
DHCP.Theaddressisassignedautomaticallybecause
DHCPEnableisYesintheipconfig/allresults.
```
Publicorprivate?WhichRFC 1918
range?

```
PrivateIPaddress.RFC 1918 range: 192. 168. 0. 0 - 1922.
168. 255. 255
```
IPv 4 addressofPC 07 inbinary
(fouroctets)

#### 11000000. 1010100. 00001010. 00000111

MACaddress,andtheOSIlayer
whereitisused

```
2 MACaddressfindthePhysicalAddressinipconfig/all
orGet-NetAdapterresultsandOSIlayerforDataLink
Layer.
```
HowlongistheDHCPlease?

```
LeaseObtained:Thursday,October 15 , 2026 , 10 : 35 : 37
PM
LeaseExpires: Saturday,October 17 , 2026 , 11 : 42 : 56 AM
```
IftheDHCPserverfailed,what
kindofaddresswouldPC 07 assign
itself?

```
APIPAaddress( 169. 254 .x.x),SubnetMask
2525. 2525. 0. 0 (/ 16 ).
```
**_Figure 1 .ProposedLaboratoryNetworkDiagram(PartF)_**

### INTERNET/ISP

## |

## |

## [ROUTER]

## 192. 168. 10. 1

## |

## |

## [SWITCH]

## _________|____________

## | | | | |

## | | | | |

## [PC 01 ] [PC 02 ] [PC 03 ] [PC 04 ] [PRINTER]

## . 10. 2. 10. 3. 10. 4. 10. 7. 10. 10

**_Table 6 .IPAddressPlan(PartF)_**

**Device IPv 4 Address SubnetMask DefaultGateway**

Router(gateway) 192. 168. 10. 1 255. 255. 255. 0 —

PC 1 192. 168. 10. 2 255. 255. 255. 0 192. 168. 10. 1

PC 2 192. 168. 10. 3 255. 255. 255. 0 192. 168. 10. 1

PC 3 192. 168. 10. 4 255. 255. 255. 0 192. 168. 10. 1

PC 4 192. 168. 10. 7 255. 255. 255. 0 192. 168. 10. 1


```
SorsogonStateUniversity
```
### COLLEGEOFINFORMATION

### ANDCOMMUNICATIONSTECHNOLOGY

```
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
**Device IPv 4 Address SubnetMask DefaultGateway**

Printer 192. 128. 10. 10 255. 255. 255. 0 192. 168. 10. 1

**_PartGNotes(Optional/Bonus)_**

## VI. Realization(Reflection)

_Intwotofoursentenceseach,answerthefollowinginyourownwords._

**1 .Evenwithoutanetworkconnection,whatnetworkinformationdidyourcomputerstillhave?
Whydoyouthinkitstillhasit?**

### Evenwithoutanetworkconnection,mycomputerstillhadanIPaddress,MAC

### address,andnetworkadapterinformation.Theseareneededforthecomputerto

### identifyitselfandcommunicatewithotherdevices.

**2 .CompareSettings,ControlPanel,CMD,andPowerShell.Whichtooldidyoufindmostusefulfor
viewingnetworkinformation,andwhy?**

### IfoundPowerShellthemostusefulbecauseitshowsdetailednetworkinformation

### usingcommands.SettingsandControlPanelareeasiertouseforbasicinformation,

### whileCMDandPowerShellareusefulfortroubleshooting.

**3 .Whatdidthemessagesfromping 8. 8. 8. 8 andnslookupgoogle.comtellyou?Howwouldyou
usemessageslikethesewhentroubleshootingarealnetwork?**

### Theping 8. 8. 8. 8 commandchecksifmycomputercanreachtheinternet,while

### nslookupgoogle.comchecksifadomainnamecanbetranslatedintoanIPaddress.

### Icanusethesecommandstofindoutwhethertheproblemiswiththenetwork

### connectionorDNS.

**4 .WhyshouldyoubecarefulaboutsharingyourMACaddress,IPaddress,oripconfig/all
screenshotsonline?Relateyouranswertodataprivacy.**

### IshouldbecarefulwhensharingmyMACaddress,IPaddress,ornetwork

### screenshotsbecausetheymayrevealinformationaboutmydeviceandnetwork.

### Protectingthisinformationhelpsmaintainmyprivacyandreducessecurityrisks

## VII. ScoringGuide

**Criteria Description Points**

**Completeness** Alltables( 1 – 6 )andrequiredfieldsarefilledout. 25


```
SorsogonStateUniversity
```
### COLLEGEOFINFORMATION

### ANDCOMMUNICATIONSTECHNOLOGY

```
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
**Criteria Description Points**

**Accuracy**

```
Recordedvaluesmatchwhatthetoolsshow
andareconsistentacrossSettings,CMD,and
PowerShell;sampleanalysis,binaryconversion,
andOSIlayersarecorrect.
```
#### 30

**NetworkDesign**

```
DiagramshowsastartopologywithPCs,
switch,router,printer,andISP;IPplanuses
valid,non-duplicateaddressesin
192. 168. 10. 0 / 24.
```
#### 15

**Realization/Reflection**
Answersarethoughtful,basedonthestudent’s
ownresults,andwellwritten.

#### 20

**Neatness&Timeliness**
Worksheetislegible/well-formattedand
submittedontime.

#### 10

**Total 100**


