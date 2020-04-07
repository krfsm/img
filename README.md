# What Is This Thing?

A pair of scripts I wrote to wrangle images I want to host.

You'll need to
* create a directory called `tmp` in your home directory
* change two lines in `img.sh.sample` and `local-img.sh.sample`:
  * Setting the SERVERPATH="/var/www/html/LOCALDIRECTORY/"
  * And BASEURL="https://host.example/" variables

SERVERPATH is for the script to know where your image host stores its files. BASEURL is the base URL shown when the script is done.

(Oh, and you need to have a server to host the images from.)
