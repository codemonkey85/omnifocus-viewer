# Alpha version (0.1) now available for download and testing #

**Version 0.1 (alpha stage) is now ready for download and testing.**

Once you download the zip file, import it in your Eclipse workspace, and then perform the following steps.

1. Identify the location of your OmniFocus SQLlite database on your mac. The default location is at /Users/username/Library/Caches/com.omnigroup.OmniFocus/

(replace username with your user ID).

Make sure that the file OmniFocusDatabase2 is there.


2. You have to create an account in a free ftp server to act as the intermediary between your Mac and the Android OmniFocus viewer application. I use the following free server:

_www.freehostia.com_

After you register and log in, create an ftp account with a default path (I use /www).


3. Test your ftp account:
cd /Users/username/Library/Caches/com.omnigroup.OmniFocus/
ftp -u [ftp://freehostiaid:password@ftp.freehostia.com/omni/](ftp://freehostiaid:password@ftp.freehostia.com/omni/) OmniFocusDatabase2

Replace "freehostiaid" with the user ID you used to register at free hostia, and "password" with your password.

4. If everything works fine, now you can look into the program's code. in the MainActivity.java file, edit lines 63 and 64 with your ftp ID and password.
> String user = "freehostiaid";
> String password="password";

5. That's it! Run the program, click the "Refresh button", and then click the "Show folders" button. You can click on any folder to see the projects in that folder, and click on any project to see the tasks in that project.



From here on it's up to you, at least for now. Feel free to modify the code or the GUI and share.