# Downloading Nptel Videos

Nptel is one of my favority online study website. However sometime i need offline due to internet issues. There are multiple way to download videos.

1. Youtube playlist.

Most video can be found in youtube playlist. But most courses are unlisted so cannot be found on youtube. If we can find it in youtube we can use `youtube-dl` and the problem is solved.

2. Try Hard.

- Go to course link like this.
```
https://nptel.ac.in/courses/106/105/106105190/
```
- Go to download video tab
- Open developer console. In firefox we can go via `Cmd+Shift+I`
- After opening console type this.
```js
  Array.from(document.querySelector('#request > tbody:nth-child(2)').querySelectorAll('a')).map(v=>v.href).join('\n')
```
- You should see similar output:
```
 "https://nptel.ac.in/content/storage2/MP4/106105190/mod01lec01.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod01lec02.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod01lec03.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod01lec04.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod01lec05.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod01lec06.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod02lec07.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod02lec08.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod02lec09.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod02lec10.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod02lec11.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod03lec12.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod03lec13.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod03lec14.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod03lec15.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod03lec16.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod04lec17.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod04lec18.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod04lec19.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod04lec20.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod04lec21.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod05lec22.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod05lec23.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod05lec24.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod05lec25.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod05lec26.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod06lec27.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod06lec28.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod06lec29.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod06lec30.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod06lec31.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod07lec32.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod07lec33.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod07lec34.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod07lec35.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod07lec36.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod08lec37.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod08lec38.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod08lec39.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod08lec40.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod08lec41.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod09lec42.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod09lec43.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod09lec44.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod09lec45.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod09lec46.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod10lec47.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod10lec48.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod10lec49.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod10lec50.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod10lec51.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod11lec52.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod11lec53.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod11lec54.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod11lec55.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod11lec56.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod12lec57.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod12lec58.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod12lec59.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod12lec60.mp4
https://nptel.ac.in/content/storage2/MP4/106105190/mod12lec61.mp4"
```
- Copy everything inside double quote.
- Add it to your download manager like aria2c or internet download manager. (I used aria2c and web-aria2c)

Done!!!!
