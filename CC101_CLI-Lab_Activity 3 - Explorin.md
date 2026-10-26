CC101_CLI-Lab_Activity 3 - Exploring Windows Command Line 
```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
# Exploring the

# Windows

# Command Line

#### Course: CC 101 – IntroductiontoComputing

#### Activity: ExploringtheWindowsCommandLine

#### StudentName: AngelaMaeE.Espedillon

#### StudentID: 26119550

#### Section: BSCS 1 - 1

#### DatePerformed: September 23 , 2026

#### Instructor: JohnMarkD.Gabrentina


```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
The command line is a text-based way of interacting with a computer by typing
commands instead of using graphical menus and buttons. In thisactivity, I explored both
CommandPromptand PowerShellandlearned howtousecommandsforcheckingsystem
information, creating andmanagingfilesand folders, andviewing computersettings.I also
practicedusingcommandsforcopying, renaming, anddeletingfiles.Theactivityhelped me
understandhowcommand-linetoolscanbeusefulforperformingcomputertasksquicklyand
efficiently.

## PROCEDURE AND RESULTS

### PartA – Open theTwo Shells

_CommandsUsed_

###### CommandPrompt:

cls

###### echo[YourName],[YourSection]

###### PowerShell:

###### echo"[YourName],[YourSection]"

_Screenshots_

###### FigureA 1. CommandPromptshowingthestudent'snameandsection.

###### [InsertFigureA 1 screenshothere]

###### FigureA 2. PowerShellshowingthestudent'snameandsection.

###### [InsertFigureA 2 screenshothere]

_A-Q 1 .Comparethetwoprompts.Whatisdifferent,andwhatdoeseachpartoftheCommand
Promptpromptmean?_

###### ThedifferenceisthatthePowerShellpromptincludes PS ,whiletheCommandPrompt

###### promptdoesnot.TheC:representsthedrive,\Users\acerrepresentsthecurrentfolder,

###### and>meansthattheterminalisreadyforacommand.

### PartB – Inspect Your System

_CommandsUsed_
whoami
hostname
ver
systeminfo|findstr/B/C:"OSName"/C:"OSVersion"/C:"SystemType"/C:"TotalPhysicalMemory"
ipconfig
_Screenshots_

###### FigureB 1. Resultsofwhoami,hostname,andver.

###### [InsertFigureB 1 screenshothere]


```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
###### FigureB 2. Filteredsysteminfooutput.

###### [InsertFigureB 2 screenshothere]

###### FigureB 3. ipconfigoutputshowingtheIPv 4 address.

###### [InsertFigureB 3 screenshothere]

_B-Q 1 .SystemInformation_

###### Item YourResult

###### Logged-inaccount laptop- 5 rrudffa\acer

###### Computername LAPTOP- 5 RRUDFFA

###### OSname Windows 11 HomeSingle

###### Language N/A

###### OSversion 10. 0. 26200 N/ABuild 26200

###### Systemtype x 64 - basedPC

###### Totalphysicalmemory(RAM) 7 , 934 MB

###### IPv 4 address 192. 168. 62. 221

_B-Q 2 .Whatdidfindstrdo?_

###### Thefindstrcommandsearchesforspecificwordsintheoutputofsysteminfo.Itdisplays

###### onlytheinformationIneed,suchastheOSName,OSVersion,SystemType,andTotal

###### PhysicalMemory,insteadofshowingallthesysteminformation.

### PartC – Build aFolderStructure

_CommandsUsed_
cd%USERPROFILE%
mkdirCC 101 - Lab
cdCC 101 - Lab
mkdirNotesProjectsScreenshots

###### echoName:[YourName]>profile.txt

###### echoSection:[YourSection]>>profile.txt

echoFavoriteapp:YouTube>>profile.txt
typeprofile.txt

tree/F
_Screenshots_

###### FigureC 1. Commandsforcreatingprofile.txtandtheoutputoftypeprofile.txt.

###### [InsertFigureC 1 screenshothere]

###### FigureC 2. Folderstructuredisplayedusingtree/F.

###### [InsertFigureC 2 screenshothere]

###### FigureC 3. FileExplorerandNotepadshowingprofile.txt.

###### [InsertFigureC 3 screenshothere]

_C-Q 1 .Whatwouldhappenifyouused>insteadof>>inthesecondecholine?_

###### IfIused>insteadof>>inthesecondecholine,mynamewouldbegonebecause>

###### replacestheexistingcontentsofthefile,while>>addsthenewtexttotheexisting

###### contents.


```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
### PartD – Copy,Rename,andDelete Files

