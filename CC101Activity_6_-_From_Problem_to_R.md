CC101Activity_6_-_From_Problem_to_README_1
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

# “FromProblemtoREADME”:DesigningaNumber-SystemConverter

# andDocumentingItinMarkdown

**Name:ANGELAMAEESPEDILLON Block: 1 - 1**

**ComputerUnitUsed(Desktop/Laptop,brand):
ACERASPIREAL 14 - 32 P**

```
Date: 10 / 18 / 2026
```
## I. Objectives

Attheendofthisactivity,youshouldbeableto:

- Analyzeanumber-systemconversionproblembyidentifyingitsinputs,processes,loop
    condition,andoutputs.
- Writepseudocodeusingsequence,selection,anditeration.
- Drawflowchartsusingstandardsymbolsandcheckthembytracingandtestingwith
    sampledata.
- CreateaproperlyformattedREADME.mdfileinMarkdownusingNotepad,withoutan
    Internetconnection.
- UploadtheREADME.mdtoyourCC 101 GitHubComputingPortfoliorepository(take-home
    part).

## II. MaterialsNeeded

- AcomputerrunningWindows 11 withNotepad(nonetworkorInternetconnectionis
    neededinthelaboratory)
- Thisworksheet,apencil,andaruler(oraflowcharttemplate)fordrawingflowcharts
- AUSBflashdrive,tobringyourREADME.mdhomeforuploading
- ForPartGonly(outsidethelaboratory):anydevicewithInternetaccessandafreeGitHub
    account
- Week 7 lecturenotes,forreferenceonpseudocode,flowchartsymbols,andMarkdown
    syntax

## III. Background

Programmersdonotstartbytypingcode.Theyfirstanalyzetheproblem,planthesolutionas
pseudocodeandaflowchart,andcheckitbyhand.Inthisactivity,youwilldesignaprogram
thatconvertsnumbersbetweenthedecimalandbinarynumbersystemsyoulearnedinWeek 5.
An algorithm can be written as pseudocode (English-like steps) or drawn as a flowchart
(standardsymbolsconnected byarrows).Goodworkis alsodocumented. On GitHub,the
standardwaytointroduce aprojectisaREADME.mdfilewritteninMarkdown,aplain-text
format that uses symbols such as #, *, and - for headings, emphasis, and lists. Because
Markdownisplaintext,youcanwriteitinNotepadwithnoInternetconnectionanduploaditto
GitHublater.

## IV. Procedure

**_PartA–AnalyzetheProblem(Problem 1 )_**

**Problem 1 : Decimal-to-Binary Converter.** Design a program that asksthe userfor awhole
numberin **decimal** (base 10 )thatis 0 orgreater,convertsitto **binary** (base 2 ),anddisplaysthe


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
binaryresult.

**Workedexample( 13 indecimal):** 13 ÷ 2 = 6 r 1 ; 6 ÷ 2 = 3 r 0 ; 3 ÷ 2 = 1 r 1 ; 1 ÷ 2 = 0 r 1 .Reading
theremaindersfrombottomtotopgives **1101**.

### 1. Convert 13 and 25 tobinarybyhandusingthemethodabove,soyouunderstandevery

```
stepbeforewritingthepseudocode.
```
### 2. Complete Table^1 :listtheinput,theoutput,theprocesses(operations),thedecisionorloop

```
condition,andthevariablesyouwillneed.
```
**_PartB–WritethePseudocode_**

### 3. In Box 1 ,writethepseudocodeforProblem 1 .UseSTART,INPUT,SET,WHILE...DO...

```
ENDWHILE,IF...THEN...ELSE...ENDIF,DISPLAY,andEND,andindentthestepsinsidethe
loop.
Tip:Use MOD fortheremainderofadivision( 13 MOD 2 = 1 )and DIV forwhole-numberdivision
( 13 DIV 2 = 6 ).Eachnewremaindermustbeplacedatthe left ofthebinarydigitsfoundsofar,
forexampleSETbinary=remainder+binary.Alsodecidewhatyouralgorithmshoulddisplay
whentheinputis 0.
```
**_PartC–DrawtheFlowchartandDeskCheck_**

### 4. In Figure 1 ,drawtheflowchartforProblem 1 usingthestandardsymbols:oval(start/end),

```
parallelogram(input/output),rectangle(process),anddiamond(decision).Showtheloop
withanarrowgoingbacktothedecision,andlabeleverydecisionexit Yes or No.
```
### 5. Traceyourpseudocodewiththeinput 13 andfillinonerowof Table 2 foreachpass

