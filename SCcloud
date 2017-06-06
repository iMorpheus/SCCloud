#!/bin/bash

### INPUT ###
read -p "File to be converted: " -e TSRC;


### OUTPUT DESTINATION ###
read -p "Destination Folder: " -e DEST;
mkdir $DEST;

function SCcloud(){
x=0;
CNT=$TSRC;
while IFS= read -r CNT
do
	say -v Daniel $CNT -o "./$DEST/"$x"_Of".m4a ;
	((x++));
	echo $x;
done < "$CNT"

clear;

}

trap SCcloud EXIT
