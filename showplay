#!/bin/bash

player="$(playerctl -a -f '{{playerName}} {{status}}' status | grep Playing | head -n1 | cut -d ' ' -f1)"

if [[ "$player" ]];
then
	title="$(playerctl -p $player metadata title)"
	if [ "$(playerctl -p $player metadata | grep artist)" ];
	then
		artist="$(playerctl -p $player metadata artist)"
		text="${title} - ${artist}"
	else
		text="${title}"
	fi
else
	text="No Media Playing"
fi

echo "$text"
