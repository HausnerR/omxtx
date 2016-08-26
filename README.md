omxtx
=====

This is a simple proof-of-concept OpenMAX transcoder for the Raspberry Pi.

See the warnings in the comments at the top of omxtx.c

Little fixes was applied for valid compilation.
Compiled successfully on Raspberry Pi 2 with Ubuntu 15.10 and ffmpeg 2.7.3


Copyright
=========

omxtx - OpenMAX transcoder for the Raspberry Pi
Copyright (C) 2012, 2013 Dickon Hood <dickon@fluff.org>

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License along
with this program; if not, write to the Free Software Foundation, Inc.,
51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.


example
=======
trancoding h264 > h264 lower bitrate, stream url must end with .flv

./omxtx -b 512000 -r 640x360 rtmp://hostname/live/livefull.flv rtmp://hostname/feed/live512k.flv
