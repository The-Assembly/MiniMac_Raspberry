## LCD driver installations and set up

###### Type the various lines of codes in the Terminal to install the LCD driver

sudo rm -rf LCD-show <br/>
git clone https://github.com/goodtft/LCD-show.git <br/>
chmod -R 755 LCD-show <br/>

###### Open terminal and type following to use LCD screen -

cd LCD-show <br/>
sudo ./LCD32-show (for the 3.2-inch LCD-TFT screen) <br/>
sudo ./LCD35-show (for the 3.5-inch LCD-TFT screen) <br/>

###### To disable LCD, type following on LCD screen in terminal –

cd LCD-show
sudo ./LCD-hdmi
