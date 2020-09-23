<div align="center">

## Moblie Java Development Kit


</div>

### Description

This is a way to have a mobile Java development kit. It is self contained on one cd and will run even if you have no rights on the computer you are logging on to.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Robert Somers](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/robert-somers.md)
**Level**          |Beginner
**User Rating**    |3.8 (15 globes from 4 users)
**Compatibility**  |Java \(JDK 1\.1\), Java \(JDK 1\.2\)
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__2-57.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/robert-somers-moblie-java-development-kit__2-2188/archive/master.zip)





### Source Code

Items needed:
1) Java JDK or SDK<BR>
2) Textpad 4.x<BR>
3) CD Burner<BR>
4) (optional) Java documentation<BR>
Java mobile development kit:<BR>
Step 1:<BR>
Download and install your Java development kit (JDK) or SDK. You can optionally download the documentation (it is somewhat useful&#8230;). Install this on to your hard drive.<BR>
Step 2:<BR>
Download and install Textpad 4.x. It is shareware and it is probably the best text editor I have seen. I recommend registering this software based on the fact that it is second only to Visual Studio in ease of use and functionality, and it is only $25&#8230; <BR>
Step 3:<BR>
Configure Textpad. Go to Configure --> Prerences&#8230; and then click on the plus symbol for &#8216;document classes&#8217;. Click on the plus symbol next to Java. Then click on syntax. In the dropdown list select &#8216;Java.syn&#8217;. At this point, you are golden. Then click &#8216;Tools&#8217; (still in the &#8216;configure preferences&#8217; property page) and &#8216;add&#8217;. Select &#8216;jdk commands&#8217;.<BR>
Step 4:<BR>
Create a batch file. Write the following code into Textpad and save it as &#8216;autoOpen.bat&#8217;.<BR>
SET jdkRoot=%cd%<BR>
SET PATH=%path%;%jdkroot%\jdk1.3.0_02\bin<BR>
SET CLASSPATH=%jdkroot%\jdk1.3.0_02\lib;%jdkroot%\jdk1.3.0_02\jre\lib;%jdkroot%\jdk1.3.0_02\jre;%jdkroot%\jdk1.3.0_02;<BR>
SET PROMPT=%prompt%$LJavaTerm$G<BR>
start %jdkRoot%\Textpad4\textpad.exe<BR>
pause<BR>
Note:<BR>
If you are using a JDK other than 1.3 you need to specify the correct folder names in the &#8216;SET PATH&#8217; command and the &#8216;SET CLASSPATH&#8217; command&#8230;<BR>
Step 5:<BR>
Create an Autorun.inf file. Write the following code to it.<BR>
[autorun]<BR>
open=autoOpen.bat<BR>
Step 6:<BR>
Copy the JDK folder &#8216;jdk1.3.0_02&#8217; in this case and the &#8216;Textpad 4&#8217; to a common folder. (Preferably to the root of one of your hard drives.) And rename the folder &#8216;Textpad 4&#8217; to &#8216;Textpad4&#8217; (remove the space&#8230;) Then copy the &#8216;autoOpen.bat&#8217; and the &#8216;autorun.inf&#8217; to the same place. So your directory should look like this:<BR>
Jdk1.3.0_02\<BR>
Jdk1.3\ (this is the documentation folder&#8230; optional)<BR>
Textpad4\<BR>
autoOpen.bat<BR>
autorun.inf<BR>
Step 7:<BR>
Burn these files to a cd. I personally use CDRWin (it&#8217;s a geek thing&#8230;). Make sure to preserve long filenames in your cd program!!! If you cannot do this use CDRWin&#8230; Also make sure the root of your cd looks like the result of step 6!!!<BR>
Now, if the directions were followed correctly, you have a cd that will autorun textpad with the Java syntax highlighting and under tools you should see &#8216;compile java&#8217;; &#8216;run java application&#8217; and &#8216;run java applet&#8217;. It will also have a command prompt window. It is very important that you do not close this window until you are done developing. The path and classpath statements in the batch file expire when you close this window&#8230; This means that the compile and run commands will cease working&#8230; <BR>
Anyway, happy coding and have fun with this!!!<BR>
Dagaz

