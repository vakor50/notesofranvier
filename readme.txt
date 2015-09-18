The main files you will need to look at are:
 - index.html
 - about.html
 - members.html
 - media.html
 - contact.html **
 - css/style.css

--------------------------------------------------------------------

Each .html file has basically the same first 79 lines
the <head> tags set the text of the tab, and link to resource files

the css files are style sheets that make the page pretty basically

inside the body, there is a <nav> tag which is what makes the menu bar at the top
 of the padding-left

to create more tags on the left side of the menu bar, go to line 39
  paste in another <li> element of the same structure. If you want the tag to
  appear to be selected, the tag should look like this: <li class="active">

to add links to the media dropdown
  paste in another <li> of the same structure as in line 45
  make sure you change the destination of the new link

to create more tags on the right side of the menu bar, go to line 54
  these li have links to social media icons
  each has an <a> tag that wraps the image
  (they all have the class btn-facebook because that class is styled to not have color)
  to change the icon, modify the <i> tag
      <i class="fa fa-____">
      fill in the blank with whatever icon you want
      icons can be found at http://fontawesome.io/icons/
  to change the link from the tag, change the href attribute

each .html file also has a footer at the end of the page
<div id="footer">
  <div class="container">
    <p class="text-muted">© Notes of Ranvier 2015 | Designed by Vir Thakor</p>
  </div>
</div>

--------------------------------------------------------------------

index.html
This is the home page. When someone opens the site this is the page that loads
to add images the the carousel
    add another <li> with a different number to the "Indicators" at linke 94
    add another <div class="item"> to the "Wrapper for slides" starting at line 102
    make sure each image has a height to width ration such that: 2 * height = width

to change the content after the carousel
  change anything you see fit going on after <div class="container"> in line 138

--------------------------------------------------------------------

about.html
there are two boxes, where you can write whatever content you want
  <div class="col-md-7 about-desc"> line 93
  <div class="col-md-4 about-supp"> line 97

starting at line 104, there is a short description and link to to Media

--------------------------------------------------------------------

memebers.html
starting at line 81, we have content for each memeber of the team
each person is structured the same
    <div class="col-xs-6 col-lg-4">
      <img class="img-circle" src="img/chris.jpg" alt="Sabrina Palazzolo" width="140" height="140">
      <h3>Sabrina Palazzolo</h3>
      <p>Publicity Chair</h3>
      <p>Alto - Class of 2018</p>
      <p><a class="btn btn-default" href="#" role="button">View details »</a></p>
    </div>

    <img>
      src="__"  == the location of the image of the person (make sure each image is a square)
      alt="__"  == the text to be displayed if the image doesn't load properly
    <h3>__</h3>  == the name of the member
    <p>__</p>  == optional: position
    <p>__</p>  == vocal range and expected graduation year
    <p><a ...>  == link to more details on the person
      delete if you want
      change href="__" to link to any info about the person

--------------------------------------------------------------------

media.html
to add another youtube link, follow this format and add into <div id="page-wrap"> on line 104

<div id="top-space">
  <a id="media1"></a>
  <hr>
</div>

<div id="page1">
  <div id="content-wrap">
    <h4>Shake It Out / Blank Space</h4>
    <!-- 16:9 aspect ratio -->
    <div class="embed-responsive embed-responsive-16by9">
      <iframe class="embed-responsive-item" width="560" height="315" src="https://www.youtube.com/embed/L7VsuRLzCxg" frameborder="0" allowfullscreen></iframe>
    </div>
    <div class="desc">
      <p>Opb. Florence + the Machine / Taylor Swift </p>
      <p>Soloists: Sara Shah '17 and Sabrina Palazzolo '18 </p>
      <p>Arranged by Sara Shah '17 and Chris Le '17 </p>
    </div>
  </div>
</div>

make sure you change
 - the numbers
 - the src
 - the links in the header for each .html file
 - the links on the about page
