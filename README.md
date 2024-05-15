# AndroidStudio-Installation-Guide

第一步：準備階段

載卸載工具：UninstallTool-3.7.3.5716-All.exe
※工具已上傳倉庫，自行下載打開即用，可以卸載軟體安裝失敗產生的一些殘留文件。

官網曆史版本軟體：https://developer.android.google.cn/studio/archive#android-studio-3-0?utm_source=androiddevtools&utm_medium=website
※Google Android Studio 官網鏈接，下載的軟體更安全，更新。

JDK軟體官網：https://www.oracle.com/java/technologies/downloads/archive/
※其中JDK8幾以下版本需登錄賬戶。

第二步：安裝階段

安裝系統環境配置JDK：
JAVA_HOME    安裝JDK軟體的目標文件夾
CLASSPATH    .;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar;
Path    %JAVA_HOME%\bin;%JAVA_HOME%\jre\bin

配置AVD幾Gradle目錄：
GRADLE_USER_HOME   均為希望配置的文件夾路徑
ANDROID_SDK_HOME   均為希望配置的文件夾路徑

配置ADB：
Path    設置為下載的sdk adb路徑

一些常見的疑難雜症：
校園網幾不可抗拒的原因下導致的，通常在這種情況下，我們只需要找到對應的hosts文件，在編輯模式下加入：
203.208.50.100  dl.google.com
203.208.40.37  dl.l.google.com
保存並替換，重新打開AS即可運行。
