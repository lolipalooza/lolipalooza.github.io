---
layout: lolnada/post
title:  Animación psicodélica
date:   2022-06-07 12:34:00 -0400
source: https://codepen.io/isladjan/pen/BaaNKqj
---
<style type="text/css">
* {
    margin: 0;
    padding: 0;
}

#wrapper {
    overflow: hidden;
    width: 100%;
    height: 100vh;
    position: relative;
    background: url(https://user-images.githubusercontent.com/26748614/112760946-182a8300-8ff9-11eb-9881-8ca96150852e.jpg) 75% 0% /140%;
    animation: bg 25s linear infinite paused;
}

.bg {
  width: 100%;
  height: 100vh;
  background: linear-gradient(to right, #EE7752, #E73C7E, #23A6D5, #23D5AB);
  background-size: 400% 100%;
  animation: bg 20s infinite;
}

@keyframes bg {
  0% {
      background-position: 0% 50%;
  }

  50% {
      background-position: 100% 50%;
  }

  100% {
      background-position: 0% 50%;
  }
}

/* === SVG === */
svg {
  display: block;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100%;
  height: 100vh;
}

svg polygon {
  position: absolute;
}

svg polygon.center {
  opacity:0.7;
  cursor: pointer;
  transition: opacity 0.3s;
}

svg polygon.center:hover {
  opacity:0.2;
}

#startText {
  font-family: 'Turret Road', cursive;
  font-weight: 700;
  fill:#fff;
  user-select: none;
  pointer-events: none;
}

#restartText {
  font-family: 'Turret Road', cursive;
  font-weight: 700;
  fill:rgb(255, 255, 255);
  user-select: none;
  pointer-events: none;
  opacity: 0;
}
</style>

