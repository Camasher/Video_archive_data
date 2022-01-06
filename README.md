# Video_archive_data
Tracking recorded 1FPS volcano imagery data

volcano - name of the volcano that the imagery is of, generally "white island", but could be any of the volcanoes such as "raoul", "ruapehu", or "tongariro". Lowercase.

camera code - code name of the camera from the GeoNet Delta cameras.csv. eg. "WINR". All uppercase.

camera name - site name of the camera from the Geonet Delta cameras.csv. eg "whiteislandnorthrim"

start date/time - In UTC, format as YYYY-MM-DDTHH:MM:SSZ eg. 2021-12-25T03:12:00Z

end data/time - In UTC, format as YYYY-MM-DDTHH:MM:SSZ eg. 2021-12-25T03:15:00Z

framerate - typically "1FPS"

resolution - typically "640x480"

notes - any special details about the video clip, which may be in TAR format, zoomed, of differing quality, or from multiple lenses simultaneously


File Naming Convention:

"netcam-[camera name]_YYYYMMDDTHHMM-HHMM"

For thermal imagery add "_thermal"
For Confidential, add "_CONFIDENTIAL"


To add at a later date:

TAGS: a field to catpure important information about a specific video. Does it contain an eruption? nightglow?

LENS: is the view a night or day lens shot? or is it thermal?

FORMAT: generally formats are in .mxg, but .tar and .mp4 also exist. A .mp4 file implies that the .mxg version no longer exists.
