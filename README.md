General:

Debug mode:
python server.py

Prod mode:
gunicorn -w 3 -k gevent server:app -b 127.0.0.1:1234

I left a configuration file if you want to use with supervisord.

Memcache version:

Generates a temporary id to pass it to the customer and you can download the file

Example url:
http://example.com/file_id/82578172d136400ca28b0ad20b2c175d

Redis version:

Generates a permanent id to pass it to the customer and you can download the file

Example url:
http://example.com/file_id/82578172d136400ca28b0ad20b2c175d

Basic version:

This application is an example to create permanent links to files that are not typically have access, and serve them through another server, for example, nginx.

Passing a relative path, create a folder with random name and a symbolic link within the file, so you have a url like this:
http://example.com/82578172d136400ca28b0ad20b2c175d/pepito.jpg

It would be advisable to have a system cron erasing the old links (I will add more later)