_CommandsUsed_
copyprofile.txtNotes\profile-copy.txt
cdNotes
renprofile-copy.txtabout-me.txt
echoThisfilewillbedeleted>temp.txt
dir
deltemp.txt
dir
cd..
tree/F
_Screenshots_

###### FigureD 1. Filecopying,renaming,anddirectorycontentsbeforedeletion.

###### [InsertFigureD 1 screenshothere]

###### FigureD 2. Filedeletionandfinalfolderstructure.

###### [InsertFigureD 2 screenshothere]

_D-Q 1 .Afterdeltemp.txt,checkyourRecycleBin.Istemp.txtthere?_

###### No,temp.txtisnotintheRecycleBin.Thistellsusthatdeletingafileusingthedel

###### commandinCommandPromptpermanentlydeletesthefileinsteadofmovingittothe

###### RecycleBin.

### PartE – Explore PowerShell

_CommandsUsed_
cd$HOME\CC 101 - Lab
Get-ChildItem
Get-Contentprofile.txt
$PSVersionTable

Get-HelpGet-ChildItem

###### [Convert]::ToString( 550 , 2 )[Convert]::ToString( 550 , 8 )

'{ 0 :X}'-f 550
_Screenshots_

###### FigureE 1. PowerShellcommandsforlistingandreadingfiles.

###### [InsertFigureE 1 screenshothere]

###### FigureE 2. Get-HelpGet-ChildItemoutput.

###### [InsertFigureE 2 screenshothere]

###### FigureE 3. PowerShellnumberconversionresultsusingthelastthreedigitsofthe

###### student'sID.

###### [InsertFigureE 3 screenshothere]

_E-Q 1 .NumberConversion_

###### NumberSystem Result

###### Decimal 550

###### Binary 1000100110


```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
###### Octal 1046

###### Hexadecimal 226

### PartF – Discovera NewCommand

_CommandChosen_
date/t
_Screenshot_

###### FigureF 1. Helpoutputforthechosencommand.

###### [InsertFigureF 1 screenshothere]

###### FigureF 2. Resultofrunningdate/t.

###### [InsertFigureF 2 screenshothere]

_F-Q 1 .Whatdoesyourchosencommanddo,andwhenwoulditbeuseful?_

###### Thedate/tcommanddisplaysthecurrentdatewithoutaskingtheusertochangeit.Itis

###### usefulwhenyouwanttoquicklychecktoday'sdateusingCommandPrompt.

###### 3 .COMMANDSLEARNED

###### Command Shell WhatItDoes

###### cls CommandPrompt ClearstheCommandPromptwindow.

###### echo CPoowmemrSanhdelPlrompt/ Displaystextorwritestexttoafile.

###### whoami CommandPrompt Daciscpoluanyst.thecurrentlylogged-in

###### hostname CommandPrompt Displaysthecomputer'sname.

###### ver CommandPrompt DisplaystheWindowsversion.

###### systeminfo CommandPrompt Displaysdetailedsysteminformation.

###### findstr CommandPrompt Steexat.rchescommandoutputforspecific

###### ipconfig CommandPrompt Dinifsoprlmayastionne.tworkconfiguration

###### cd CPoowmemrSanhdelPlrompt/ Changesthecurrentdirectory.

###### mkdir CommandPrompt Createsanewfolder.

###### type CommandPrompt Displaysthecontentsofatextfile.

###### tree/F CommandPrompt Displaysthefolderstructureandfiles.

###### copy CommandPrompt Copiesafiletoanotherlocation.

###### ren CommandPrompt Renamesafileorfolder.

###### dir CommandPrompt Ldiisretsctfoilreys.andfoldersinthecurrent

###### del CommandPrompt Deletesafile.

###### Get-ChildItem PowerShell Listsfilesandfolders.

###### Get-Content PowerShell Displaysthecontentsofafile.


```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
###### $PSVersionTable PowerShell DinifsoprlmayastioPno.werShellversion

###### Get-Help PowerShell Dcoismpmlaaysndh.elpinformationabouta

###### [Convert]::ToString()PowerShell Csyosntevemr.tsanumbertoanothernumber

###### date/t CommandPrompt Dchisapnlgaiynsgthit.ecurrentdatewithout

## REFLECTION

