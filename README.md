# course

```
cd /var/www/html/moodle
rm -r course
git clone https://github.com/alejandrobujan/course.git
chmod -R 777 .
apt update
apt install nodejs npm
npm install -g n
sudo n stable
npm install -g grunt
cd course
grunt amd
cd ../blocks
git clone https://github.com/alejandrobujan/activity_completion.git
```
