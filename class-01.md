Class One - Reading Assignment
Ken Lindsay

So, here's what we covered:

HTML   1: Structure
HTML   8: Extra Markup
HTML  17: HTML5 Layout
HTML  18: Process & Design

JS Intro
JS     1: The ABC of Programming.

With the lead up to our first class on 12FEB2022, we reviewed the fundamentals of HTML for generating a simple webpage and the use of CSS and Javascript to enable enhance functionality. Our initial assignment was to design a simple webpage, making use of basic functions to help with design and layout. I decided to make a website for a meal delivery service 'The Crabby Chef', as I have been learning a lot about dietary requirements of various friends and their journey in meal preparation. Another aspect of the assignment was to make use of alert() functions to prompt questions from the user and record their answers. I decided to bundle this up into a website asking a series of dietary questions and recording those answers for the final response, tying it all together.

The most challenging aspect, to me, was... getting what I wanted. I wanted to created a simple page with 3 images lined up next to each other. Simple, no? No. For this, I had two options: complicated HTML OR CSS. Wanting to understand CSS, I did a little digging into what it is and why I needed it. CSS, provides some great control of design and layout of webpage attributes. In reviewing several sources on CSS, I found that one could introduce tables (columns, rows, etc.) and by placing my images within, all I needed was 1 row, with 3 columns, and to specify the attributes (or images) of those cells, with CSS. the resulting code below, is what I included in the head section of my HTML.

CSS
    <head>
        <meta charset = "UTF-8">
        <title style = "font-size: 4rem;"> The Crabby Chef.</title>
        <style>
        main {
            color: rgb(5, 5, 5)
        }
        body { 
        background-color: rgb(15, 184, 206);
        }
        .column {
                float: left;
                width: 33.33%;
                padding: 5px;
            }
            .row::after {
                content: "";
                clear: both;
                display: table;
            }
        </style>
    </head>

The key to making the images equally sized, was to alter the width parameter to take up a third of the space (for three images).
With this in place, everything was layed out with equal sizing and spacing. While I know things can get more complicated with webpages. I felt this was a great start and I began to see CSS as a powerful tool rather than a necessary hassel.
-KL