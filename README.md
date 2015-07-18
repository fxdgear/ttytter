# ttytter
Dockerized ttytter

Run TTYtter twitter client in a docker container. 

## To run:

```bash
$ docker run --rm -it -v ~/.config/ttyttr:/data fxdgear/ttyttr -ansi -dostream -ssl -readline -newline -verify -notifies=dm,me,reply
```

* Running with the `-rm` flag will destroy the container after each run, there's no data to persist. 
* Using `-it` allows us to interact with the container
* If you have a keyfile mount it to the `/data/` volume inside the container (for auth)
* pass in any other ttytter parameters you feel like

## Todo

* hookup to a notification system (libnotify, growl, etc)
