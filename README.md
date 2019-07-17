# Steps
## Step 1: LCD driver installations and set up

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

## Step 2: Installation of Mac OS

###### Download the files **place them in the Downloads folder of the raspberry** :

###### To install the Mac OS , type the various code unto the terminal :

mkdir mac
cp ~/Downloads/mac.7z ./mac
cp ~/Downloads/9779D2C4\ -\ Macintosh\ II.7z ./mac

###### To check for the components in the mac folder:

cd mac
Ls

###### To unzip the packages:

sudo apt-get install p7zip
p7zip -d mac.7z
p7zip -d 9779D2C4\ -\ Macintosh\ II.7z

###### To create necessary files

mv 9779D2C4\ -\ Macintosh\ II.rom MacII.ROM
sh ./mkmacdisk.sh ( disk name:mac , size = 200 )
chmod +x minivmac

###### To run the file:

./minivmac

###### Installation of the Mac OS

In the mac folder ,Go to sys 7 folder, throw the install 1 image file into the emulator 
Ctrl + h + s + a
In the mac folder , Drag mac.dsk to the emulator, click install
Follow various image dropping – quit – restart

###### To update the version of the mac OS 7.53

Move mac.dsk file into the emulator then install.dsk file to the emulator
Go to folder 7.53, go to 1 of 19, agree 
Go to installer, press continue, change easy install to custom install
Select everything and under system software select only the top and hit install then restart

###### To update the version of the mac OS 7.55

Throw the mac.dsk file into the emulator
Add install.dsk to the emulator
Go to 7.55 folder, Click update 1 of 3 file then continue the save
Do the same step for update 2 of 3 and update 3 of 3
Open disk copy folder , open disk copy   
Add all three update files into the disk copy file
In the system update 7.5.5 update-1 folder , go to installer , click agree , click install then restart

###### to run the mac without adding the dsk file 

./minivmac mac.dsk 

###### To copy files from the Raspbian OS to the Mac OS 

Drag the importfI.dsk file to the emulator
Open the importFI folder 
Open the importFI file 
Drag whatever file u want to copy from the Raspbian to the mac os

## Step 3: Downloading the games 

https://archive.org/details/softwarelibrary_mac

Guidelines:

if the game is an img file , we transfer it unto the Mac OS then run it
if the game is a dsk file , we drop it on the emulator and we will get a folder containing the game file

