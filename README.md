
# showplay
show now playing media information


### About
![script preview](https://github.com/kaonkaon/showplay/blob/main/Preview.png?raw=true) </br>
A script to show currently playing media info. can be used on terminal or as module as you need.</br>
~~*honestly who need this*~~

## Dependencies
* playerctl
* You, yes you

## Installation
* clone the git
```
git clone https://github.com/kaonkaon/showplay
```
* enter showplay dir
```
cd showplay
```
* give it permission to run
```
chmod +x showplay
```
* move it to bin dirrectory
```
sudo cp showplay /usr/local/bin/
```
### use as Polybar Module
just add this on polybar modules.ini
```
[module/showplay]
type = custom/script
exec = /usr/local/bin/showplay
interval = 1
format = <label>
label = "%output:0:100% "
```
then add the module to your bar

## Contribute(?)
go ahead, please, don't leave me alone
