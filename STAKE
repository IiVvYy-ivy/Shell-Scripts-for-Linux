#!/bin/bash

echo "Please input start port x："
read x

echo "Please input end port y："
read y

echo
echo
while [ $x -le $y ]
do
    echo "x = $x" > /dev/null
    x=$((x + 3))
    cmd="curl -XPOST localhost:$x/stake/100000000000000000"
    echo "Execute complete：$cmd" > /dev/null
    sleep 10 > /dev/null
    result=$(eval $cmd) > /dev/null

done 
echo "Stake complete"
