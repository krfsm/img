# What Is This Thing?

A pair of scripts I wrote to wrangle images I want to host.

# Usage

* `img.sh`, optionally followed by the URL you want to fetch and local file name you want to use.
* `local-img.sh`, optionally followed by the file name you want to import and what you want to rename it to.

# What Does It Do?

It downloads the image file, rotates it so that it is oriented correctly (if this is set), strips EXIF data, rescales it so the maximum dimension is 1024 pixels (the test files are from when it was 800), moves it to a directory tree named for year/month/day you fetched/imported the file, and shows you the URL it's now hosted on.

# Know This!

You'll need to:
* create a directory called `tmp` in your home directory
* change two lines in `img.sh.sample` and `local-img.sh.sample` that set these two variables:
  * `SERVERPATH="/var/www/html/LOCALDIRECTORY/"`
  * `BASEURL="https://host.example/"`
* rename `img.sh.sample` to `img.sh` and `local-img.sh.sample` to `local-img.sh` (and make sure they're executable)

`SERVERPATH` is for the script to know where your image host stores its files. `BASEURL` is the base part of the URL shown when the script is done.

(Oh, and you need to have a server to run this on and host the images from.)
