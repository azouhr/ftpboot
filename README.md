# ftpboot
Enable z/VM to directly boot from a ftp server

This originally was a hack to simplify testing of lots of SLES builds. Now, it is a even simplified hack that has all special settings removed that I need here. 
Since we now have openSUSE Tumbleweed available at http://download.opensuse.org/ports/zsystems/tumbleweed/repo/oss/, this script might be helpful for others as well. Before you can use this, you will have to add IOS3270 to your system as found at http://www.vm.ibm.com/download/packages/descript.cgi?IOS3270.

When running this program, it displays a number of ftp servers that provide openSUSE Tumbleweed for s390x. To boot, proceed as follows:
1. put the cursor into the line with the server you want to use and press enter
2. The script will download all needed files on a ramdisk
3. An xedit window will be displayed with the current parmfile. You can either edit the parameters there or just press F3 to continue.
4. The installation routine will be started.