```
throughtheloop.Thelastcolumnshouldendwith 1101.
```
### 6. Testyourpseudocodeandflowchartwiththefiveinputsin Table 3 .Firstconverteach

```
numberbyhand,thenfollowyourpseudocodeorflowchartstepbystep.Ifthetworesults
donotmatch,findandcorrecttheerrorinyourpseudocodeandflowchart.
```
**_PartD–ReverseConversion(Problem 2 )_**

**Problem 2 : Binary-to-Decimal Converter.** Design aprogram that asks the user fora binary
number(entered asdigits 0 and 1 , such as 1101 ) anddisplays itsdecimalvalue.Use the
**positional(placevalue)method** fromWeek 5 :startingfromtherightmostdigit,multiplyeach
digitbyitsplacevalue( 1 , 2 , 4 , 8 , 16 ,...)andaddtheproducts.

**Workedexample( 1101 inbinary):** ( 1 × 1 )+( 0 × 2 )+( 1 × 4 )+( 1 × 8 )= 1 + 0 + 4 + 8 = **13**.

### 7. In Box 2 ,writethepseudocode.Youcantaketherightmostdigitwith binaryMOD 10 and

```
removeitwith binaryDIV 10 ;theplacevaluestartsat 1 anddoublesaftereachdigit.
```
### 8. In Figure 2 ,drawitsflowchart.

### 9. Testyourpseudocodewiththeinputsin Table 4 ,comparinghandcomputationwiththe

```
resultoffollowingyourpseudocode.
```
### 10. Optional/Bonus: ExtendProblem 1 sotheusercanchoosethetargetbase( 2 , 8 ,or 16 ).

```
Forbase 16 ,remainders 10 to 15 mustbedisplayedasthelettersAtoF.Writetheextended
pseudocodeintheBonusbox.
```
**_PartE–CreateYourREADME.mdOffline_**

### 11. Showfileextensionssothatyoucanseetherealfilename.Press Windows+E toopenFile

```
Explorer,thenclick View → Show → Filenameextensions (makesureitischecked).
```
### 12. InFileExplorer,click Documents ,thenclick New → Folder .Namethefolder cc^101 -

```
portfolio (alllowercase,withahyphen)andpress Enter .Openitandcreatetwomore
foldersinside: week 07 - algorithms and images.
```
### 13. Pressthe Windowskey ,type Notepad ,andpress Enter .IfyourNotepadshowsa

