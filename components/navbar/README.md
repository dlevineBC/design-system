---
description: Navigation bars provide a list of links to important content on a website or application. Typically they are placed in the header.
title: Navigation Bar – Basic
status: Draft
author: orinevares
---

![Status](https://img.shields.io/badge/Component-Draft-orange.svg)

# Navigation Bar – Basic
Navigation bars provide a list of links to important areas on a website or application. Typically, they are placed by the header. 

## Required

## Last Updated:

## Visual

![Navbar](./images/navbar.gif)

## Requirements
* This component must be used according the the standard outined in this document. Any feedback should be directed to the feedback forum.

## Use This For
* Sites with six (6) or fewer navigation links or pages; sites with more links or with a hierarchy of pages should consider using a more advanced navigation structure.

## Don't Use This when
* Sites that have seven (7) or more navigation links, consider using a more advanced navigation structure.

## Design Protocol
* Present items in order of the users priority – higher demand links should be placed further to the left while lower demand links should be placed further to the right.

## Rationale
The B.C. government navigation bar provides a consistent look, feel, and functionality across government sites.

## Behaviour
1.	Link text appears underlined on hover
2.	Link text remains underlined and bolded when user is on the associated page
3.	The ‘hamburger icon’ should not appear on its own unless it has suitable Alternative text to ensure that It is recognizable by screen readers.”
4.	The menu should be full size on large screens and regular browsers. Smaller browers, including landscape tablets should use the collapsed version of the menu. The browser window is minimized to mobile view the navigation bar should appear as a hamburger dropdown menu.

## Accessibility
This component has been built according to [WCAG 2.0 AA](https://www.w3.org/TR/WCAG20/) standards and all government services should strive to meet this level.  This component successfully includes the following accessibility features:

### Screenreaders
* Proper ALT labels are included
* Language tag has been set to english
* List items are labelled properly
* Hamburger icon labelled properly

### Colour Contrast
* Contrast ratios are at least 7:1 for normal text and 4.5:1 for large text

### Keyboard Navigation
* Supports tab navigation for use without a mouse

### Learn More
* Contacts
* Online Tools
* Online Resources
* Gov Resources

## Prototype with This Component
Download and use the B.C. government Design System library to help build prototypes and wireframes for your website or application.

The library is constantly updated and currently available in the following tools:

*	[Sketch](https://sketch.cloud/s/Q0bkG)
* [UxPin and others]

## Code
### HTML

This component builds on the `header` component; See `sample.html` for a working example.

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8"/>
    <meta http-equiv="x-ua-compatible" content="ie=edge"/>
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no"/> 
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.5.0/css/all.css" integrity="sha384-B4dIYHKNBt8Bc12p+WXckhzcICo0wtJAoU8YZTY5qE0Id1GSseTk6S+L3BlXeVIU" crossorigin="anonymous">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/css/bootstrap-reboot.min.css">
    <link href="https://fonts.googleapis.com/css?family=Noto+Sans" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
    <title>Sample Navigation</title>
</head>

<!--
  All in-line CSS is specific to this sample; it can and should be ignored.
 -->

<body style="background: #F8F8F8; margin-top: 130px;">
  <header>
    <div class="banner">
        <a href="https://gov.bc.ca" alt="Go to the Government of British Columbia website">
          <img src="../assets/images/logo-banner.png" alt="Go to the Government of British Columbia website" />
        </a>
        <h1>Hello British Columbia</h1>
    </div>
    <div class="other">
      <a class="nav-btn">
        <i class="fas fa-bars" id="menu"></i>
      </a>
    <!-- 
      This place is for anything that needs to be right aligned
      beside the logo.
    -->
    </div>
  </header>
  <nav class="navigation-main" id="navbar">
    <div class="container">
      <ul>
        <li><a href="sample.html" class="active">Home</a></li>
        <li><a href=".">Some Thing</a></li>
        <li><a href=".">Another Thing</a></li>
        <li><a href=".">Somewhere</a></li>
        <li><a href=".">Elsewhere</a></li>
        <li><a href=".">Hello</a></li>
      </ul>
    </div>
  </nav>
  <p style="margin-left: 25px; margin-right: 25px;">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus quis elementum mauris. Pellentesque non velit id quam placerat laoreet. Ut tempus velit eget lorem maximus, quis hendrerit erat vestibulum. Nulla blandit, enim id pulvinar lacinia, augue magna pretium sapien, quis venenatis ligula tellus a enim. Aenean elementum sagittis dolor, eget blandit ante porttitor sed. Nunc maximus lorem et tellus tincidunt, eget tincidunt libero hendrerit. Suspendisse in feugiat magna, sit amet eleifend lacus. In mi lacus, viverra ac mi ac, tincidunt vestibulum mi. Donec in tempor urna, a pharetra lectus. Pellentesque a vestibulum diam. Etiam ullamcorper viverra pulvinar. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Nulla vel venenatis velit, vel dictum sapien. Donec sed ante malesuada, sagittis metus vitae, placerat metus.
  </p><p style="margin-left: 25px; margin-right: 25px;">
    Mauris lacinia, mauris in molestie interdum, sapien lacus cursus libero, ut scelerisque arcu dui id orci. Morbi ac eros id augue consequat lacinia in id lorem. Nam sed est vitae sapien lacinia facilisis. Vestibulum euismod, dui eu fringilla consectetur, ante nisl dapibus risus, id posuere erat mi rutrum urna. Cras erat tortor, congue quis volutpat ac, pellentesque a sapien. Sed pretium sapien ac lobortis lacinia. Morbi dui risus, suscipit congue fringilla vel, interdum pulvinar arcu. Pellentesque et tellus vel mauris gravida commodo eu ut dui. Donec risus magna, feugiat nec ex in, sagittis commodo mauris.
  </p><p style="margin-left: 25px; margin-right: 25px;">
    Nunc in nisi pretium, cursus ante a, commodo nibh. Nullam sed dignissim augue. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Duis non laoreet justo. Nunc tempus neque eget condimentum sagittis. Nunc lacinia nisi nibh, eget euismod lectus viverra ac. Vivamus rutrum mi id nisi dictum convallis.
  </p><p style="margin-left: 25px; margin-right: 25px;">
    Suspendisse convallis odio sed risus vehicula auctor. Integer et vulputate mi. Donec dictum velit ut mollis ultricies. Fusce semper, nisi vel sagittis interdum, lorem libero tristique magna, eget hendrerit ipsum elit sed justo. Aliquam accumsan tempus arcu ut rutrum. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras malesuada est at risus fermentum, ac molestie quam porta. Vivamus eros lorem, facilisis at ornare sit amet, placerat in sapien. Aenean ut tellus non nunc aliquet finibus et at ligula. In laoreet euismod purus, lacinia feugiat nibh porta eu.
  </p><p style="margin-left: 25px; margin-right: 25px;">
    Donec venenatis mattis erat ut semper. Aenean id nisl accumsan, tempus enim quis, accumsan lectus. Vivamus rutrum egestas quam, ut lobortis nibh tristique id. Etiam gravida at metus quis egestas. Curabitur ultricies a ipsum ut lacinia. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Phasellus suscipit metus urna, ut auctor risus imperdiet vitae. Etiam in mollis est. Nulla ultricies lectus nisl, vitae fringilla nisl venenatis non. Vivamus tincidunt cursus purus et facilisis.
  </p><p style="margin-left: 25px; margin-right: 25px;">
    Donec ac dui ex. Nulla est leo, vehicula vel hendrerit vel, ornare id erat. Mauris eget dignissim erat, sit amet pretium enim. Donec tincidunt dolor vitae libero ullamcorper molestie. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec lacinia hendrerit dapibus. Maecenas mollis lorem sit amet facilisis feugiat. Sed faucibus lectus et blandit dictum. Mauris augue purus, placerat quis fermentum et, ullamcorper sit amet felis. Vivamus at ultricies odio, ac condimentum diam. Praesent faucibus quis tellus et maximus.
  </p><p style="margin-left: 25px; margin-right: 25px;">
    Donec accumsan tincidunt neque, non interdum eros venenatis eget. Phasellus condimentum convallis purus, a gravida diam dignissim nec. Nulla convallis magna ut ligula luctus, at ultricies nisi lacinia. Nullam ornare sodales lobortis. Suspendisse mattis commodo felis, id tempus risus dapibus ac. Phasellus non hendrerit dolor. Integer ac arcu at elit tempus condimentum non sed metus. Nunc egestas eros non imperdiet accumsan. Sed molestie tortor in imperdiet ornare. Vivamus malesuada blandit augue, ut euismod nisi mollis molestie. Phasellus porttitor ex non nulla commodo, sit amet efficitur nisi lacinia.
  </p><p style="margin-left: 25px; margin-right: 25px;">
    Sed consectetur egestas lectus sed hendrerit. Donec molestie orci quis erat scelerisque aliquet. Sed auctor maximus feugiat. Proin mollis, risus at dapibus dapibus, dolor metus volutpat sapien, sed condimentum magna turpis non purus. Pellentesque auctor felis eget rhoncus pellentesque. Sed neque enim, imperdiet vitae egestas placerat, commodo sed mauris. Etiam egestas lacus ac ex commodo laoreet. Suspendisse sed augue vitae ex elementum hendrerit. Pellentesque ullamcorper facilisis augue, ut lacinia ipsum consectetur sit amet. Aenean eget diam ac neque scelerisque placerat.
  </p>

  <script>
    function setupSampleMenuControl() {
      const useCapture = false;
      const show = elem => elem.style.display = 'block';
      const hide = elem => elem.style.display = 'none';
      const toggle = (elem) => {
        if (window.getComputedStyle(elem).display === 'block') {
          hide(elem);
          return;
        }
        show(elem);
      };
      // Listen for click events
      const menuButton = document.getElementById('menu');
      menuButton.addEventListener('click', (event) => {
        // Filter events
        if (event.target.id !== 'menu') return;
        // Prevent default link behavior
        event.preventDefault();
        // Check for a valid target
        const nav = document.getElementById('navbar')
        if (!nav) return;
        // Toggle
        toggle(nav);
      }, useCapture);
    }
    setupSampleMenuControl();
  </script>

</body>
</html>
```

### CSS

This component builds on the `header` component; See `style.css` for a working example.

```css
header {
    background-color: #036;
    border-bottom: 2px solid #fcba19;
    padding: 0 30px 0 30px;
    color: #fff;
    display: flex;
    height: 65px;
    top: 0;
    position: fixed;
    width: 100%;
    -webkit-box-shadow: 0 6px 8px -4px #b3b1b3;
    -moz-box-shadow: 0 6px 8px -4px #b3b1b3;
    box-shadow: 0 6px 8px -4px #b3b1b3;
  }
  
  header h1 {
    font-family: 'Noto Sans','Calibri', 'Arial', 'Sans Serif';
    font-weight: normal;  /* 400 */
    margin: 5px 5px 0 18px;
    visibility: hidden;
  }
  
  header .banner {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    margin: 0 10px 0 0;
    /* border-style: dotted;
    border-width: 1px;
    border-color: lightgrey; */
  }
  
  header .other {
    display: flex;
    align-items: center;
    flex-grow: 1;
    /* border-style: dotted;
    border-width: 1px;
    border-color: lightgrey; */
  }

  header a [class^="fas fa-"] {
    color: white;
    font-size: 1.4em;
    font-style: bold;
    line-height: 1;
    /* border-style: solid;
    border-width: 1px;
    border-color: #fcba19; */
    padding: 5px;
    -webkit-font-smoothing: antialiased;
  }
  
  header .nav-btn {
    display: block;
    width: auto;
    margin: 0 0 0 auto;
    cursor: pointer;
  }

  .navigation-main {
    display: none;
    position: fixed;
    top: 65px;
    color: #fcba19;
    background-color: #38598a;
    width: 100%;
    -webkit-box-shadow: 0 6px 8px -4px #b3b1b3;
    -moz-box-shadow: 0 6px 8px -4px #b3b1b3;
    box-shadow: 0 6px 8px -4px #b3b1b3;
  }

  .navigation-main .container {
    padding: 10px 0 10px 0;
  }
  
  .navigation-main .container ul {
    display: flex;
    flex-direction: column;
    margin: 0;
    color: #fff;
    list-style: none;
    margin-left: -25px;
    /* border-style: dotted;
    border-width: 1px;
    border-color: red; */
  }

  .navigation-main .container ul li {
    margin: 5px 0;
  }

  .navigation-main .container ul li a {
    display: flex;
    font-size: 0.813em;
    font-weight: normal;  /* 400 */
    color: #fff;
    padding: 0 15px 0 15px;
    text-decoration: none;
    /* border-style: dotted;
    border-width: 1px;
    border-color: green; */
  }

  .navigation-main .container ul li a:hover {
    text-decoration: underline;
  }

  .navigation-main .container ul .active {
    text-decoration: underline;
    font-weight: bold;
  } 

  /*
    These are sample media queries only. Media queries are quite subjective
    but, in general, should be made for the three different classes of screen
    size: phone, tablet, full. 
  */
  
  @media screen and (min-width: 768px) {
    .navigation-main {
      display: block;
    }

    .navigation-main .container ul {
      flex-direction: row;
    }

    .navigation-main .container ul li {
      margin: 0;
    }
    
    .navigation-main .container ul li a {
      border-right: 1px solid #9b9b9b;
    }

    header .nav-btn {
      display: none;
      width: auto;
      margin: 0 0 0 auto;
      cursor: pointer;
    }
  }

  @media screen and (min-width: 768px) and (max-width: 899px) {
    header h1 {
      font-size: calc(7px + 2.2vw);
      visibility: visible;
    }
  }
  
  @media screen and (min-width: 900px) {
    header h1 {
      font-size: 2.0em;
      visibility: visible;
    }
  }
```

### Assets
  Assets go here