<div id="wrapper" ontouchstart="">
<div class="bg"></div>

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1280 500" preserveAspectRatio="xMidYMid slice">
    <defs>
        <radialGradient id="polygonGradient" cx="50%" cy="50%" r="70%" gradientUnits="userSpaceOnUse">
            <stop offset="0%" stop-color="#414141" />
            <stop offset="100%" stop-color="black" />
        </radialGradient>

        <radialGradient id="transparentGradient" cx="50%" cy="50%" r="75%" gradientUnits="userSpaceOnUse">  
            <stop offset="0%" style="stop-color:rgb(29, 29, 29); stop-opacity:0.4" />
            <stop offset="100%" style="stop-color:rgb(29, 29, 29)" />
            </radialGradient>
    </defs>

    <g id="hexs" fill="url(#polygonGradient)">
        <polygon points="-34.2 38.5 -34.2 0.5 -1.3 -18.5 31.6 0.5 31.6 38.5 -1.3 57.5 -34.2 38.5"/>
        <polygon points="35.2 38.5 35.2 0.5 68.1 -18.5 101.1 0.5 101.1 38.5 68.1 57.5 35.2 38.5"/>
        <polygon points="104.7 38.5 104.7 0.5 137.6 -18.5 170.5 0.5 170.5 38.5 137.6 57.5 104.7 38.5"/>
        <polygon points="174.1 38.5 174.1 0.5 207 -18.5 240 0.5 240 38.5 207 57.5 174.1 38.5"/>
        <polygon points="243.6 38.5 243.6 0.5 276.5 -18.5 309.4 0.5 309.4 38.5 276.5 57.5 243.6 38.5"/>
        <polygon points="313 38.5 313 0.5 345.9 -18.5 378.9 0.5 378.9 38.5 345.9 57.5 313 38.5"/>
        <polygon points="382.5 38.5 382.5 0.5 415.4 -18.5 448.3 0.5 448.3 38.5 415.4 57.5 382.5 38.5"/>
        <polygon points="451.9 38.5 451.9 0.5 484.8 -18.5 517.8 0.5 517.8 38.5 484.8 57.5 451.9 38.5"/>
        <polygon points="521.4 38.5 521.4 0.5 554.3 -18.5 587.2 0.5 587.2 38.5 554.3 57.5 521.4 38.5"/>
        <polygon points="590.8 38.5 590.8 0.5 623.8 -18.5 656.7 0.5 656.7 38.5 623.8 57.5 590.8 38.5"/>
        <polygon points="660.3 38.5 660.3 0.5 693.2 -18.5 726.1 0.5 726.1 38.5 693.2 57.5 660.3 38.5"/>
        <polygon points="729.7 38.5 729.7 0.5 762.7 -18.5 795.6 0.5 795.6 38.5 762.7 57.5 729.7 38.5"/>
        <polygon points="799.2 38.5 799.2 0.5 832.1 -18.5 865 0.5 865 38.5 832.1 57.5 799.2 38.5"/>
        <polygon points="868.6 38.5 868.6 0.5 901.6 -18.5 934.5 0.5 934.5 38.5 901.6 57.5 868.6 38.5"/>
        <polygon points="938.1 38.5 938.1 0.5 971 -18.5 1003.9 0.5 1003.9 38.5 971 57.5 938.1 38.5"/>
        <polygon points="1007.5 38.5 1007.5 0.5 1040.5 -18.5 1073.4 0.5 1073.4 38.5 1040.5 57.5 1007.5 38.5"/>
        <polygon points="1077 38.5 1077 0.5 1109.9 -18.5 1142.8 0.5 1142.8 38.5 1109.9 57.5 1077 38.5"/>
        <polygon points="1146.4 38.5 1146.4 0.5 1179.4 -18.5 1212.3 0.5 1212.3 38.5 1179.4 57.5 1146.4 38.5"/>
        <polygon points="1215.9 38.5 1215.9 0.5 1248.8 -18.5 1281.7 0.5 1281.7 38.5 1248.8 57.5 1215.9 38.5"/>
        <polygon points="0.4 98.1 0.4 60.1 33.3 41.1 66.2 60.1 66.2 98.1 33.3 117.1 0.4 98.1"/>
        <polygon points="69.8 98.1 69.8 60.1 102.7 41.1 135.7 60.1 135.7 98.1 102.7 117.1 69.8 98.1"/>
        <polygon points="139.3 98.1 139.3 60.1 172.2 41.1 205.1 60.1 205.1 98.1 172.2 117.1 139.3 98.1"/>
        <polygon points="208.7 98.1 208.7 60.1 241.6 41.1 274.6 60.1 274.6 98.1 241.6 117.1 208.7 98.1"/>
        <polygon points="278.2 98.1 278.2 60.1 311.1 41.1 344 60.1 344 98.1 311.1 117.1 278.2 98.1"/>
        <polygon points="347.6 98.1 347.6 60.1 380.5 41.1 413.5 60.1 413.5 98.1 380.5 117.1 347.6 98.1"/>
        <polygon points="417.1 98.1 417.1 60.1 450 41.1 482.9 60.1 482.9 98.1 450 117.1 417.1 98.1"/>
        <polygon points="486.5 98.1 486.5 60.1 519.4 41.1 552.4 60.1 552.4 98.1 519.4 117.1 486.5 98.1"/>
        <polygon points="556 98.1 556 60.1 588.9 41.1 621.8 60.1 621.8 98.1 588.9 117.1 556 98.1"/>
        <polygon points="625.4 98.1 625.4 60.1 658.3 41.1 691.3 60.1 691.3 98.1 658.3 117.1 625.4 98.1"/>
        <polygon points="694.9 98.1 694.9 60.1 727.8 41.1 760.7 60.1 760.7 98.1 727.8 117.1 694.9 98.1"/>
        <polygon points="764.3 98.1 764.3 60.1 797.3 41.1 830.2 60.1 830.2 98.1 797.3 117.1 764.3 98.1"/>
        <polygon points="833.8 98.1 833.8 60.1 866.7 41.1 899.6 60.1 899.6 98.1 866.7 117.1 833.8 98.1"/>
        <polygon points="903.2 98.1 903.2 60.1 936.2 41.1 969.1 60.1 969.1 98.1 936.2 117.1 903.2 98.1"/>
        <polygon points="972.7 98.1 972.7 60.1 1005.6 41.1 1038.5 60.1 1038.5 98.1 1005.6 117.1 972.7 98.1"/>
        <polygon points="1042.1 98.1 1042.1 60.1 1075.1 41.1 1108 60.1 1108 98.1 1075.1 117.1 1042.1 98.1"/>
        <polygon points="1111.6 98.1 1111.6 60.1 1144.5 41.1 1177.4 60.1 1177.4 98.1 1144.5 117.1 1111.6 98.1"/>
        <polygon points="1181 98.1 1181 60.1 1214 41.1 1246.9 60.1 1246.9 98.1 1214 117.1 1181 98.1"/>
        <polygon points="1250.5 98.1 1250.5 60.1 1283.4 41.1 1316.3 60.1 1316.3 98.1 1283.4 117.1 1250.5 98.1"/>
        <polygon points="-34.4 158.2 -34.4 120.2 -1.5 101.2 31.4 120.2 31.4 158.2 -1.5 177.2 -34.4 158.2"/>
        <polygon points="35 158.2 35 120.2 67.9 101.2 100.9 120.2 100.9 158.2 67.9 177.2 35 158.2"/>
        <polygon points="104.5 158.2 104.5 120.2 137.4 101.2 170.3 120.2 170.3 158.2 137.4 177.2 104.5 158.2"/>
        <polygon points="173.9 158.2 173.9 120.2 206.8 101.2 239.8 120.2 239.8 158.2 206.8 177.2 173.9 158.2"/>
        <polygon points="243.4 158.2 243.4 120.2 276.3 101.2 309.2 120.2 309.2 158.2 276.3 177.2 243.4 158.2"/>
        <polygon points="312.8 158.2 312.8 120.2 345.7 101.2 378.7 120.2 378.7 158.2 345.7 177.2 312.8 158.2"/>
        <polygon points="382.3 158.2 382.3 120.2 415.2 101.2 448.1 120.2 448.1 158.2 415.2 177.2 382.3 158.2"/>
        <polygon points="451.7 158.2 451.7 120.2 484.6 101.2 517.6 120.2 517.6 158.2 484.6 177.2 451.7 158.2"/>
        <polygon points="521.2 158.2 521.2 120.2 554.1 101.2 587 120.2 587 158.2 554.1 177.2 521.2 158.2"/>
        <polygon points="590.6 158.2 590.6 120.2 623.5 101.2 656.5 120.2 656.5 158.2 623.5 177.2 590.6 158.2"/>
        <polygon points="660.1 158.2 660.1 120.2 693 101.2 725.9 120.2 725.9 158.2 693 177.2 660.1 158.2"/>
        <polygon points="729.5 158.2 729.5 120.2 762.4 101.2 795.4 120.2 795.4 158.2 762.4 177.2 729.5 158.2"/>
        <polygon points="799 158.2 799 120.2 831.9 101.2 864.8 120.2 864.8 158.2 831.9 177.2 799 158.2"/>
        <polygon points="868.4 158.2 868.4 120.2 901.4 101.2 934.3 120.2 934.3 158.2 901.4 177.2 868.4 158.2"/>
        <polygon points="937.9 158.2 937.9 120.2 970.8 101.2 1003.7 120.2 1003.7 158.2 970.8 177.2 937.9 158.2"/>
        <polygon points="1007.3 158.2 1007.3 120.2 1040.3 101.2 1073.2 120.2 1073.2 158.2 1040.3 177.2 1007.3 158.2"/>
        <polygon points="1076.8 158.2 1076.8 120.2 1109.7 101.2 1142.6 120.2 1142.6 158.2 1109.7 177.2 1076.8 158.2"/>
        <polygon points="1146.2 158.2 1146.2 120.2 1179.2 101.2 1212.1 120.2 1212.1 158.2 1179.2 177.2 1146.2 158.2"/>
        <polygon points="1215.7 158.2 1215.7 120.2 1248.6 101.2 1281.5 120.2 1281.5 158.2 1248.6 177.2 1215.7 158.2"/>
        <polygon points="0.2 217.8 0.2 179.8 33.1 160.7 66 179.8 66 217.8 33.1 236.8 0.2 217.8"/>
        <polygon points="69.6 217.8 69.6 179.8 102.5 160.7 135.5 179.8 135.5 217.8 102.5 236.8 69.6 217.8"/>
        <polygon points="139.1 217.8 139.1 179.8 172 160.7 204.9 179.8 204.9 217.8 172 236.8 139.1 217.8"/>
        <polygon points="208.5 217.8 208.5 179.8 241.4 160.7 274.4 179.8 274.4 217.8 241.4 236.8 208.5 217.8"/>
        <polygon points="278 217.8 278 179.8 310.9 160.7 343.8 179.8 343.8 217.8 310.9 236.8 278 217.8"/>
        <polygon points="347.4 217.8 347.4 179.8 380.3 160.7 413.3 179.8 413.3 217.8 380.3 236.8 347.4 217.8"/>
        <polygon points="416.9 217.8 416.9 179.8 449.8 160.7 482.7 179.8 482.7 217.8 449.8 236.8 416.9 217.8"/>
        <polygon points="486.3 217.8 486.3 179.8 519.2 160.7 552.2 179.8 552.2 217.8 519.2 236.8 486.3 217.8"/>
        <polygon points="555.8 217.8 555.8 179.8 588.7 160.7 621.6 179.8 621.6 217.8 588.7 236.8 555.8 217.8"/>
        <polygon points="625.2 217.8 625.2 179.8 658.1 160.7 691.1 179.8 691.1 217.8 658.1 236.8 625.2 217.8"/>
        <polygon points="694.7 217.8 694.7 179.8 727.6 160.7 760.5 179.8 760.5 217.8 727.6 236.8 694.7 217.8"/>
        <polygon points="764.1 217.8 764.1 179.8 797 160.7 830 179.8 830 217.8 797 236.8 764.1 217.8"/>
        <polygon points="833.6 217.8 833.6 179.8 866.5 160.7 899.4 179.8 899.4 217.8 866.5 236.8 833.6 217.8"/>
        <polygon points="903 217.8 903 179.8 935.9 160.7 968.9 179.8 968.9 217.8 935.9 236.8 903 217.8"/>
        <polygon points="972.5 217.8 972.5 179.8 1005.4 160.7 1038.3 179.8 1038.3 217.8 1005.4 236.8 972.5 217.8"/>
        <polygon points="1041.9 217.8 1041.9 179.8 1074.8 160.7 1107.8 179.8 1107.8 217.8 1074.8 236.8 1041.9 217.8"/>
        <polygon points="1111.4 217.8 1111.4 179.8 1144.3 160.7 1177.2 179.8 1177.2 217.8 1144.3 236.8 1111.4 217.8"/>
        <polygon points="1180.8 217.8 1180.8 179.8 1213.8 160.7 1246.7 179.8 1246.7 217.8 1213.8 236.8 1180.8 217.8"/>
        <polygon points="1250.3 217.8 1250.3 179.8 1283.2 160.7 1316.1 179.8 1316.1 217.8 1283.2 236.8 1250.3 217.8"/>
        <polygon points="-34.7 277.6 -34.7 239.6 -1.8 220.6 31.2 239.6 31.2 277.6 -1.8 296.6 -34.7 277.6"/>
        <polygon points="34.8 277.6 34.8 239.6 67.7 220.6 100.6 239.6 100.6 277.6 67.7 296.6 34.8 277.6"/>
        <polygon points="104.2 277.6 104.2 239.6 137.1 220.6 170.1 239.6 170.1 277.6 137.1 296.6 104.2 277.6"/>
        <polygon points="173.7 277.6 173.7 239.6 206.6 220.6 239.5 239.6 239.5 277.6 206.6 296.6 173.7 277.6"/>
        <polygon points="243.1 277.6 243.1 239.6 276 220.6 309 239.6 309 277.6 276 296.6 243.1 277.6"/>
        <polygon points="312.6 277.6 312.6 239.6 345.5 220.6 378.4 239.6 378.4 277.6 345.5 296.6 312.6 277.6"/>
        <polygon points="382 277.6 382 239.6 414.9 220.6 447.9 239.6 447.9 277.6 414.9 296.6 382 277.6"/>
        <polygon points="451.5 277.6 451.5 239.6 484.4 220.6 517.3 239.6 517.3 277.6 484.4 296.6 451.5 277.6"/>
        <polygon points="520.9 277.6 520.9 239.6 553.8 220.6 586.8 239.6 586.8 277.6 553.8 296.6 520.9 277.6"/>
        <polygon points="590.4 277.6 590.4 239.6 623.3 220.6 656.2 239.6 656.2 277.6 623.3 296.6 590.4 277.6"/>
        <polygon points="659.8 277.6 659.8 239.6 692.8 220.6 725.7 239.6 725.7 277.6 692.8 296.6 659.8 277.6"/>
        <polygon points="729.3 277.6 729.3 239.6 762.2 220.6 795.1 239.6 795.1 277.6 762.2 296.6 729.3 277.6"/>
        <polygon points="798.7 277.6 798.7 239.6 831.7 220.6 864.6 239.6 864.6 277.6 831.7 296.6 798.7 277.6"/>
        <polygon points="868.2 277.6 868.2 239.6 901.1 220.6 934 239.6 934 277.6 901.1 296.6 868.2 277.6"/>
        <polygon points="937.6 277.6 937.6 239.6 970.6 220.6 1003.5 239.6 1003.5 277.6 970.6 296.6 937.6 277.6"/>
        <polygon points="1007.1 277.6 1007.1 239.6 1040 220.6 1072.9 239.6 1072.9 277.6 1040 296.6 1007.1 277.6"/>
        <polygon points="1076.5 277.6 1076.5 239.6 1109.5 220.6 1142.4 239.6 1142.4 277.6 1109.5 296.6 1076.5 277.6"/>
        <polygon points="1146 277.6 1146 239.6 1178.9 220.6 1211.8 239.6 1211.8 277.6 1178.9 296.6 1146 277.6"/>
        <polygon points="1215.4 277.6 1215.4 239.6 1248.4 220.6 1281.3 239.6 1281.3 277.6 1248.4 296.6 1215.4 277.6"/>
        <polygon points="-0.1 337.2 -0.1 299.1 32.8 280.1 65.8 299.1 65.8 337.2 32.8 356.2 -0.1 337.2"/>
        <polygon points="69.4 337.2 69.4 299.1 102.3 280.1 135.2 299.1 135.2 337.2 102.3 356.2 69.4 337.2"/>
        <polygon points="138.8 337.2 138.8 299.1 171.7 280.1 204.7 299.1 204.7 337.2 171.7 356.2 138.8 337.2"/>
        <polygon points="208.3 337.2 208.3 299.1 241.2 280.1 274.1 299.1 274.1 337.2 241.2 356.2 208.3 337.2"/>
        <polygon points="277.7 337.2 277.7 299.1 310.6 280.1 343.6 299.1 343.6 337.2 310.6 356.2 277.7 337.2"/>
        <polygon points="347.2 337.2 347.2 299.1 380.1 280.1 413 299.1 413 337.2 380.1 356.2 347.2 337.2"/>
        <polygon points="416.6 337.2 416.6 299.1 449.5 280.1 482.5 299.1 482.5 337.2 449.5 356.2 416.6 337.2"/>
        <polygon points="486.1 337.2 486.1 299.1 519 280.1 551.9 299.1 551.9 337.2 519 356.2 486.1 337.2"/>
        <polygon points="555.5 337.2 555.5 299.1 588.4 280.1 621.4 299.1 621.4 337.2 588.4 356.2 555.5 337.2"/>
        <polygon points="625 337.2 625 299.1 657.9 280.1 690.8 299.1 690.8 337.2 657.9 356.2 625 337.2"/>
        <polygon points="694.4 337.2 694.4 299.1 727.3 280.1 760.3 299.1 760.3 337.2 727.3 356.2 694.4 337.2"/>
        <polygon points="763.9 337.2 763.9 299.1 796.8 280.1 829.7 299.1 829.7 337.2 796.8 356.2 763.9 337.2"/>
        <polygon points="833.3 337.2 833.3 299.1 866.2 280.1 899.2 299.1 899.2 337.2 866.2 356.2 833.3 337.2"/>
        <polygon points="902.8 337.2 902.8 299.1 935.7 280.1 968.6 299.1 968.6 337.2 935.7 356.2 902.8 337.2"/>
        <polygon points="972.2 337.2 972.2 299.1 1005.2 280.1 1038.1 299.1 1038.1 337.2 1005.2 356.2 972.2 337.2"/>
        <polygon points="1041.7 337.2 1041.7 299.1 1074.6 280.1 1107.5 299.1 1107.5 337.2 1074.6 356.2 1041.7 337.2"/>
        <polygon points="1111.1 337.2 1111.1 299.1 1144.1 280.1 1177 299.1 1177 337.2 1144.1 356.2 1111.1 337.2"/>
        <polygon points="1180.6 337.2 1180.6 299.1 1213.5 280.1 1246.4 299.1 1246.4 337.2 1213.5 356.2 1180.6 337.2"/>
        <polygon points="1250 337.2 1250 299.1 1283 280.1 1315.9 299.1 1315.9 337.2 1283 356.2 1250 337.2"/>
        <polygon points="-34.9 397.3 -34.9 359.3 -2 340.2 31 359.3 31 397.3 -2 416.3 -34.9 397.3"/>
        <polygon points="34.6 397.3 34.6 359.3 67.5 340.2 100.4 359.3 100.4 397.3 67.5 416.3 34.6 397.3"/>
        <polygon points="104 397.3 104 359.3 136.9 340.2 169.9 359.3 169.9 397.3 136.9 416.3 104 397.3"/>
        <polygon points="173.5 397.3 173.5 359.3 206.4 340.2 239.3 359.3 239.3 397.3 206.4 416.3 173.5 397.3"/>
        <polygon points="242.9 397.3 242.9 359.3 275.8 340.2 308.8 359.3 308.8 397.3 275.8 416.3 242.9 397.3"/>
        <polygon points="312.4 397.3 312.4 359.3 345.3 340.2 378.2 359.3 378.2 397.3 345.3 416.3 312.4 397.3"/>
        <polygon points="381.8 397.3 381.8 359.3 414.7 340.2 447.7 359.3 447.7 397.3 414.7 416.3 381.8 397.3"/>
        <polygon points="451.3 397.3 451.3 359.3 484.2 340.2 517.1 359.3 517.1 397.3 484.2 416.3 451.3 397.3"/>
        <polygon points="520.7 397.3 520.7 359.3 553.6 340.2 586.6 359.3 586.6 397.3 553.6 416.3 520.7 397.3"/>
        <polygon points="590.2 397.3 590.2 359.3 623.1 340.2 656 359.3 656 397.3 623.1 416.3 590.2 397.3"/>
        <polygon points="659.6 397.3 659.6 359.3 692.5 340.2 725.5 359.3 725.5 397.3 692.5 416.3 659.6 397.3"/>
        <polygon points="729.1 397.3 729.1 359.3 762 340.2 794.9 359.3 794.9 397.3 762 416.3 729.1 397.3"/>
        <polygon points="798.5 397.3 798.5 359.3 831.4 340.2 864.4 359.3 864.4 397.3 831.4 416.3 798.5 397.3"/>
        <polygon points="868 397.3 868 359.3 900.9 340.2 933.8 359.3 933.8 397.3 900.9 416.3 868 397.3"/>
        <g>
           <polygon  id="restartPolygon" points="937.4 397.3 937.4 359.3 970.4 340.2 1003.3 359.3 1003.3 397.3 970.4 416.3 937.4 397.3"/>
           <text id="restartText" fill="#fff" dy="1.5%" dx="-27">Restart</text>
        </g>
        <polygon points="1006.9 397.3 1006.9 359.3 1039.8 340.2 1072.7 359.3 1072.7 397.3 1039.8 416.3 1006.9 397.3"/>
        <polygon points="1076.3 397.3 1076.3 359.3 1109.3 340.2 1142.2 359.3 1142.2 397.3 1109.3 416.3 1076.3 397.3"/>
        <polygon points="1145.8 397.3 1145.8 359.3 1178.7 340.2 1211.6 359.3 1211.6 397.3 1178.7 416.3 1145.8 397.3"/>
        <polygon points="1215.2 397.3 1215.2 359.3 1248.2 340.2 1281.1 359.3 1281.1 397.3 1248.2 416.3 1215.2 397.3"/>
        <polygon points="-0.3 456.8 -0.3 418.8 32.6 399.8 65.6 418.8 65.6 456.8 32.6 475.8 -0.3 456.8"/>
        <polygon points="69.2 456.8 69.2 418.8 102.1 399.8 135 418.8 135 456.8 102.1 475.8 69.2 456.8"/>
        <polygon points="138.6 456.8 138.6 418.8 171.5 399.8 204.5 418.8 204.5 456.8 171.5 475.8 138.6 456.8"/>
        <polygon points="208.1 456.8 208.1 418.8 241 399.8 273.9 418.8 273.9 456.8 241 475.8 208.1 456.8"/>
        <polygon points="277.5 456.8 277.5 418.8 310.4 399.8 343.4 418.8 343.4 456.8 310.4 475.8 277.5 456.8"/>
        <polygon points="347 456.8 347 418.8 379.9 399.8 412.8 418.8 412.8 456.8 379.9 475.8 347 456.8"/>
        <polygon points="416.4 456.8 416.4 418.8 449.3 399.8 482.3 418.8 482.3 456.8 449.3 475.8 416.4 456.8"/>
        <polygon points="485.9 456.8 485.9 418.8 518.8 399.8 551.7 418.8 551.7 456.8 518.8 475.8 485.9 456.8"/>
        <polygon points="555.3 456.8 555.3 418.8 588.2 399.8 621.2 418.8 621.2 456.8 588.2 475.8 555.3 456.8"/>
        <polygon points="624.8 456.8 624.8 418.8 657.7 399.8 690.6 418.8 690.6 456.8 657.7 475.8 624.8 456.8"/>
        <polygon points="694.2 456.8 694.2 418.8 727.1 399.8 760.1 418.8 760.1 456.8 727.1 475.8 694.2 456.8"/>
        <polygon points="763.7 456.8 763.7 418.8 796.6 399.8 829.5 418.8 829.5 456.8 796.6 475.8 763.7 456.8"/>
        <polygon points="833.1 456.8 833.1 418.8 866 399.8 899 418.8 899 456.8 866 475.8 833.1 456.8"/>
        <polygon points="902.6 456.8 902.6 418.8 935.5 399.8 968.4 418.8 968.4 456.8 935.5 475.8 902.6 456.8"/>
        <polygon points="972 456.8 972 418.8 1004.9 399.8 1037.9 418.8 1037.9 456.8 1004.9 475.8 972 456.8"/>
        <polygon points="1041.5 456.8 1041.5 418.8 1074.4 399.8 1107.3 418.8 1107.3 456.8 1074.4 475.8 1041.5 456.8"/>
        <polygon points="1110.9 456.8 1110.9 418.8 1143.8 399.8 1176.8 418.8 1176.8 456.8 1143.8 475.8 1110.9 456.8"/>
        <polygon points="1180.4 456.8 1180.4 418.8 1213.3 399.8 1246.2 418.8 1246.2 456.8 1213.3 475.8 1180.4 456.8"/>
        <polygon points="1249.8 456.8 1249.8 418.8 1282.8 399.8 1315.7 418.8 1315.7 456.8 1282.8 475.8 1249.8 456.8"/>
        <polygon points="-35 516.4 -35 478.4 -2.1 459.4 30.8 478.4 30.8 516.4 -2.1 535.4 -35 516.4"/>
        <polygon points="34.4 516.4 34.4 478.4 67.4 459.4 100.3 478.4 100.3 516.4 67.4 535.4 34.4 516.4"/>
        <polygon points="103.9 516.4 103.9 478.4 136.8 459.4 169.7 478.4 169.7 516.4 136.8 535.4 103.9 516.4"/>
        <polygon points="173.3 516.4 173.3 478.4 206.3 459.4 239.2 478.4 239.2 516.4 206.3 535.4 173.3 516.4"/>
        <polygon points="242.8 516.4 242.8 478.4 275.7 459.4 308.6 478.4 308.6 516.4 275.7 535.4 242.8 516.4"/>
        <polygon points="312.2 516.4 312.2 478.4 345.2 459.4 378.1 478.4 378.1 516.4 345.2 535.4 312.2 516.4"/>
        <polygon points="381.7 516.4 381.7 478.4 414.6 459.4 447.5 478.4 447.5 516.4 414.6 535.4 381.7 516.4"/>
        <polygon points="451.1 516.4 451.1 478.4 484.1 459.4 517 478.4 517 516.4 484.1 535.4 451.1 516.4"/>
        <polygon points="520.6 516.4 520.6 478.4 553.5 459.4 586.4 478.4 586.4 516.4 553.5 535.4 520.6 516.4"/>
        <polygon points="590 516.4 590 478.4 623 459.4 655.9 478.4 655.9 516.4 623 535.4 590 516.4"/>
        <polygon points="659.5 516.4 659.5 478.4 692.4 459.4 725.3 478.4 725.3 516.4 692.4 535.4 659.5 516.4"/>
        <polygon points="728.9 516.4 728.9 478.4 761.9 459.4 794.8 478.4 794.8 516.4 761.9 535.4 728.9 516.4"/>
        <polygon points="798.4 516.4 798.4 478.4 831.3 459.4 864.2 478.4 864.2 516.4 831.3 535.4 798.4 516.4"/>
        <polygon points="867.8 516.4 867.8 478.4 900.8 459.4 933.7 478.4 933.7 516.4 900.8 535.4 867.8 516.4"/>
        <polygon points="937.3 516.4 937.3 478.4 970.2 459.4 1003.1 478.4 1003.1 516.4 970.2 535.4 937.3 516.4"/>
        <polygon points="1006.7 516.4 1006.7 478.4 1039.7 459.4 1072.6 478.4 1072.6 516.4 1039.7 535.4 1006.7 516.4"/>
        <polygon points="1076.2 516.4 1076.2 478.4 1109.1 459.4 1142 478.4 1142 516.4 1109.1 535.4 1076.2 516.4"/>
        <polygon points="1145.6 516.4 1145.6 478.4 1178.6 459.4 1211.5 478.4 1211.5 516.4 1178.6 535.4 1145.6 516.4"/>
        <polygon points="1215.1 516.4 1215.1 478.4 1248 459.4 1280.9 478.4 1280.9 516.4 1248 535.4 1215.1 516.4"/>
    </g>

    <text id="startText" dy="8.5%" dx="5" >Start</text>
    <circle id="redDot" cx="0" cy="0" r="3" fill="red"></circle>
