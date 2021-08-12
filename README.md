# Custom Moodle Course Module

This is a custom version of the Course Module in Moodle 3.11, it was developed as a requirement for [Activity Completion](https://github.com/alejandrobujan/activity_completion) block. 

## Installation 

Place the contents of this source tree into your Moodle installation so that within your Moodle root, this file is course/README.md. You can follow the next steps:

```
# Placed into your Moodle root (e.g. /var/www/html/moodle)
rm -r course
git clone https://github.com/alejandrobujan/course.git
chmod -R 777 .

# Now you have to re-build your Moodle environment with Grunt
apt update
apt install -y nodejs npm
npm install -g n
n stable
PATH="$PATH"
npm install grunt-cli --save-dev
npm install -g grunt
cd course
grunt amd
```

## License

Copyright (C) 2021  Alejandro Buján Pampín

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
