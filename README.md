# Simple-File-Server

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/a2b646100fc84cf2901f3ae86dcbdc1d)](https://www.codacy.com/app/RDCH106/Simple-File-Server?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=RDCH106/Simple-File-Server&amp;utm_campaign=Badge_Grade)

Simple Python File Server with browser upload and authentication.

Simple tool that gave secure remote file control with no client-side installation.

### What is this?
This is a simple file server that
* supports file directory browse of the server
* supports file upload to the server
* supports authentication
* marks frequently visited directories for easier navigation

Find the latest version at https://github.com/RDCH106/Simple-File-Server

### How To Run

Configure the `setting.py` file with the desired configuration and run as other python program:

`python simple_file_server.py`

To run the server in background redirecting the log `tmp` symtem folder:

`python simple_file_server.py > /tmp/simple_file_server.log 2>&1 &` (**only in GNU/Linux**)

### How To Install
Read and edit settings.py.

`sudo ./install`

Once the script is completed, this file server should be registered as an upstart service.

Check the file server at http://host:port/base_url

###How To Uninstall
`sudo ./uninstall`

###Credit
This is a fork of https://github.com/wonjohnchoi/Simple-Python-File-Server-With-Browse-Upload-and-Authentication written by [wonjohnchoi](https://github.com/wonjohnchoi) (who also forked of http://li2z.cn/?s=SimpleHTTPServerWithUpload  written by bones7456 who also was forked from http://www.opensource.apple.com/source/python/python-3/python/Lib/SimpleHTTPServer.py)

This fork basically adds install scripts, authentication, and some more on top of the original code that supports directory browse and file upload.