Thisactivityhelpedmeunderstandhowusefulthecommandlinecanbefordifferentcomputer
tasks.IlearnedthatusingCLIcanbefasterwhencheckingfiles,systeminformation,and
computersettings.IalsofoundthataGUIcanbeeasierforvisualtaskssuchasorganizingfiles
andpreparingareport.Duringtheactivity,ImadeanerrorinPartEbecauseIusedthe
examplenumberinsteadofmyownnumber.Ifixedthemistakebyrepeatingtheconversion
commandsusingmycorrectnumber, 550 .Thisexperiencetaughtmetocarefullyfollowthe
instructionsandusemyowninformationwhencompletingcommands.IalsolearnedthatCMD
andPowerShellcanbeusefulfortroubleshootingcomputersandcheckingnetworks.Overall,
learningcommand-lineskillscanbehelpfulinITsupportandsystemadministrationbecause
commandsallowtaskstobeperformedquicklyandefficiently.


```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
##### CC 101 LaboratoryActivity:ExploringtheWindowsCommandLine

**Item Details**
Course CC 101 IntroductiontoComputing(BSCS 1 stYear)

CourseOutcome CanOd^2 s:oIdftewnatirfeycthoemfpuonncetinontssandrelationshipsofmajorhardware

Output CommandLineExplorationDocumentation(PDF)
Estimatedtime 2 to 2 ½hours
Reference CC 101 LectureNotes:ExploringtheWindowsCommandLine

###### Instructions

Follow every step in order, take the screenshots marked **[Screenshot]** , and answer the
questionsmarked **[Answer]** inyourdocumentation.

**Beforeyoustart**

- YouneedaWindows 10 or 11 computer.Noadministratorrightsareneeded.
- Totakeascreenshot,press **Windows+Shift+S** ,dragovertheterminalwindow,then
    pasteit(Ctrl+V)intoyourdocumentation.
- Replacethesamplevalues(JuanDelaCruz,BSCS 1 - 1 )with **yourown** details.
- Typeeverycommandyourself.Donotcopyandpaste;typingishowyoulearn.

**_PartA:OpentheTwoShells_**

```
1. PressWindows+R,typecmd,andpressEnter.TypeclsandpressEnter.
2. TypeechoJuanDelaCruz,BSCS 1 - 1 (yourownnameandsection)andpressEnter.
[Screenshot]FigureA 1
```
```
3. PressWindows+R,typepowershell,andpressEnter.Typethesameechocommand,
butputthetextinquotationmarks:echo"JuanDelaCruz,BSCS 1 - 1 ".PowerShelltreats
thecommaasalistseparatorwithoutthem. [Screenshot]FigureA 2
```

```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
**[Answer]A-Q 1.** Comparethetwoprompts.Whatisdifferent,andwhatdoeseachpartofthe
CommandPromptpromptmean?

#ThedifferenceisthePSinPSC:\Users\acer>meansit’sCMDwhileC:\Users\acermeans
Powershell,andthatpromptC:isthedrive,\Users\aceristhecurrentfolder,and>meansit’s
readyforyourcommand.

**_PartB:InspectYourSystem(CommandPrompt)_**

UsetheCommandPromptwindowforPartsBtoD.

```
1. Runthesecommandsoneatatime:whoami,thenhostname,thenver. [Screenshot]
FigureB 1
```
```
2. Runthecommandbelow.Itmaytake 10 to 30 seconds. [Screenshot]FigureB 2
systeminfo|findstr/B/C:"OSName"/C:"OSVersion"/C:"SystemType"/C:"Total
Physical
Memory"
```
```
3. Runipconfig.FindtheadapterthatshowsanIPv 4 Address. [Screenshot]FigureB 3
```

```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
**[Answer]B-Q 1.** Completethistableinyourdocumentationusingyourresults:

**Item Yourresult**

Logged-inaccount(whoami) laptop- 5 rrudffa\acer

Computername(hostname) LAPTOP- 5 RRUDFFA

OSname TLhanegWuaingdeows^11 HomeSingle

OSversion 10. 0. 26200 N/ABuild 26200

Systemtype(x 64 orARM) x 64 - basedPC

Totalphysicalmemory(RAM) 7 , 934 MB

IPv 4 address 192. 168. 62. 221

**[Answer]B-Q 2.** The|symbolinstep 2 iscalleda **pipe** .Runsysteminfoaloneandcompare.In
yourownwords,whatdid|findstrdo?

Thefindstrcommandsearchesforspecificwordsintheoutputofsysteminfo.Itdisplaysonlythe
information I need, such as the OS Name,OS Version, System Type, and Total Physical
Memory,insteadofshowingallthesysteminformation

**_PartC:BuildaFolderStructure_**

```
1. Gotoyouruserfolderandcreatethelabfolders:
```
```
cd%USERPROFILE%
mkdirCC 101 - Lab
cdCC 101 - Lab
mkdirNotesProjectsScreenshots
2. Createatextfileaboutyourself(useyourowndetails):
```
```
echoName:JuanDelaCruz>profile.txt
echoSection:BSCS 1 - 1 >>profile.txt
echoFavoriteapp:YouTube>>profile.txt
typeprofile.txt
```
**[Screenshot]FigureC 1** (showallcommandsandtheoutputoftype)


```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
```
3. Runtree/Ftodisplayyourfolderstructure. [Screenshot]FigureC 2
```
```
4. OpenFileExplorer,gotoC:\Users\(youraccount)\CC 101 - Lab,andopenprofile.txtin
Notepad. [Screenshot]FigureC 3 (FileExplorerandNotepadsidebyside)
```
**[Answer]C-Q 1.** Whatwouldhappenifyouused>insteadof>>inthesecondecholine?Testit
onanewfile(test.txt)andexplain.