</svg>
</div>


<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/gsap/2.1.3/TweenMax.min.js"></script>
<script type="text/javascript">
var polygons = document.querySelectorAll("#hexs polygon");
var restartPolygon = document.getElementById("restartPolygon");
var restartText = document.getElementById("restartText");
var redDot = document.getElementById("redDot");
var startText = document.getElementById("startText");
var center = 85;
var polygonCenter = polygons[center];
polygonCenter.classList.add("center");
var polygonsRows = [];
var j = -1;
var desetica = 1;
for (var i = 1; i < 10; i++) {
    window['polygons' + i] = [];
    polygonsRows.push(window['polygons' + i])
}
for (var i = 0; i < polygons.length; i++) {
    j++;
    if (j < 19) {
        window['polygons' + desetica].push(polygons[i]);
        if (j === 18) {
            j = -1;
            desetica++;
        }
    }
}

function changeCentar() {
    startText.setAttribute("x", polygonCenter.getBBox().x);
    startText.setAttribute("y", polygonCenter.getBBox().y)
    startText.setAttribute("textLength", polygonCenter.getBBox().width - 10) 
}
changeCentar(); 
window.onresize = function (event) {
    changeCentar();
}

polygonCenter.addEventListener("click", function () {
    tl.play("start");
    this.removeEventListener("click", arguments.callee);
}, false);

