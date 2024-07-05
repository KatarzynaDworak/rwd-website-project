# Thanks for viewing my Project ✨

![ a main page screenshot](./images/screen.png)
<br />

## :star: Live Deployment: https://katarzynadworak.github.io/rwd-website-project/
<br />

## Main goal of my work was to:

- Develop a Visually Appealing Template: Create a high-quality, premium-looking template suitable for a wide range of web projects, focusing on aesthetics and modern design principles.
Ensure Full Responsiveness:

- Implement a fully responsive design that looks great on any device, including smartphones, tablets, laptops, and desktops.
Facilitate Easy Customization:

Provide a highly customizable template, allowing users to easily change colors, images, and sections to suit their specific needs.
Incorporate Smooth User Interactions:

Utilize CSS transitions and animations to enhance user interactions, ensuring a smooth and engaging experience.
Utilize Clean and Organized Code:

Follow the BEM (Block Element Modifier) methodology for writing clean, modular, and maintainable HTML and CSS code.
Apply Modern Design Techniques:

Use modern design techniques such as radial gradients, shadows, and flexible grid layouts to create an attractive and functional interface.
Ensure Cross-Browser Compatibility:

Implement CSS properties and techniques that are compatible across different browsers, ensuring a consistent user experience.
Integrate External Fonts and Icons:

Incorporate Google Fonts and custom icons to enhance the visual appeal and readability of the template.
Offer Various Pricing Plans:

Design a clear and attractive pricing section, presenting different plans to cater to various user needs.
Showcase the Team Behind the Project:

Include a section highlighting the team members, their roles, and social media links to add a personal touch and build credibility.
By achieving these objectives, I demonstrated the ability to create visually appealing, responsive, and user-friendly web interfaces while adhering to best practices in front-end development. This project showcases my commitment to delivering high-quality web solutions and continuous improvement in my development skills.
<br />

## Solutions provided in the project
**1.** I used in this project modern CSS functions like **min(), max(), and clamp()** to create a responsive and adaptive design. These functions help ensure that the layout and elements adjust smoothly across different screen sizes and resolutions.

- Responsiveness: Elements adjust dynamically to the screen size, providing a consistent and user-friendly experience across different devices.
- Maintainability: Using these functions even reduces the need for numerous media queries, simplifying the CSS code.
- Design Consistency: Ensures a consistent look and feel, regardless of the screen size, by setting appropriate limits on property values.
- This approach leverages the power of modern CSS to create a more efficient, scalable, and maintainable codebase.

Key Features:

**Clamp() Function:** ensures the margin values are responsive and stay within the defined minimum and maximum limits, adapting to different screen sizes.

    .header__logo {
    margin: clamp(15px, 2vw, 30px) 12px 12px clamp(10px, 2vw, 25px);
    padding: 2px;
    }

**Min() Function:** sets the font size to be responsive, choosing the smaller value between 4% of the viewport width and 15px, ensuring readability across devices.

    .nav__item {
        margin: 11px;
        font-size: min(4vw, 15px);
        position: relative;
        transition: font-weight 0.3s ease, letter-spacing 0.3s ease, transform 0.3s ease;
    }

**Max() Function:** ensures that the margin is at least 10px, but can grow to 2% of the viewport width, providing a flexible and responsive layout for different screen sizes.

    .benefits__img-1, .benefits__img-2, .benefits__img-3 {
        width: 115px;
        height: 115px;
        border-radius: 19px;
        margin: max(10px, 2vw) auto;
        padding: 33px;
    }

**2.** I used CSS code to provide a clean and **functional hamburger menu** that is hidden off-screen by default and smoothly slides into view when the associated checkbox is checked, providing an intuitive and responsive navigation experience for mobile users.

    .nav__menu {
        background-color: #2c2c2c;
        border-radius: 0 0 20px 20px;
        border-bottom: 2px solid #37ebed;
        display: block;
        padding: 20px;
        position: absolute;
        right: 0;
        text-align: center;
        transform: translateX(150%);
        transition: .4s linear;
        top: 100%;
        width: 100%;
        z-index: 1;
    }
      
    .header__input:checked ~ .nav__menu {
        display: block;
        transform: translateX(0%);
    }
      
    .header__hamburger {
        background-color: #f2f4f4;
        cursor: pointer;
        height: 3px;
        position: relative;
        width: 30px;
    }
      
    .header__hamburger::after {
        content: '';
        background-color: #f2f4f4;
        height: 3px;
        position: absolute;
        transform: translateY(-10px);
        width: 30px;
    }
      
    .header__hamburger::before {
        content: '';
        background-color: #f2f4f4;
        height: 3px;
        position: absolute;
        transform: translateY(10px);
        width: 30px;
    }
   
**3.** I also used **Grid** to provide flexibility to footer elements – they can be stretched in one row as well as arranged in two or one column.

<br />
<br />

## 🛠️ Languages and Tools used: 


<img align="left" alt="HTML5" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/html/html.png" />

<img align="left" alt="CSS3" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/css/css.png" />

<img align="left" alt="Git" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/git/git.png" />

<img align="left" alt="GitHub" width="50px" src="https://raw.githubusercontent.com/github/explore/78df643247d429f6cc873026c0622819ad797942/topics/github/github.png" />

<img align="left" alt="Terminal" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/terminal/terminal.png" />

<img align="left" alt="Visual Studio Code" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/visual-studio-code/visual-studio-code.png" />

<br />
<br />
<br />
<br />

## :blue_heart:  You can find me on:
<br/>

[<img align="left" alt="Mateusz Sowa LinkedIn" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/linkedin.svg" />](https://www.linkedin.com/in/katarzynadworakk/)

 
<br />

### Thanks
To Colorlib [colorlib.com](https://colorlib.com) for free templates.

To my Mentor - devmentor.pl – for creating the task and for the code review.