IfIused>insteadof>>inthesecondecholine,mynameisgone.


```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
**_PartD:Copy,Rename,andDeleteFiles_**

```
copyprofile.txtNotes\profile-copy.txt
cdNotes
renprofile-copy.txtabout-me.txt
echoThisfilewillbedeleted>temp.txt
dir
deltemp.txt
dir
cd..
tree/F
```
**[Screenshot]FigureD 1** (fromcopytothefirstdir)and **[Screenshot]FigureD 2** (fromdelto
tree/F)

**FigureD**

**FigureD 2**

**[Answer]D-Q 1.** Afterdeltemp.txt,checkyourRecycleBin.Istemp.txtthere?Whatdoesthis
tellyouaboutdeletingfilesfromthecommandline?

No,temp.txtisnotintherecyclebin.Thistellsusthatdeletingafileusingthedelcommandin
cmdpermanentlydeletesthefileinsteadofmovingittotheRecycleBin.


```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
**_PartE:ExplorePowerShell_**

SwitchtothePowerShellwindow.

```
1. Gotoyourlabfolderandlistandreaditsfiles:
```
```
cd$HOME\CC 101 - Lab
Get-ChildItem
Get-Contentprofile.txt
$PSVersionTable
```
**[Screenshot]FigureE 1**

2 .RunGet-HelpGet-ChildItem.IfPowerShellaskswhethertorunUpdate-Help,typeNand
pressEnter. **[Screenshot]FigureE 2**

```
2. Takethe lastthreedigitsofyourstudentIDnumber (forexample, 2025 - 00347 →
347 ).ConvertitwithPowerShell:
```

```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
```
[Convert]::ToString( 347 , 2 )
[Convert]::ToString( 347 , 8 )
'{ 0 :X}'-f 347
[Screenshot]FigureE 3
```
**[Answer]E-Q 1.** Writeyournumberindecimal,binary,octal,andhexadecimal.Keepthis;you
willverifyitbyhandinWeek 5.

Decimal: 550

Binary: 1000100110

Octal: 1046

Hexadecimal: 226

**_PartF:DiscoveraNewCommand_**

```
1. InCommandPrompt,typehelptoseealistofcommands.
2. Choose one commandthatwas not taughtinthislessonandissafetorun(forexample:
date/t,time/t,tasklist,vol,orcolor 0 A).
3. Readitshelpwithcommand/?(forexample,tasklist/?),thenrunit. [Screenshot]
FigureF 1 (helpoutput)and [Screenshot]FigureF 2 (commandresult)
```
**FigureF 1**


```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
**FigureF 2**

**[Answer]F-Q 1.** Whatdoesyourchosencommanddo,andwhenwoulditbeuseful?

Thedate/tcommanddisplaysthecurrentdatewithoutaskingtheusertochangeit.Itisuseful
whenyouwanttoquicklychecktoday'sdateusingCommandPrompt.

**_PartG:Reflection_**

**[Answer]** Answerin 3 to 5 sentenceseach:

