# Thanks for viewing my Project ✨

## ⭐ Live Deployment: (link - github pages)

### Main goal of my work was to:
- code **Responsive Web Design (RWD)** site 📱
- do it in a way that it **looks decent on mobiles, tablets and desktops** 🖥️
- use **semantic HTML** (BEM) 📝
- use **Sass** 🦋
- make project **as readable as it is possible** (clean code, many directories, BEM, small sass files) 📖

#### Solutions provided in the project
- CSS file created with node-sass library.

- Sass mixins used to define breakpoints – having all breakpoints in one place makes it possible to change them at any time, all at once. See the example of - mixin for desktop breakpoint beneath:

@mixin desktop {
	@media (min-width: 1330px) {
		@content;
	}
}
- Responsive font size created with CSS function: clamp(). Using vw unit for the middle parameter value makes the font grow and shrink smoothly while resolution changes. As clamp() is not fully supported yet, it was necessary to provide also the media queries breakpoints. Here is the example of using both - mixins and clamp():
  
&__headline {
		font-size: 1.3rem;
	@include tablet-and-landscape {
		font-size: 1.5rem;
	}
	@include desktop{
		font-size: 1.7rem;
	}
	@supports (font-size: clamp(1.3rem, 2vw, 1.7rem)) {
		font-size: clamp(1.3rem, 2vw, 1.7rem);
	}}
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
 

💡 Technologies
HTML5 CSS3 JavaScript

 

🔗 See also
Are you interested in techonologyName and technologyName? See my other project Interesting Project Name.

 

💿 Installation
The project uses node and npm. Having them installed, type into the terminal: npm i.

 

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






