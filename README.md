# multiroom_audio
multi room/device audio using mopidy and snapserver. works well with android snapcast client. 
on macos docker, the audio sometimes stutters though.

build the images using docker files and properly tag them
cd into multiroom audio directory
docker-compose up

for connecting to snapserver:
1. use snapcast app on android, works better than web browser
2. http://localhost:1780/ use on any web browser (doesnt work on ios)

for playing local songs via iris(mopidy):
1. mount music directory properly for mopidy image in docker compose 
2. navigate to http://127.0.0.1:6680/ 

source of these dockerfiles:
https://github.com/IVData/dockerfiles/tree/master/mopidy-multiroom

made changes to mopidy dockerfile and sh and config as what i got from the repo directly weren't working.