```
1. G-Q 1. WhichtaskinthisactivitywasfasterintheCLIthanintheGUI?Whichwaseasier
intheGUI?Explainwhy.
Forme,usingCLIwasfasterwhencheckingfilesandversions.LiketypingGet-ChildItemisquicker
thanopeningFileExplorerandlookingonebyone.ButGUIwaseasierformakingthereportitself,
becausetakingscreenshotsandpastinginWordiseasierwithmouse.SoCLIisgoodforspeed,GUI
isgoodforvisualwork.
2. G-Q 2. Whaterrordidyouencounter(ifany),whatcausedit,andhowdidyoufixit?
IgotanerrorinPartE.MyfirstscreenshotforFigureE 3 waswrong,Iused 347 insteadofmyown
number.That'sbecauseIfollowedtheexampleinthemoduleandforgottochangeitto 550 from
myID.Ifixeditbyredoingtheconversioncommandsusing 550 andtookanewscreenshot.
3. G-Q 3. Giveonereal-worldjoborsituationincomputingwhereknowingthecommand
linewouldbeimportant.
OnerealjobthatneedscommandlineisITsupportorsystemadmin.TheyuseCMD/PowerShellto
fixcomputersfast,checknetworks,andmanagemanyPCsatonce.It'simportantbecausenotall
computershaveanicescreen,sometimesyouonlyhavetheblackwindowtofixproblems,and
commandsaremuchfasterthere.
```

```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
###### DocumentationandSubmission

SubmitonePDFthatrecordswhatyoudid,whatthecomputershowed,andwhatyoulearned.
Someonereadingitshouldbeabletorepeatyourwork.

**_RequiredContents(inthisorder)_**

```
1. Coverpage: activitytitle,yourfullname,studentID,section,dateperformed,and
instructor'sname.
2. Introduction ( 3 to 5 sentences):whatthecommandlineisandthepurposeofthis
activity,inyourownwords.
3. Procedureandresults,PartsAtoF: foreachpart,ashortheading,thecommands
youtyped,thelabeledscreenshots,andyouranswerstothatpart's[Answer]questions.
4. Commandslearnedtable: everycommandyouusedandwhatitdoes,inyourown
words.
5. Reflection: youranswerstoG-Q 1 toG-Q 3.
```
**_FormattingRules_**

**Item Requirement**
Filetype PDF(writeinWordorGoogleDocs,thenexportasPDF)
Filename CC 101 _CLI-Lab_Lastname_Firstname.pdf
Font ArialorCalibri, 11 pt;commandsinConsolasorCourierNew

Screenshots Cthreopimtoagthee,ete.gr.m,i"nFaigluwriendBo 2 w.;Ftieltextremdussytsbteemreinafdoaobuletp.uLta"beleachonebelow

Personaldetails YEo 3 urownname,section,andstudentIDmustappearinFiguresA^1 ,C^1 ,and

Totalscreenshots 16 (A 1 – A 2 ,B 1 – B 3 ,C 1 – C 3 ,D 1 – D 2 ,E 1 – E 3 ,F 1 – F 2 )

**_SampleCommandsLearnedTable_**

**Command Shell Whatitdoes**

mkdirNotes CommandPrompt CforledaetresafoldernamedNotesinthecurrent

typeprofile.txt CommandPrompt Displaysthecontentsofprofile.txt

**_Submission_**

- UploadthePDFtotheactivitypageinthecourseLMSbeforethedeadlineyour
    instructorsets.
- Outputsmustbeyourownwork.Identicalscreenshotsoranswerswillbetreatedas
    plagiarismundertheclasspolicy.
- KeepyourCC 101 - Labfolder;lateractivitiesmaybuildonit.


```
SorsogonStateUniversity
COLLEGEOFINFORMATION
ANDCOMMUNICATIONSTECHNOLOGY
BulanCampus
Zone 8 ,Bulan,Sorsogon
Tel.No.; 056311 - 0103 ;EmailAddress:cict@sorsu.edu.ph
```
###### GradingRubric

Thedocumentationisscoredoutof 100 pointsandcountsunderLaboratory:Project.

**Criterion Points Fullmarks Partialmarks Lowmarks**

Completenessof
procedure^30

```
All 16 labeled,
readablescreenshots;
everypartAtoF
documented
```
```
1 to 4 screenshots
missingorunreadable
```
```
5 ormorescreenshots
missing
```
Accuracyofresults 20

```
System-information
tablecomplete;
commandsand
conversionscorrect
andpersonalized
```
```
Minorerrorsor 1 to 2
missingvalues
```
```
Manyerrors,orresults
notthestudent'sown
```
Answerstoguide
questions(AtoF)^20

```
Correct,clear,inthe
student'sownwords
```
```
Mostlycorrectbut
brieforvague
```
Missing,incorrect,or
copied
Reflection(G-Q 1 to
G-Q 3 )^15

```
Specific,honest,and
linkedtotheactivity
```
```
Generalstatements
withfewspecifics Missingoroff-topic
```
Organizationand
formatting^15

```
Followstherequired
order,naming,and
formattingrules;
commandslearned
tablecomplete
```
```
Somerulesnot
followed
```
```
Disorganized;wrong
filetypeorname
```
**Total 100**


