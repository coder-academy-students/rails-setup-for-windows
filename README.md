# Install Rails on Windows

Note: Even if you are using a 64bit version of Windows, it is advised to use the 32bit versions of the Devkit & Ruby as they are more stable.

Note: RailsFTW hasn't updated to the latest version of ruby so we have to do a bit of manual work to get it up to date. *This avoid certificate errors you might find on a windows machine.*

01. Go to the RailsFTW download page. [http://railsftw.bryanbibat.net/](http://railsftw.bryanbibat.net/)

  Click on the Download button, download and install the package.

02. Under "Other Useful Downloads", download the latest zipped version of Ruby (2.3.1 32 bit version) and extract contents. Copy and replace the files/folders in the *C:/RailsFTWxxx* folder. It will copy over the older version.
[Other Useful Downloads](http://rubyinstaller.org/downloads)

03. The gems in Ruby certificates need to be updated. Download ruby-gemsupdate-2.6.7 and save the file to your C:/ directory. It may as permission, say continue/ok.
[gemsupdate-2.6.7](https://rubygems.org/downloads/rubygems-update-2.6.7.gem)

04. Open the program Powershell and type:
`gem install --local C:\rubygems-update-2.6.7.gem`
`update_rubygems --no-ri --no-rdoc`

05. You can uninstall rubygems-update by typing in Powershell:
`gem uninstall rubygems-update -x`

06. Download the **Devkit** for use with Ruby 2.0 and above (32bits version only - even if you have a 64bit computer): [http://rubyinstaller.org/downloads](http://rubyinstaller.org/downloads).

  Currently: `DevKit-mingw64-32-4.7.2-20130224-1151-sfx.exe`

07. In Powershell type `ruby -v` to see that your Ruby has been installed correctly.

08. Download and run DevKit . It is a zip file and will ask where you want to extract the files. **Choose the RailsFTW folder which will be directly on your C: drive**.

09. When the files are extracted, open up a command prompt window. (Start menu, type `cmd` and hit enter)

10. Navigate the to where the RailsFTW directory was installed. Usually something like (Note: the xxx is your RailsFTW version number):
    ```
    cd C:\RailsFTWxxx
    ```


11. Run the following commands. More information here: [https://github.com/oneclick/rubyinstaller/wiki/Development-Kit](https://github.com/oneclick/rubyinstaller/wiki/Development-Kit)
    ```
    ruby dk.rb init
    ruby dk.rb install
    ```

12. Download the latest Node.js from the website: [https://nodejs.org/](https://nodejs.org/) and install as normal.

    Then restart your command prompt windows. You will know that it is installed if you type in `npm -v` and see a version number as the response.

13. To install Rails 5.0 type the command `gem install rails`

14. Also type `rails -v` to see that Rails has been installed.


15. You should now be able to create Rails apps! Congratulations!!

16. Also download and install [Git](https://git-scm.com/)
