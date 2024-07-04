# Thanks for viewing my Project ✨

![ a main page screenshot](./images/screen.png)
<br />

## :star: Live Deployment: https://katarzynadworak.github.io/rwd-website-project/
<br />

## Main goal of my work was to:
- code **Responsive Web Design (RWD)** site 📱
- do it in a way that it **looks decent on mobiles, tablets and desktops** 🖥️
- use **semantic HTML** (BEM) 📝
- make project **as readable as it is possible** (clean code, many directories, BEM) 📖
<br />

### Solutions provided in the project
This project uses modern CSS functions like min(), max(), and clamp() to create a responsive and adaptive design. These functions help ensure that the layout and elements adjust smoothly across different screen sizes and resolutions.

Key Features:
Clamp() Function:

clamp() is used extensively to define flexible padding, margins, font sizes, and other properties. This allows for setting minimum, preferred, and maximum values for various elements, ensuring they scale properly on different devices.
Example: padding: clamp(10px, 2vw, 20px); ensures that padding will be at least 10px, preferably 2% of the viewport width, but not more than 20px.
Min() and Max() Functions:

These functions are used to set upper and lower bounds for various properties, allowing for more control over the layout.
Example: letter-spacing: max(1px, 0.1vw); ensures that letter spacing will be at least 1px but can increase to 0.1% of the viewport width.
Benefits:
Responsiveness: Elements adjust dynamically to the screen size, providing a consistent and user-friendly experience across different devices.
Maintainability: Using these functions reduces the need for numerous media queries, simplifying the CSS code.
Design Consistency: Ensures a consistent look and feel, regardless of the screen size, by setting appropriate limits on property values.
This approach leverages the power of modern CSS to create a more efficient, scalable, and maintainable codebase.



1. Hamburger rozwijany
2. Responsywne obrazy 
</br>

</br>
/* Styl dla elementów menu po najechaniu kursorem */

    .nav__item:hover {
        font-weight: bold; /* Pogrubienie tekstu */
        letter-spacing: 1px; /* Oddalenie liter */
        transform: translateX(5px); /* Przesunięcie elementu */
    }
   
</br>  
3. Zmieniające się przyciski po najechaniu myszką
   
    .header__button {
        margin-right: 26px;
        margin-top: 30px;
    }
    
    .header__button--download {
        background-color: #0885f6;
        border-radius: 5px;
        border: 2px solid #0885f6;
        width: 106px;
        padding: 10px;
        color: #f2f4f4;
        font-size: 15px;
        transition: .3s linear;
    }

    .header__button--download:hover {
        background-color: #f2f4f4;
        color: #0885f6;
    }

    </br>

- Linear-gradient used for CSS background property along with an image allowed to achieve the effect of colored overlay. As linear-gradient is now well-supported across different browsers, using it is a more convenient and space-saving way of creating an overlay than doing it with CSS pseudo-elements.
background: linear-gradient(rgba(97, 179, 255, 0.9), rgba(97, 179, 255, 0.9)),
		    url(../images/banner/testmonial.png) no-repeat center center/cover;
- Grid provides flexibility to footer elements – they can be stretched in one row as well as arranged in two or one column.

# Conclusions for future projects
I found a way to improve margin and padding changes depending on resolution. In this project they are modified with media queries in the place of their occurrence. In the future projects I will definitely use Sass @extend rule, keeping all shared measures in one place and changing them with only one time use of media queries per breakpoint. Example of usage beneath:

###### File storing resolution values:
%shared-pd {
  padding: 10px;
  @include tablet-and-landscape {
    padding: 50px;
  }
  @include desktop {
    padding: 100px;
  }
}

###### Values shared between different elements:
.footer-up {
	@extend %shared-pd;
}
.download {
	@extend %shared-pd;
}
Thanks
To Colorlib for free templates.
To my mentor for creating the task and for the code review.

## 🛠️ Languages and Tools used: 


<img align="left" alt="HTML5" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/html/html.png" />

<img align="left" alt="CSS3" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/css/css.png" />

<img align="left" alt="Git" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/git/git.png" />

<img align="left" alt="GitHub" width="50px" src="https://raw.githubusercontent.com/github/explore/78df643247d429f6cc873026c0622819ad797942/topics/github/github.png" />

<img align="left" alt="Terminal" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/terminal/terminal.png" />

<img align="left" alt="Visual Studio Code" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/visual-studio-code/visual-studio-code.png" />
<br />

### :blue_heart:  You can find me on:
<br/>

 Portfolio Website *(during construction*)* [<img align="left" alt="Portfolio" width="22px" src="https://raw.githubusercontent.com/iconic/open-iconic/master/svg/globe.svg" />][website]

 LinkedIn Profile [<img align="left" alt="Katarzynadworak LinkedIn" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/linkedin.svg" />][linkedin]
 
 Maybe my Instagram? [<img align="left" alt="@katarzynadworakk instagram" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/instagram.svg" />][instagram]

 Or Facebook? [<img align="left" alt="" width="22px" src="https://www.flaticon.com/svg/static/icons/svg/61/61045.svg" />][facebook]
<br />

### Copyright

Wszelkie prawa autorskie oraz pokrewne do szablonu i elementów wchodzacych w jego skład należą do [colorlib.com](https://colorlib.com).
Szablon i jego elementy mogą być wykorzystywane na zasadach zgodnych z [licencją](https://colorlib.com/wp/licence/).

[website]: google.com
[linkedin]: https://www.linkedin.com/in/katarzynadworak/
[instagram]: https://www.instagram.com/katarzynadworakk
[facebook]: https://www.facebook.com/katarzynadworakk
<br />



#### 🛠️ Languages and Tools used:
HTML5
CSS3
Sass
Git
GitHub
Terminal
Visual Studio Code

##### 💙 You can find me on:
LinkedIn Profile (link)

##### Thanks (+links)
To Colorlib for free templates.
To my mentor for creating the task and for the code review.

# DO USUNIĘCIA
SEKCJA NOTATEK - usuń po napisaniu README :)
funkcjonalności programu
problemy i ich rozwiązania + fragmenty kodu
fragment kodu

większy fragment kodu
materiały, które pomogły Ci uzyskać dany efekt
reużywalne części projektu
narzędzia, frameworki, biblioteki
niezbędne paczki i komendy do uruchomienia projektu
wtyczki – rozszerzenia do przeglądarki czy do IDE
inspiracje
wnioski, pomysły na rozwój projektu
 

Koniec sekcji notatek. Poniżej znajdziesz szablon właściwego README.
screen or GIF of your app

Project Name
See the live version of Project Name.

1-3 sentences about the project...

Main features:

one
two
three
 

🔗 See also
Are you interested in techonologyName and technologyName? See my other project Interesting Project Name.

🤔 Solutions provided in the project
one
 

two:
some example code

more code :)
 

three
Issue	Solution	
one	short code example	
two	short code example	
thre	short code example	
 

four - some shortcut Ctrl + C
 

five - example with a screenshot
what it is

 

💭 Conclusions for future projects
I would like to improve...

This is the first issue:
and this is a code example
This is the second issue:
and this is a code example
 

🙋‍♂️ Feel free to contact me
Write sth nice ;) Find me on...

 

👏 Thanks / Special thanks / Credits
Thanks to my Mentor - devmentor.pl – for providing me with this task and for code review.

# Prawa autorskie

Wszelkie prawa autorskie oraz pokrewne do szablonu i elementów wchodzacych w jego skład należą do [colorlib.com](https://colorlib.com).
Szablon i jego elementy mogą być wykorzystywane na zasadach zgodnych z [licencją](https://colorlib.com/wp/licence/).

