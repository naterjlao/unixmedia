# Unix Media Utility
Media Utility Tool for Unix Systems

This package can be used to process media from removable media and store contents in specified locations.

## Usage:
The target must first be mounted in filesystem:

`sudo mount /dev/sdb1 /mnt`

Find all media files and copy them over to the default backup directory (as specified in the configuration file):

`medutil backup /mnt`

Search through the target and copy only jpegs, mp3s and pngs. Override user configuration and store in specified directory:

`medutil backup /mnt --type jpg mp3 png --out /home/user/backup`

## Use Cases:
* Video and Photos from cameras
* Audio from recording devices
* Flash drives for media distribution

## Target Features:
* Debian/Ubuntu support
* Process a target directory for backup on process call
* User configurable target rules for different file types

## Future Features:
* Redhat/Fedora support
* Duplicate file management
* Backup processing for redundacy locations
* Support for 3rd party backup services (AWS, Google Drive, etc.)
