Zaplesszap is a docker container for zap2xml that includes everything required to run zap2xml exlucding the zap2xml.pl script.   To use this container visit the authors page: http://zap2xml.awardspace.info/ to download zap2xml.pl....

Steps to configure :
Create the following container paths:
  - /config - place zap2xml.conf and the zap2xml.pl files in this folder
  - /data  - this is where your guide.xml will be generated.

Follow the guide on the authors page for the  config file. It should look something like this :
user=<username>
pass=<password>
cache=/config/cache
days=14
outformat=xmltv
outfile=/data/guide.xml

To add parametrs that are not available via the config file you can set a container environment variable called FLAGS 
