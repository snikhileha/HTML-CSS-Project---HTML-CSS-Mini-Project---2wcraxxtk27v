
# University Website Design

This project designed with HTML, CSS. This project has multiple html pages linked via navigation menu. You can explore following pages Home, About, Course, Contact. As this web app is responsive hence user could access it via mobile as well.

## Features

- Navigation menu to navigate over different pages.
- Responsive website.
- Javascript function to toggle menu in mobile view.
- Bootstrap-CDN to use icons.
- Beautiful hover on images, paragraphs and details etc.


## Tech Stack

**Client:** HTML, CSS, JAVASCRIPT


## Lets Explore More Here :

- ### Navigation Menu :
    The navigation menu you can see on the top right 
    corner of the every page like Home, About, Course and
    Contact. You can jump to any page from any page. Once you
    hover a mouse on any menu option it will get hover by
    just getting underline to it.

    A common HTML and CSS code is used to see these navigation
    menu on each page.
    Just replace the class = "header" with "sub-header" for all pages other than Home.html    

            
        <section class="header">    <!-- Header : Home page -->
            <nav>   <!-- The nav tag shows multipages links on the top right position -->
                
                <a href="./index.html"><img src="./images/logo.png" alt=""></a> <!-- Show logo of "Eduford on top 
                    left corner "-->
                
                <div class="nav-links" id="navLinks"> <!-- div container with id "navLinks",
                     to perform open and close menu in responsive window-->
                    
                     <i class="fa-solid fa-xmark" onclick="hideMenu()"></i> <!-- In responsive window  upon clicking
                         this icon will used to close menu -->
                    <ul>    <!-- List of horizontal (vertically right in responsive window) -->
                        <li><a href="index.html">HOME</a></li>
                        <li><a href="about.html">ABOUT</a></li>
                        <li><a href="course.html">COURSE</a></li>
                        <li><a href="contact.html">CONTACT</a></li>
                    </ul>
                </div>
                <i class="fa-solid fa-ellipsis-vertical" onclick="showMenu()"></i> <!-- In responsive window upon clicking
                    this icon will used to show menu -->
            </nav>

            <div class="text-box">  <!-- div container for Home page highlights -->
                <h1>Worlds Biggest University</h1>
                <p>Making website is now one of the easiest thing in the world. You 
                    jsut need to learn HTML, CSS, <br>Javascript and you are good to go.
                </p>
                <a href="" class="hero-btn">Visit Us To Know More</a>
            </div>

        </section>   <!-- End of Header : Home page -->

    - ### Footer :
        The footer includes the developer's information and its connection links to social media.
        THis footer information will also available on all pages.

    - ### Home : 
        You can see all the highlights about the app on the home page.
        This includes information about Course, About us and Contact.
        The course and campus details are beautifully shown with hover effects.
        You could see details of it in the "Course".

    - ### About :
        To know all about the University you can get here. The deatils are given here in brief but you can 
        explore more by just clicking "Explore Now".
        The image and details are in the "div" tag are managed in parallel
        using CSS display : flex.

    - ### Course :
        The University offers different courses like Intermediate, Degree, Post Graduation.
        These three courses shown in the UI in the block. When you focus on any 
        one of them that block will get hover and the background color will change.
        Also you can see facilities provided with images.

    - ### Contact :
        Provided a map to reachout at the location. This job is done by using iframe with google map location in a section.
        After that you can see the contact details of the university and a form is provided to send your queries.
    
    - ### media queries :
        The media queries are used to make this website fully responsive.
        You could use it in you mobile browser as well.

    #        
        @media(max-width: 700px) {
        .text-box h1 {
            font-size: 20px;
        }
        .nav-links ul li {
            display: block;
        }
        .nav-links {
            position: absolute;
            background: #f44336;
            height: 100vh;
            width: 200px;
            top: 0;
            right: -200px;
            text-align: left;
            z-index: 2;
            transition: 1s;
        }
        
        nav .fa-solid {
            display: block;
            color:#fff;
            margin: 12px;
            font-size: 22px;
            cursor: pointer;
            background: transparent;
        }

            .nav-links ul {
                padding: 30px;
            } 
        }
        
    - ### Javascript :
    The below code does toggle between navigation menu in the mobile responsive window.
        #
        var navLinks = document.getElementById("navLinks");

            function showMenu() {
                navLinks.style.right = "0";
            }
            function hideMenu() {
                navLinks.style.right = "-200px";
            }

## Feedback

If you have any feedback, please reach out to us at snehajoshi1895@gmail.com

