# Install Rails on Windows

Note: Even if you are using a 64bit version of Windows, it is advised to use the 32bit versions of the Devkit & Ruby as they are more stable.

Note: RailsFTW hasn't updated to the latest version of ruby so we have to do a bit of manual work to get it up to date. *This avoid certificate errors you might find on a windows machine.*

01. Go to the RailsFTW download page. [http://railsftw.bryanbibat.net/](http://railsftw.bryanbibat.net/)

  Click on the Download button, download and install the package.

02. Under "Other Useful Downloads", download the latest zipped version of Ruby (2.3.1 32 bit version) and extract contents. Copy and replace the files/folders in the *C:/RailsFTWxxx* folder. It will copy over the older version.
[Other Useful Downloads](http://rubyinstaller.org/downloads)

03. Download the **Devkit** for use with Ruby 2.0 and above (32bits version only - even if you have a 64bit computer): [http://rubyinstaller.org/downloads](http://rubyinstaller.org/downloads).

  Currently: `DevKit-mingw64-32-4.7.2-20130224-1151-sfx.exe`

04. Once RailsFTW is installed, you will have a program called "Start Command Prompt with Ruby".

  Open this and type `ruby -v` to see that your Ruby has been installed correctly.
  Also type `rails -v` to see that Rails has been installed.

05. Download and run DevKit . It is a zip file and will ask where you want to extract the files. **Choose the RailsFTW folder which will be directly on your C: drive**.

06. When the files are extracted, open up a command prompt window. (Start menu, type `cmd` and hit enter)

07. Navigate the to where the RailsFTW directory was installed. Usually something like:
    ```
    cd C:\RailsFTWxxx
    ```

08. Run the following commands. More information here: [https://github.com/oneclick/rubyinstaller/wiki/Development-Kit](https://github.com/oneclick/rubyinstaller/wiki/Development-Kit)
    ```
    ruby dk.rb init
    ruby dk.rb install
    ```

09. Download the latest Node.js from the website: [https://nodejs.org/](https://nodejs.org/) and install as normal.

    Then restart your command prompt windows. You will know that it is installed if you type in `npm -v` and see a version number as the response.

10. To install Rails 5.0 type the command `gem install rails`

11. You should now be able to create Rails apps! Congratulations!!

12. Also download and install [Git](https://git-scm.com/)
