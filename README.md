
please see https://stackoverflow.com/questions/2447837/upload-1gb-files-using-chunking-in-php
for more details. This project was done in March 2010 so a lot has changed in this world since then.
It was my attempt to create a client that can send a large file in chunks to a PHP server because I could 
not find any way to stream files to a PHP server. 

The original code was in an svn repo on google code. This is for educational and archive purposes ported to github.


README of project
------------------------
gigaupload is javafx and php scripts to enable very large (giga) file upload

gigaupload project would help you to upload very large files, like 1 GB (giga bytes) file using a javafx client and a server side PHP script. PHP does not have nice support for request stream and file upload size is limited by web server and php.ini settings (typically 2MB - 8 MB)

Giga Upload allows you to overcome that limit by providing a client that can chunk big files on client side and then send these chunks one by one to PHP receiver script. One file chunk is sent as a POST to server (well within the POST_MAX limits) PHP receiver script will then assemble these chunks and create the original file on server.

This project is aimed at developers and released under a very liberal license.
