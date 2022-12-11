# Tatiana Pokareva
---
# My Contact Info:
* Address: Togliatti, Russia
* Phone: +7(917)974-15-07
* E-mail: tanyapokareva2002@gmail.com
* GitHub: ta-pokareva21
---
# About me
I am a third-year student at Samara University. My specialty is "computer science and computer engineering". My goal is to master the profession. I have always studied and continue to study with great aspiration. My main motivation is learning something new, communicating with interesting people and the results of my hard work.
---
# My skills
* HTML
* CSS
* JS(basic knowledge)
* С#
* Version control: Git (remote service GitHub)
* Java(basic knowledge)
* Python
* Editors: Sublime Text, VSCode, VS, PyCharm, IntelliJ IDEA Community
---
# Сode examples 
```javascript
const personalMovieDB = {
    count: 0,
    movies: {},
    actors: {},
    genres: [],
    private: false,
    start: function() {
        personalMovieDB.count = +prompt('How many movies have you watched so far?','');

        while (personalMovieDB.count == '' || personalMovieDB.count == null || isNaN(personalMovieDB.count)) {
            personalMovieDB.count = +prompt('How many movies have you watched so far?','');
        }
    },
    rememberMyFilms: function () {
        for (let i = 0; i < 2; i++) {
            const a = prompt('One of the last movies you watched?','').trim(),
                  b = +prompt('How much do you rate it?','').trim();
            if ( a != null && b != null &&  a != '' && a.length <=50 && b !=''){
                personalMovieDB.movies[a] = b;
                console.log('done');
            } else {
                console.log('error')
                i--;
            }
        }
    },
    detectPersonalLevel: function () {
        if (personalMovieDB.count < 10){
            console.log("Quite a few movies have been viewed");
        }
        else if(personalMovieDB.count >= 10 && personalMovieDB.count <=30){
            console.log("You are a classic spectator");
        }
        else if(personalMovieDB.count > 30){
            console.log("You're a movie fan!");
        }else{
            console.log("An error has occurred")}
        
    },
    showMyDB: function (hidden) {
        if(!hidden){
            console.log(personalMovieDB);
        }
    },
    toggleVisibleMyDB: function(){
        if(personalMovieDB.private){
            personalMovieDB.private = false;
        }else {
            personalMovieDB.private = true;
        }
    },
    writeYourGenres: function() {
        let genres=[];
        for(let i = 1; i < 4; i++){
            let genre = prompt(`Your favorite genre is numbered ${i}`); 
            if( genre === '' || genre === null){
                console.log("You entered incorrect data or did not enter it at all");
                i--;
            }else {
            personalMovieDB.genres[i-1] = genre;
            }
        }
        personalMovieDB.genres.forEach((item,i) => {
            console.log(`Favorite genre ${i+1} this is ${item}`);
        });
    }
};
```
---
# Work experience
No work experience.
---
# Education
* 3 courses of Samara university
# English language
My English level is A2.
---