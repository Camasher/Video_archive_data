# Video_archive_data
Tracking recorded 1FPS volcano imagery data

|Field Name   |Description   |Example   |
|---|---|---|
|volcano   |Name of the volcano that the imagery is of. Lowercase.   |ruapehu, tongariro, whiteisland, raoul   |
|camera code   |code name of the camera from the GeoNet Delta "cameras.csv". Uppercase.   |WINR   |
|camera name   |site name of the camera from the Geonet Delta "cameras.csv". Lowercase, one word.  |whiteislandnorthrim   |
|start date/time   |In UTC, format as YYYY-MM-DDTHH:MM:SSZ   |2021-12-25T03:12:00Z   |
|end data/time   |In UTC, format as YYYY-MM-DDTHH:MM:SSZ   |2021-12-25T03:15:00Z   |
|framerate   |In Frames per Second   |1FPS   |
|resolution   |quality of the video. In cases where two lenses are used, it will display the format of one of the lenses   |VGA 640x480   |
|filetype   |captured for non raw .mxg files   |mxg, mp4, tar|
|lens   |To captured what type of lens the image was captured   |day, night, thermal    |
|notes   |any special details about the video clip. Seperated by vertical line   |TAR format, multiple lenses, confidential, thermal   |
|keywords   |For specific search words to help narrow down focus media. Seperated by vertical line "|"   |eruption, ash, plume, glow    |

List of Camera Codes:
| Code | Site Name |
|---|---|
| XXXX  | this refers to a temporary site and will be named accordingly  |
| DISC  | Discovery Lodge   |
| KAKA  | Kakaramea  |
| KMTP  | Tai Ping  |
| MTSR  | Mangateitei  |
| RIMK  | Raoul Island Mount Moumoukai  |
| TEMO  | Taranaki Emergency Management Office  |
| TOKR  | Karewarewa  |
| WHOH  | Whakatane Hub  |
| WICF  | White Island Factory  |
| WINR  | White Island North Rim  |
| WIWR  | White Island West Rim  |

### File Naming Convention:

"netcam-[camera name]_YYYYMMDDTHHMM-HHMM"

- For thermal imagery add "_thermal"
- For confidential videos such as White Island eruption videos, which are provided on a case-by-case basis, add "_CONFIDENTIAL"
- For videos which have been sped up, add "_8x" or "_64x" depending on how sped up the video is. It is preffered that the raw .mxg video is archived, but if the .mxg no longer exists, and only a sped up .mp4 exists, then this is acceptable.

If the video spans multiple days, the YYYYMMDD is the date at which the video starts

### Locations to Check

- [X] J Drive
- [X] VolcDB
- [X] Slack - Volcanology
- [X] Slack - Duty
- [ ] Teams - Volcanology
- [ ] NGMC J Drive - mostly .mp4 and/or sped up
- [ ] CA Laptop
- [X] CA Old Laptop
- [ ] CA PC
- [ ] RJ Laptop
- [ ] RJ PC
- [ ] VML

### ToDo at a later date:

~~add field **TAGS** or **KEYWORDS**: a field to catpure important information about a specific video. Does it contain an eruption? nightglow?~~

~~add field **LENS**: is the view a night or day lens shot? or is it thermal?~~

~~add field **FORMAT**: generally formats are in .mxg, but .tar and .mp4 also exist. A .mp4 file implies that the .mxg version no longer exists.~~

add field that auto-generates file name with hyperlink

Remove FPS from FPS field entries as it is redundant. No need to say "FPS: 1FPS" when you could just say "FPS: 1"

~~Remove VGA or QXGA from resolution as they are redundant, just leave the field as 640x480. Some thought needs to go in to DUAL LENSES files, as in most cases that are two 640x480 videos merged side-by-side and are therefore 1280x480 resolution~~
