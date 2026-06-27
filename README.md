# mmdvm-hotspot-docker
- Set of build files and docker-compose.yaml to create MMDVM Brandmeister network hotspot on docker server
- MMDVM set to simplex mode, frequency 434.500 MHz
- 
# configuration

Please see config/MMDVM.ini and config/DMRGateway.ini

Fill in your callsign, DMR ID, DMR ID with hotspot prefix (9 digits), Brandmeister password

Assumption is, the MMDVM modem would be connected to /dev/ttyACM0

# deployment

- build the packages using **docker compose build**
- start with **docker compose up -d**
- check logs of mmdvmhost, dmrgateway and moquitto for any errors
- ENJOY :)
