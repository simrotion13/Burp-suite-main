#Installing Burpsuite Pro in Windows

++++++++++++++++++++++++++++++++++++++
Prequisites
++++++++++++++++++++++++++++++++++++++

Download .jar file for Burp Suite Pro from**
-> https://portswigger.net/burp/releases/download?product=pro&version=2022.7.1&type=Jar

Download Burp Loader files & Follow Below Steps for Activation
-> https://github.com/simrotion13/Burp-suite-main/

If using in Windows 10, Download and Install Java and JDK

Java --> https://javadl.oracle.com/webapps/download/AutoDL?BundleId=246806_424b9da4b48848379167015dcc250d8d
JDK --> https://download.oracle.com/java/18/latest/jdk-18_windows-x64_bin.exe

++++++++++++++++
Execution and Activation
++++++++++++++++
	
1. Place all files in 1 folder in desktop. [e.g C:\Users\kali\Desktop\burp-suite\]
----------------------------------------------
2. Run This Command for Windows in CMD Prompt.
   java --illegal-access=permit -Dfile.encoding=utf-8 -javaagent:"C:\Users\kali\Desktop\burp-suite\loader.jar" -noverify -jar "C:\Users\kali\Desktop\burp-suite\burpsuite_pro_v2022.7.1.jar"
---------------------------------------------
3. Use keygen.jar to generate the License key
   java -jar keygen.jar
----------------------------------------------
4. Activate Burp Suite Pro
	1. Modify License String like "license to kali"
	2. Copy License key from keygen.jar and paste in Burp Suite Pro and click Next.
	3. Select Manual Activation Option on your bottom Right in Burp Suite Pro.
	4. Copy License Request from BurpSuite_Pro and paste in keygen.jar
	5. Copy license response from keygen.jar and paste in BurpSuite_Pro, and next and Done
----------------------------------------------
5. For Windows Follow These Steps
	1. Open Notepad and Paste command at 2 and save the file with name burp.bat in "C:\Users\kali\Desktop\burp-suite\" Folder.
	2. Open another Notepad and Paste below command and save it with burp.VBS extension in Desktop.
		Set WshShell = CreateObject("WScript.Shell")
		WshShell.Run chr(34) & "C:\Users\kali\Desktop\burp-suite\burp.bat" & Chr(34), 0
		Set WshShell = Nothing
----------------------------------------------
6 For Executing Burp in Windows, Double Click on burp.VBS file.