//GSAP Timeline
var tl = new TimelineMax({ delay: 0.5, paused: true });

//do nothing
tl.to(redDot, 0.5, { y: -1 });
tl.add("start");
tl.set(redDot, { visibility: "hidden" });
tl.set(polygonCenter, { opacity: 1 });
tl.to(polygons[center - 19], 0.1, { opacity: 0.2, delay: 0.1 });
tl.to(polygons[center - 20], 0.1, { opacity: 0.2, delay: 0.1 });
tl.to(polygons[center - 1], 0.1, { opacity: 0.2, delay: 0.1 });
tl.to(polygons[center + 18], 0.1, { opacity: 0.2, delay: 0.1 });
tl.to(polygons[center + 19], 0.1, { opacity: 0.2, delay: 0.1 });
tl.to(polygons[center + 1], 0.1, { opacity: 0.2, delay: 0.1 });
tl.to(polygons[center], 0.1, { opacity: 0, delay: 0.1 })
tl.to(startText, 0.5, { scale: 2.2, transformOrigin: "50% 50%", ease: Elastic.easeOut.config(1, 0.3) }, "-=0.6");
tl.to(polygons, 1, { rotation: 30, x: 20, y: -10 });
tl.add("HeyYOU");
tl.call(function () { startText.innerHTML = "Hey YOU!" });
tl.set(startText, { opacity: 0, attr: { textLength: 160 }, scale: 1, x: -50, fontSize: "2.5vw" });
tl.staggerTo(polygons, 0.7, { scaleX: 1.2, scaleY: 0.8, ease: Power1.easeOut, stagger: { amount: 0.5, from: "center" } }, "HeyYOU");
tl.to(startText, 0.7, { opacity: 1, }, "HeyYOU");
tl.set(startText, { x: "+=47px", scale: 1.3 });
tl.call(function () { startText.innerHTML = "you" });
tl.to(startText, 1, { attr: { textLength: 60 }, ease: Elastic.easeOut.config(1, 0.3) });
tl.staggerTo(polygons, 1, { scaleX: 1, scaleY: 1, ease: Power1.easeOut, stagger: { amount: 0.3, from: "center" } });
tl.call(function () { startText.innerHTML = "are" });
tl.to(startText, 0.5, { scale: 1.8, transformOrigin: "50% 50%", ease: Elastic.easeOut.config(1, 0.3) }, "-=0.5");
tl.staggerTo(polygons, 0.7, { scaleX: 0.1, scaleY: 2, ease: Power1.easeOut, stagger: { amount: 0.5, from: "center" } });
tl.call(function () { startText.innerHTML = "awesome" });
tl.to(startText, 0.5, { attr: { textLength: 160 }, scale: 1, x: -60, ease: Elastic.easeOut.config(1, 0.3) })
tl.staggerTo(polygons, 0.7, { scaleX: 1, scaleY: 1, ease: Power1.easeOut, stagger: { amount: 0.5, from: "center" } });
tl.staggerTo(polygons, 1, { opacity: 0, ease: Elastic.easeInOut.config(1, 0.3), stagger: { amount: 0.5, from: "center" } });
tl.to(startText, 0.2, { opacity: 0 }, "-=1.2");
tl.set(polygons, { y: 500, opacity: 1 });
tl.staggerTo(polygonsRows, 1, { y: 0, ease: Power3.easeOut, stagger: { amount: 1 } });
tl.staggerTo(polygons, 1, { rotation: 0, x: 0, y: 0, ease: Back.easeOut.config(1.7), stagger: { amount: 1 } });
tl.staggerTo(polygons, 1.5, { rotation: 0, ease: Elastic.easeInOut.config(1, 0.3), cycle: { x: [0, 50] }, stagger: { amount: 0.5 } });
tl.staggerTo(polygons, 1.5, { x: 0, ease: Elastic.easeInOut.config(1, 0.3), cycle: { x: [50, 0], scale: [0, 1.2] }, stagger: { amount: 0.5 } });
tl.staggerTo(polygons, 1, { scale: 1, x: 0, ease: Elastic.easeInOut.config(1, 0.3), stagger: { amount: 0.5 } });
tl.staggerTo(polygons, 2, { scale: 0.5, rotation: 90, ease: Elastic.easeInOut.config(1, 0.3), cycle: { y: [16, -16, 8, -8] }, stagger: { amount: 0.5 } });
tl.staggerTo(polygons, 1.5, { scale: 1, rotation: -120, y: 70, x: 10, stagger: { amount: 0.5, from: "end" } });
tl.staggerTo(polygons, 0.2, { fill: "url(#transparentGradient)", ease: Elastic.easeInOut.config(1, 0.3), stagger: { amount: 0.2, from: center } }, "-=0.5");
tl.staggerTo(polygons, 2, { rotation: -60, yoyo: true, repeat: 1, ease: Sine.easeInOut, cycle: { y: [150, 150, 150, 150, 150, 150, 150, 150, 150, 150, 150, 150, 150, 150, 150, 150, 150, 150, 150, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0] }, stagger: { amount: 0.5 } });
tl.to(polygonCenter, 1, { scale: 0, rotation: 360, transformOrigin: "50% 50%" });
tl.staggerTo("polygon:not(.center)", 1, { scale: 1, x: 0, y: 0, rotation: 0, ease: Elastic.easeInOut.config(1, 0.3) });
tl.to(".bg", 1, { opacity: 0 }, 31);  
tl.call(function () { document.getElementById("wrapper").style.animationPlayState = 'running' }, this, 30);
tl.call(restartShow, this, 32);
tl.set(redDot, { visibility: "visible" });
tl.to(redDot, 0.4, { opacity: 0, yoyo: true, repeat: -1 });
tl.set(restartPolygon, { cursor: "pointer" });


function restartShow() {
    var x = Math.floor(restartPolygon.getBBox().width / 2 + restartPolygon.getBBox().x);
    var y = Math.floor(restartPolygon.getBBox().height / 2 + restartPolygon.getBBox().y);

    redDot.setAttribute("cx", x + "px");
    redDot.setAttribute("cy", y + 20 + "px");

    restartText.setAttribute("x", x + "px");
    restartText.setAttribute("y", y + "px");

    tl.to(restartPolygon, 1.7, { opacity: 0.5 }, "-=1");
    tl.to(restartText, 1.7, { opacity: 1 }, "-=1");

    restartPolygon.addEventListener("click", function () {
        startText.innerHTML = "Start";
        tl.restart();
        this.removeEventListener("click", arguments.callee);
    }, false);

}
</script>