> ⭐ ***README** to coś więcej niż opis. Poprzez nie **pokazujesz swoje mocne strony** – swoją dokładność, sposób myślenia i podejście do rozwiązywania problemów. Niech Twoje README pokaże, że masz **świetne predyspozycje do rozwoju!***
> 
> 🎁 *Zacznij od razu. Skorzystaj z **[szablonu README i wskazówek](https://github.com/devmentor-pl/readme-template)**.* 

&nbsp;



# HTML & CSS: Responsywność (RWD)

Czas zakodować stronę, która ma przygotowane 3 widoki dla różnych punktów granicznych (ang. breakpoints):

- mobile
- tablet
- desktop.

## Od czego zacząć?

Przeczytaj dokładnie treść, którą zamieszczam poniżej. Następnie zapoznaj się ze zrzutami ekranu prezentującymi poszczególne widoki – znajdziesz je w katalogu `./assets`.

Na każdym widoku zaznacz sobie, które elementy to oddzielne sekcje strony. Zwróć uwagę, jak się one zmieniają podczas przechodzenia z jednego widoku do drugiego. To ułatwi Ci zaplanowanie układu.

Zacznij od **widoku na telefon**. Możesz użyć [PerfectPixela](https://chrome.google.com/webstore/detail/perfectpixel-by-welldonec/dkaagdgjmgdmbnecmcefdhjekcoceebi?hl=pl) – dodatku do przeglądarki Chrome – aby ułatwić sobie kodowanie. Pamiętaj, że nie warto odzwierciedlać projektu 1:1 co do piksela. Masz zaznajomić się z technikami RWD i przy okazji utrwalić wiedzę z HTML-a i CSS-a. Widok ma być podobny do pierwowzoru: zachować koncepcję i estetykę oraz dopasowanie do najważniejszych rozdzielczości. Nie ma być identyczny, a w zasadzie nie może być, ponieważ na każdym urządzeniu z inną rozdzielczością będzie się prezentował trochę inaczej.

Jeśli będziesz korzystać z PerfectPixela, pamiętaj o ustawieniu prawidłowej skali dla podglądu obrazu oraz ustawienia odpowiedniej szerokości dla okna przeglądarki.

Możesz również skorzystać z dodatku [ColorZilla](https://chrome.google.com/webstore/detail/colorzilla/bhlhnicpbhignbdhedgjhgdocnmhomnp), dzięki któremu pobierzesz kolor ze wskazanego miejsca. Wystarczy wyświetlić obraz w przeglądarce Chrome i użyć tego rozszerzenia. 

Kiedy skończysz kodować widok dla telefonu, zajmij się **widokiem tabletowym**. Pamiętaj, aby sprawdzać, czy zmiany wprowadzone do widoku tabletowego nie spowodowały zmian w widoku mobilnym.

Po skończeniu kodowania widoku dla tabletu zajmij się **desktopem**. Ponownie pamiętaj o częstym sprawdzaniu, czy czegoś nie popsułeś w poprzednich wersjach. Im wcześniej się zorientujesz, że coś nie działa, tym łatwiej będzie Ci to naprawić.

## Zasoby

### Fonty

Font wykorzystywany w projekcie to `Poppins`. Znajdziesz go w [Google Fonts](https://fonts.google.com/specimen/Poppins).

### Obrazy

Wszystkie niezbędne obrazy, w tym kształty, znajdziesz w katalogu `./images`. 

### Ikony

Ikony mediów społecznościowych znajdujące się w stopce stwórz przy pomocy [Font Awesome](https://fontawesome.com/).


## Widoki

Nie podaję dokładnych punktów granicznych, abyś sam mógł ocenić, kiedy zrobić przejście.

Zamieszczam tylko informację, dla jakich rozdzielczości był robiony przedstawiony zrzut ekranu:

 - mobile => 600px
 - tablet => 900px
 - desktop => 1200px

### mobile => 600px

![](./assets/mobile.png)

### tablet => 900px

![](./assets/tablet.png)

### desktop => 1200px

![](./assets/desktop.png)

# Zadanie dodatkowe

Najwyższy czas zaprezentować swoje umiejętności znajomym na Facebooku czy Instagramie! Być może właśnie w ten sposób zdobędziesz swoje pierwsze zlecenie – poważnie! Osoby, które Cię znają, są w stanie bardziej zaufać Tobie niż komuś „z ulicy”. Dzięki temu zdobędziesz, tak ważne przy rekrutacji, doświadczenie komercyjne.

## GitHub Pages

GitHub udostępnia funkcjonalność, która nazywa się [GitHub Pages](https://pages.github.com/). W ten sposób możemy „serwować” naszą stronę całkowicie za darmo na podstawie zawartości naszego repozytorium. Możliwość ta dotyczy jedynie stron statycznych korzystających z HTML-a, CSS-a i JavaScriptu – więc również z Reacta. 

Wystarczy, że przejdziesz do [ustawień (Settings) swojego repozytorium](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#choosing-a-publishing-source) i wybierzesz gałąź (branch), która zawiera pliki strony (pewnie będzie to `master` lub `main`). Po minucie czy dwóch strona powinna być już dostępna.

Potrzebujesz szczegółowych instrukcji lub Twoja strona nie działa? Poszukaj wskazówek w moim artykule: [GitHub Pages – podgląd projektu na GitHubie](https://devmentor.pl/b/github-pages-podglad-projektu-na-githubie).

> **Uwaga!** Czasami nawet GitHub ma problemy z własnymi serwerami/usługami i coś może nie działać, jak należy. Wtedy wystarczy sprawdzić „status” na [tej stronie](https://www.githubstatus.com/). Tego typu rozwiązanie jest dość powszechne.

## Własna domena

Mile widziana (a już na pewno, gdy znajdziesz klienta) będzie własna domena. Na szczęście GitHub Pages daje możliwość jej podpięcia.

Koszt domeny to zaledwie kilkanaście złotych w pierwszym roku, a jej przedłużenie na kolejny rok to zazwyczaj mniej niż 99 zł (zależnie od końcówki). Taką domenę możesz kupić np. w [seohost.pl](https://seohost.pl/?ref=22965).

> **Uwaga!** Nieuczciwe firmy oferują domeny w bardzo atrakcyjnych cenach za pierwszy rok, ale nadrabiają to kosztem przedłużenia, które musisz wykonać, jeśli chcesz zatrzymać domenę. Przeczytaj dokładnie regulamin, zanim dokonasz zakupu.

Domena to nazwa wskazująca na konkretny serwer, na którym znajdują się pliki naszej strony internetowej. Wskazanie to jest realizowane przez [DNS](https://pl.wikipedia.org/wiki/Domain_Name_System).

Jak przeczytamy w [dokumentacji GitHub Pages](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site#configuring-a-subdomain), możemy użyć [domeny](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain) lub [subdomeny](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site#configuring-a-subdomain) (jeśli kupimy np. domenę devmentor.pl, to jej subdomeną będzie np. rwd.devmentor.pl). Aby to zrobić, musimy dodać odpowiedni rekord w ustawieniach DNS. Sposób wykonania tego zadania zależy od dostawcy domeny i jego panelu administracyjnego. W seohost możesz to zrobić w [taki sposób](https://seohost.pl/pomoc/konfiguracja-rekordow-dns-domeny). Jeśli sobie nie poradzisz, to support (pomoc techniczna) na pewno Ci pomoże. Zawsze byli dla mnie pomocni.

> **Uwaga!** Dokonanie zmian w DNS (propagacja informacji) może trwać nawet 24 h (często jednak strona działa już po paru godzinach), dlatego wygodnie jest to robić wieczorem, aby rano mieć już sprawę załatwioną.

# Prawa autorskie

Wszelkie prawa autorskie oraz pokrewne do szablonu i elementów wchodzacych w jego skład należą do [colorlib.com](https://colorlib.com).
Szablon i jego elementy mogą być wykorzystywane na zasadach zgodnych z [licencją](https://colorlib.com/wp/licence/).



&nbsp;

> ⭐ ***README** to coś więcej niż opis. Poprzez nie **pokazujesz swoje mocne strony** – swoją dokładność, sposób myślenia i podejście do rozwiązywania problemów. Niech Twoje README pokaże, że masz **świetne predyspozycje do rozwoju!***
> 
> 🎁 *Zacznij od razu. Skorzystaj z **[szablonu README i wskazówek](https://github.com/devmentor-pl/readme-template)**.* 
