A Docker image which contains Wallop and the latest FFMPEG.

## Example Usage

`sudo docker run -d -v /$config_directory:/wallop/config -p 8888:8888 kdoyen/wallop`

You will want to replace $config_directory with a local directory which contains
the config.toml for Wallop. Ensure the [ffmpeg] section has an acodec key set to
"libfdk_aac" and the ffmpeg_path key is set to "/ffmpeg/bin/ffmpeg".

## Modified by Kristopher Doyen

Forked originally from https://github.com/ipstatic/wallop-docker and modified for building against https://github.com/kdoyen/wallop/

Original wallop author https://github.com/maddox/wallop


