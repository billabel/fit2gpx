#! /usr/bin/env sh

# Converts a Garmin FIT file to GPX format using gpsbabel
# Usage "fit2gpx <filename>"

filename=`basename $1 .fit`

if [ $filename != ".fit" ]; then
    gpsbabel -i garmin_fit -f "$filename".fit -o gpx -F "$filename".gpx
else
    echo "Provide a .FIT file to convert:\n fit2gpx <filename>"
fi
