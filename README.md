# Video_archive_data
Tracking recorded 1FPS volcano imagery data

|Field Name   |Description   |Example   |
|---|---|---|
|volcano   |Name of the volcano that the imagery is of. Lowercase.   |ruapehu, tongariro, whiteisland, raoul   |
|camera code   |code name of the camera from the GeoNet Delta "cameras.csv". Uppercase.   |WINR   |
|camera name   |site name of the camera from the Geonet Delta "cameras.csv".   |whiteislandnorthrim   |
|start date/time   |In UTC, format as YYYY-MM-DDTHH:MM:SSZ   |2021-12-25T03:12:00Z   |
|end data/time   |In UTC, format as YYYY-MM-DDTHH:MM:SSZ   |2021-12-25T03:15:00Z   |
|framerate   |In Frames per Second   |1FPS   |
|resolution   |quality of the video. In cases where two lenses are used, it will display the format of one of the lenses   |VGA 640x480   |
|notes   |any special details about the video clip. Seperated by vertical line   |TAR format, multiple lenses, confidential, thermal   |

#### volcano
Name of the volcano that the imagery is of, generally "white island", but could be any of the volcanoes such as "raoul", "ruapehu", or "tongariro". Lowercase.

#### camera code
code name of the camera from the GeoNet Delta cameras.csv. eg. "WINR". All uppercase.

#### camera name
site name of the camera from the Geonet Delta cameras.csv. eg "whiteislandnorthrim"

#### start date/time
In UTC, format as YYYY-MM-DDTHH:MM:SSZ eg. 2021-12-25T03:12:00Z

#### end data/time
In UTC, format as YYYY-MM-DDTHH:MM:SSZ eg. 2021-12-25T03:15:00Z

#### framerate
typically "1FPS"

#### resolution
typically "VGA 640x480"

#### notes
any special details about the video clip, which may be in TAR format, zoomed, of differing quality, or from multiple lenses simultaneously

### File Naming Convention:

"netcam-[camera name]_YYYYMMDDTHHMM-HHMM"

For thermal imagery add "_thermal"
For Confidential, add "_CONFIDENTIAL"

### ToDo at a later date:

add field **TAGS** or **KEYWORDS**: a field to catpure important information about a specific video. Does it contain an eruption? nightglow?

add field **LENS**: is the view a night or day lens shot? or is it thermal?

add field **FORMAT**: generally formats are in .mxg, but .tar and .mp4 also exist. A .mp4 file implies that the .mxg version no longer exists.

add field that auto-generates file name with hyperlink

Remove FPS from FPS field entries as it is redundant. No need to say "FPS: 1FPS" when you could just say "FPS: 1"

Remove VGA or QXGA from resolution as they are redundant, just leave the field as 640x480. Some thought needs to go in to DUAL LENSES files, as in most cases that are two 640x480 videos merged side-by-side and are therefore 1280x480 resolution
