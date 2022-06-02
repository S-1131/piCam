# Notes on working with camera and raspberry pi


ip for pi - 192.168.1.17

## controlling the webcam

Use `lsusb` to list the webcam and verify connection.


Use `fswebcam` as command to control cam (man page where needed).

Use `-S 20` option to skip first 20 frames (this prevents black screen).


## Other Notes on the pi

Set up headless. Apparently raspbian doesn't create `pi` user with default
password anymore. Needed to create `userconfig.txt` file and add `User:Password`
using a hashed password.

Another note, using the instructions in [this article](https://web.archive.org/web/20200130073401/https://marcelwiget.blog/2018/12/02/tether-rpi-to-ipad-pro-via-ethernet-over-usb-c/amp/) for adding the dtoverlay to the config file overwrites the entire config file? Not sure if this was fatal but worth noting.

## Next Steps

* Investigate live video capture.
* Investigate ways to stream live video.

Alternatively:
* Create a script(likely bash or python) that will take photos or clips at particular increments and post them in some obscure place on the internet out there somewhere.

