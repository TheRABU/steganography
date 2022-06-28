# steganography
This repository is for steganography related solves and techniques 

Tools used:
Exiftool
● Install Command:
 sudo apt-get install libimage-exiftool-perl
● Read a image meta data
● -H read hex data
● -common
● Grep GPS
● -v more data
● “-*Comment*”
● Add Comment/text
 exiftool -comment=”hello” [imageName] 
 
Steghide 
  Install Command
  sudo apt-get install steghide
  ● Download a image / select a image
  ● Create a file that you want to hide
  ● To hide a info in a image Command:
   steghide embed -cf [imageName] -ef [fileName]

  Extract information from a Image
  ● Extract Command:
  steghide extract -sf [imageName]
  ● steghide only supports a limited amount of ‘cover’ files – 
  JPEG, BMP, WAV, and AU
  
zsteg
  ● Install Command:
         gem install zsteg
   usage:
      ● Zsteg [imageName] (This works for .png images)
      
Stegseek
    ● Install:
        Download the latest 
        https://github.com/RickdeJager/stegseek
     Install the .deb file using sudo apt install 
        ./stegseek_0.6-1.deb
    ● Run Command:
      stegseek [imageName] rockyou.txt
      
Binwalk
    ● Install: https://github.com/ReFirmLabs/binwalk/blob/master/INSTALL.md
    ● Run: 
         binwalk [imageName]
    ● Extract:
         binwalk -e [imageName]
         binwalk --dd=".*" smile.png -e 
         
Xor IMAGE
     ● gmic secret.png ciphered.png -blend xor
     
     
reference : https://github.com/foysalhossain12/Steganography-_CTF 

The using methods were explained in the solving page...







