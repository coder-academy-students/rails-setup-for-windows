# Install Rails on Windows

Note: Even if you are using a 64bit version of Windows, it is advised to use the 32bit versions of the Ruby Installer and Devkit as they are more stable.

01. Go to the RubyInstaller download page. [http://rubyinstaller.org/downloads/](http://rubyinstaller.org/downloads/)

  Download and install the latest version of the Ruby Installer. Currently 2.2.2

02. Download the Devkit for the 2.0 and 2.1 version of RubyInstaller.

  Currently: `DevKit-mingw64-32-4.7.2-20130224-1151-sfx.exe`

03. Once RubyInstaller is installed, you will have a program called "Start Command Prompt with Ruby".

  Open this and type `ruby -v` to see that your Ruby has been installed correctly.
  Also type `rails -v` to see that Rails has been installed.

04. Run the DevKit download. It is a zip file and will ask where you want to extract the files. Choose the Ruby folder which will be directly on your C: drive.
    
05. When the files are extracted, open up a command prompt window. (Start menu, type `cmd` and hit enter)

06. Navigate the to the DevKit directory.
    ```
    cd C:\Ruby\Devkit
    ```

07. Run the following commands. More information here: [https://github.com/oneclick/rubyinstaller/wiki/Development-Kit](https://github.com/oneclick/rubyinstaller/wiki/Development-Kit)
    ```
    ruby dk.rb init
    ruby dk.rb install
    ```

08. Install Node.js from their website: [https://nodejs.org/download/](https://nodejs.org/download/)
    
    Then restart your computer.

09. You should now be able to create Rails apps! Congratulations!!

  

You're done!