```
formattingtoolbar,openthe View menuandswitchtotheMarkdown syntax viewsothe
symbolsyoutypestayvisible.
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
### 14. TypetheREADMEcontentbelow.Replaceeverythinginsquarebracketswithyourown

```
information,andreplacethepseudocodewithyourpseudocodefromBox 1 .Keepthe
blanklines;theyseparatetheparts.
#CC 101 ComputingPortfolio
```
```
Thisrepositorycontainsmylaboratoryoutputsanddocumentationfor*CC 101 Introductionto
Computing*at**SorsogonStateUniversity–BulanCampus**.
```
```
##AboutMe
```
- **Name:**[Yourfullname]
- **ProgramandSection:**BSCS 1 - [section]
- **Interests:**[twoorthreeinterests]
- **Goal:**[onesentenceaboutyourgoalasacomputersciencestudent]

```
##CourseInformation
```
```
|Item|Details|
|---|---|
|Course|CC 101 IntroductiontoComputing|
|Instructor|[Instructor'sname]|
|AcademicYear| 2026 – 2027 |
```
```
##PortfolioContents
```
```
1 .[Week 7 – PseudocodeandFlowcharts](week 07 - algorithms/)
2 .Moreactivitieswillbeaddedeachweek.
```
```
##SamplePseudocode:DecimaltoBinary
```
#### ```

```
[PasteyourpseudocodefromBox 1 here]
```
```
```
##MyWorkspace
```
```
![Mylaboratorycomputer](images/my-pc.jpg)
```
#### - --

```
*Lastupdated:[dateinYYYY-MM-DDformat]*
```
### 15. Savethefile.Click File → Saveas .Goto Documents → cc 101 - portfolio .Type README.md

```
asthe Filename ,set Saveastype to Allfiles ,makesure Encoding is UTF- 8 ,andclick Save.
```
### 16. Verifythefile.InFileExplorer,openthecc 101 - portfoliofolderandconfirmthefileis

```
named README.md ,notREADME.md.txt.Ifitendsin.txt,right-clickit,choose Rename ,and
remove.txt.Thenpressthe Windowskey ,type cmd ,press Enter ,andrunthecommands
below.Recordtheresultsin Table 5.
```
```
cd%USERPROFILE%\Documents\cc 101 - portfolio
dir
typeREADME.md
Tip:If“Thesystemcannotfindthepathspecified”appears,yourDocumentsfoldermaybe
insideOneDrive.Try cd%USERPROFILE%\OneDrive\Documents\cc 101 - portfolio instead.
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
### 17. Optionalpreview:ifyourNotepadhasaformattedview,switchtoitfromthe View menu

```
andnoteinTable 5 whichelementsappearformatted.Someelements,suchastables,
images,andcodeblocks,maystillappearasplaintext.GitHubwilldisplaythemcorrectly.
```
### 18. Copythewhole cc 101 - portfolio foldertoyourUSBflashdrive.

**_PartF–PeerReview_**

### 19. Exchangeseatswithaclassmate.OpentheirREADME.mdinNotepadandcompletethe

```
checklistin Table 6 fortheirfile.Writeyournameasthereviewerandreturntheworksheet.
Fixanymissingelementinyourownfilebeforeleaving.
```
**_PartG–Take-Home:UploadtoGitHub_**

DothispartwhenyouhaveInternetaccess(athome,oncampusWi-Fi,oronyourphone's
browserindesktopmode).

### 20. Goto github.com andclick Signup .Useanemailyoucheckregularlyandchoosea

```
professionalusername,suchasyourname.Verifyyouremailaddress.
```
### 21. Clickthe + buttonattheupperrightandchoose Newrepository .Type cc 101 - portfolio as

```
the Repositoryname ,choose Public ,andleave AddaREADMEfile unchecked.Click
Createrepository.
```
### 22. Onthesetuppage,clickthelink uploadinganexistingfile .DragyourREADME.md(and

```
yourweek 07 - algorithmsfolder,ifithasfiles)ontothepage.
```
### 23. Under Commitchanges ,type AddinitialREADME asthemessageandclick Commit

```
changes.
```
### 24. Openyourrepository'smainpageandcheckthattheREADMEappearsformatted.

```
CopytherepositoryURL(forexample,https://github.com/username/cc 101 - portfolio),
recorditin Table 7 ,andsubmititthroughtheLMS.
Note:GitHubdoesnotstoreemptyfolders.Thelinktoweek 07 - algorithmswillworkafterthat
foldercontainsatleastonefile,andtheimagewillappearafteryouuploadimages/my-
pc.jpg.
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
## V. DataandFindings

**_Table 1 .ProblemAnalysisforProblem 1 (PartA)_**

**Item YourAnswer**

Restatedproblem(your
ownwords)

### Write a program that inputs a non-negative decimal

### number,applies thedivide-by- 2 and remaindermethod,

### andoutputsthebinarystring.

Input decimalNum-Integer,>= 0 ,base 10

Output binaryStr-String,base 2 ( 0 sand 1 sonly)

Processes(operations)

```
InputdecimalNum
CheckifdecimalNum== 0 thenbinaryStr=" 0 "
WhiledecimalNum> 0 :
a.remainder=decimalNumMOD 2
b.binaryStr=remainder+binaryStr
c.decimalNum=decimalNumDIV 2
```
Loopcondition(whenthe
loopstops)

```
WhiledecimalNum> 0
StopswhendecimalNum= 0
```
Variablesneeded decimalNum(Integer),remainder(Integer),binaryStr(String)

13 and 25 inbinary
(computedbyhand)

#### 13 = 1101

#### 25 = 11001

**_Box 1 .PseudocodeforProblem 1 (PartB)_**

### START

### DISPLAY"Enteradecimalnumber( 0 orgreater):"

### INPUTdecimalNum

### SETbinaryStr=""

### SETtempNum=decimalNum

### IFtempNum== 0 THEN

### SETbinaryStr=" 0 "

### ELSE

### WHILEtempNum> 0 DO

### SETremainder=tempNumMOD 2

### SETbinaryStr=remainder+binaryStr

### SETtempNum=tempNumDIV 2

### ENDWHILE

### ENDIF

### DISPLAY"Decimal:",decimalNum

### DISPLAY"Binary:",binaryStr

### END


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
**_Figure 1 .FlowchartforProblem 1 (PartC)_**

**_Table 2 .TraceofProblem 1 withInput 13 (PartC)_**

**Pass n(before)**

```
nOD 2
(remainder)
nDIV 2 (newn) binary(sofar)
```
#### 1 13 1 6 1

#### 2 6 0 3 01

#### 3 3 1 1 101

#### 4 1 1 0 1101

5 0 - - Loopstops

Valuedisplayedattheend: **1101**


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
**_Table 3 .TestCasesforProblem 1 (PartC)_**

**Case DecimalInput Binary(byhand)
BinaryFromYour
Pseudocode**

```
Match?
(Y/N)
```
#### 1 0

### 0 - Specialcase,if

### n= 0 binaryis 0

#### 0 Y

#### 2 5

```
101 - 5 / 2 = 2 r 1 , 2 / 2 = 1 r 0 ,
1 / 2 = 0 r 1
```
#### 101 Y

#### 3 13

```
1101 - 13 / 2 = 6 r 1 , 6 / 2 = 3
r 0 , 3 / 2 = 1 r 1 , 1 / 2 = 0 r 1
```
#### 1101 Y

#### 4 25

```
11001 - 25 / 2 = 12 r 1 ,
12 / 2 = 6 r 0 , 6 / 2 = 3 r 0 ,
3 / 2 = 1 be 1 , 1 / 2 = 0 r 1
```
#### 11001 Y

#### 5 255

#### 11111111 -

#### 128 + 64 + 32 + 16 + 8 + 4 + 2 + 1

```
= 255 ,allremainder 1
```
#### 11111111 Y

**_Box 2 .PseudocodeforProblem 2 (PartD)_**

### START

### DISPLAY"Enterbinarynumber:"

### INPUTbinaryStr

### SETdecimalVal= 0

### SETplaceValue= 1

### SETindex=LENGTH(binaryStr)- 1

### WHILEindex>= 0 DO

### SETdigit=TO_INT(binaryStr[index])

### IFdigit== 1 THEN

### SETdecimalVal=decimalVal+placeValue

### ENDIF

### SETplaceValue=placeValue* 2

### SETindex=index- 1

### ENDWHILE

### DISPLAY"Decimalvalueis:",decimalVal

### END


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
**_Figure 2 .FlowchartforProblem 2 (PartD)_**

**_Table 4 .TestCasesforProblem 2 (PartD)_**

**Case BinaryInput Decimal(byhand)
DecimalFromYour
Pseudocode**

```
Match?
(Y/N)
```
#### 1 1101

#### 13 -

```
( 1 x 1 )+( 0 x 2 )+( 1 x 4 )+( 1 x 8 )=
1 + 0 + 4 + 8
```
#### 13 Y

#### 2 101010

#### 42 -

```
0 x 1 + 1 x 2 + 0 x 4 + 1 x 8 + 0 x 16 +
1 x 32 = 2 + 8 + 32
```
#### 42 Y

#### 3 11111111

#### 255 -

#### 1 + 2 + 4 + 8 + 16 + 3 + 2 + 64 + 12

#### 8

#### 255 Y

4 10000000 128 - 1 x 128 128 Y


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
**_BonusBox.ExtendedPseudocode:DecimaltoBase 2 , 8 ,or 16 (Optional)_**

### STARTConvertToBase

### DISPLAY"Enterdecimalnumber:"

### INPUTdecimalNum

### DISPLAY"Entertargetbase( 2 , 8 , 16 ):"

### INPUTbase

### SETresult=""

### WHILEdecimalNum> 0 DO

### SETremainder=decimalNumMODbase

### IFbase== 16 ANDremainder>= 10 THEN

### IFremainder== 10 THENSETresult="A"+result

### IFremainder== 11 THENSETresult="B"+result

### IFremainder== 12 THENSETresult="C"+result

### IFremainder== 13 THENSETresult="D"+result

### IFremainder== 14 THENSETresult="E"+result

### IFremainder== 15 THENSETresult="F"+result

### ELSE

### SETresult=remainder+result

### ENDIF

### SETdecimalNum=decimalNumDIVbase

### ENDWHILE

### DISPLAY"Convertedvalue:",result

### ENDConvertToBase

**_Table 5 .README.mdFileCheck(PartE)_**

**Item YourFindings**

Fullfolderpathofcc 101 - portfolio cdDocuments\cc 101 - portfolio

FilenameshowninFileExplorer README.md

TypeshowninFileExplorer(Details
view)
MarkdownSourceFile

SizeofREADME.mdshownbydir
(bytes)
1420 bytes

DoestypeREADME.mdshowyour
Markdowntext?(Y/N)

#### YES

Notepadformattedview
available?(Y/N)

#### YES

Elementsthatappeared
formattedinNotepad(if
available)

```
Headings,bold,Italic,bulletedlist,numberedlist,table,
link, image,code block, horizontal,rule all appeared
formatted
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
**_Table 6 .PeerReviewChecklist(PartF)_**

Reviewer'sname: **ANGELAMAEE.ESPEDILLON** OwneroftheREADME: **KYLIEESTONANTO**

**Element MarkdownUsed
PresentandCorrect?
(Y/N)**

Level- 1 heading **#** Y

Level- 2 headings **##** Y

Paragraph Textwithablanklinebeforeandafter Y

Boldanditalictext ****bold** *italic*** Y

Bulletedlist **- item** Y

Numberedlist **1 .item** Y

Table **|---|** headerseparator Y

Link **[text](url)** Y

Image **![alt](path)** Y

Codeblock
Linesbetweentwolinesofthree
backticks

#### Y

Horizontalrule **- --** Y

Filesavedas
README.md(not.txt)

#### — Y


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
**_Table 7 .GitHubSubmission(PartG,Take-Home)_**

**Item YourAnswer**

GitHubusername angelaespedillon

RepositoryURL https://github.com/angelaespedillon/cc 101 - portfolio

Dateuploaded(YYYY-MM-DD) 2026 = 10 - 18

DoestheREADMEdisplay
formattedonGitHub?(Y/N)

#### Y

Elementsthatdidnotdisplayas
expected,andwhy

```
None, All elements displayed. The link to week 07 -
algorithmswillnotworkyetbecausethefolderisempty,
which is expected per the note in step 24. Image
displayedcorrectlyafteruploadingimages/my-pc.jpg
```
## VI. Realization(Reflection)

_Intwotofoursentenceseach,answerthefollowinginyourownwords._

**1 .Whichwaseasierforyoutocreate,thepseudocodeortheflowchart?Why?**

### Pseudocodewaseasierformetocreatethantheflowchart.Icanwriteitlikestep-

### by-stepinstructionsinEnglish,soitfeelsmorenatural.FlowchartwasharderbecauseI

### neededtorememberthecorrectshapesandmakesurethearrowswereconnected

### properly.

**2 .Didtracingandtestingrevealanyerrorsinyourpseudocodeorflowcharts?Describewhat
youfoundandhowyoucorrectedit.**

### Yes,whenItracedmyworkIfoundasmallerrorinmycondition.Iforgottoinclude

### the elsepart, sothe programwouldstopincorrectly.Icorrecteditbyaddingthe

### missingstepandtestingitagainwithsampledatauntilitworked.

**3 .HowiswritingaREADMEinMarkdowndifferentfromtypingadocumentinMicrosoftWord?**

### WritinginMarkdownisdifferentbecauseyouusecodeslike#and**toformat,not

### buttons.InWordyoujustclickBoldorchangefontsizedirectlyandyouseeitright

### away.InMarkdownyouhavetotypethesymbolsandyouonlyseethefinalformat

### afteruploadingittoGitHub.

**4 .HowcanaGitHubportfoliohelpyouasafuturecomputingprofessional?**

### AGitHubportfoliocanhelpme showmyprojectsandskillstofutureemployers.It

### servesasproofofwhatIhavelearnedandbuiltduringmystudies.Italsohelpsme

### practice version control and collaboration which are important for a computer

### sciencecareer.


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
## VII. ScoringGuide

**Criteria Description Points**

**ProblemAnalysis&
Pseudocode**

```
Table 1 iscomplete;thepseudocodeforboth
conversionsiscorrect(correctuseofMOD,DIV,
andtheloop),usesproperkeywords,andis
indented.
```
#### 25

**Flowcharts&Testing**

```
Bothflowchartsusethecorrectsymbolswith
labeleddecisionsandaclearloop;thetrace
(Table 2 )andtestcases(Tables 3 and 4 )are
correct.
```
#### 25

**README.md**

```
ThefileissavedcorrectlyasREADME.md,uses
allrequiredMarkdownelements,andpasses
thepeerreviewinTable 6.
```
#### 25

**GitHubUpload**

```
TheREADMEisuploadedtoapubliccc 101 -
portfoliorepositoryandtheURLissubmitted
(Table 7 ).
```
#### 10

**Realization/Reflection**
Answersarethoughtful,specifictothestudent's
ownwork,andwellwritten.

#### 10

**Neatness&Timeliness**
Worksheetislegible/well-formattedand
submittedontime.

#### 5

**Total 100**


