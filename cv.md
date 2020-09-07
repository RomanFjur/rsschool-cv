1. **Name and Surname:**Raman Zhminko;
2. **Phone number:** +375-(29)-206-82-86; **Email:** www.ramanzhminko@gmail.com;
3. **About me:** My name is Raman (shortly Roma) and I'm 28 years old. I want to create awesome websites and SPA's with totally complicated animations, great and clear functional, interesting and unique web-applications. I now that it's hard, but it's very interesting and epic process for me. When you writing code that after all hours and days start working correctly and as you wanted - it's cool and awesome! I want to learn and create more!
4. **Skills:**
   * JavaScript;
   * HTML;
   * CSS;
   * Less/Sass;
   * Gulp;
   * Git;
   * JSON;
   * BEM.

   **Tools:**
   * Atom;
   * Adobe Photoshop CS6;
   * Figma;
   * GitKraken;
   * iTerm;
   * Android Studio;
   * Xcode;
   * MAMP.
5. **Code example:**
   *Timer*
   ```javascript
   const deadline = '2020-05-11';

   function getTimeRemaining(endtime) {
       const t = Date.parse(endtime) - Date.parse(new Date()),
           days = Math.floor( (t/(1000*60*60*24)) ),
           seconds = Math.floor( (t/1000) % 60 ),
           minutes = Math.floor( (t/1000/60) % 60 ),
           hours = Math.floor( (t/(1000*60*60) % 24) );

       return {
           'total': t,
           'days': days,
           'hours': hours,
           'minutes': minutes,
           'seconds': seconds
       };
   }

   function getZero(num){
       if (num >= 0 && num < 10) {
           return '0' + num;
       } else {
           return num;
       }
   }

   function setClock(selector, endtime) {

       const timer = document.querySelector(selector),
           days = timer.querySelector("#days"),
           hours = timer.querySelector('#hours'),
           minutes = timer.querySelector('#minutes'),
           seconds = timer.querySelector('#seconds'),
           timeInterval = setInterval(updateClock, 1000);

       updateClock();

       function updateClock() {
           const t = getTimeRemaining(endtime);

           days.innerHTML = getZero(t.days);
           hours.innerHTML = getZero(t.hours);
           minutes.innerHTML = getZero(t.minutes);
           seconds.innerHTML = getZero(t.seconds);

           if (t.total <= 0) {
               clearInterval(timeInterval);
           }
       }
   }

   setClock('.timer', deadline);
   ```
6. **Experience:** https://github.com/RomanFjur;
7. **Education:** HTMLAcademy courses, Udemy courses, self education;
8. **English:** Level A2;
