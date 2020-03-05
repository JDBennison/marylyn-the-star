# Marilyn The Star

*Marilyn The Star* is an upcoming production at the Brighton Fringe following the life of Marilyn Monroe. This site was designed to sell the show and to inform about the cast and crew as well as informing the public where they can buy tickets and where to find the venue.

## UX

This website was designed for the theatre company who are putting on the show. They had a few requirements which I tried to bear in mind.

They wanted:
* a wesbite which looked professional which would sell the show
* information about the show displayed in a stylish format
* details about the cast and crew to act as a digital programme for the audience who do come to see the show

I decided that simplicity would work best for the company and so I put all the information on a one page layout with the navbar fixed to the top for quick access to everything.

[My initial mockup](assets/mockups/Marilyn.pdf) for desktop sites.

[My mobile mockup](assets/mockups/MarilynMobile.pdf) for mobile devices.

### User Stories
* As a person exploring the show for the first time I want information about the play close to the top to find out whether it is something I would be interested in.
* As someone who has decided to see the show I want a clear button to take me to booking infomation so I can see when the show is on and book tickets.
* As an audience member coming to see the show that day I want some easy to find directions to the venue so I know where to find it.
* As an audience member watching the show or a reviewer writing up about the show I want all the details about the cast and crew available so I can find out more about them and spell their names properly in the glowing reviews.
* As an audience member who has seen the show I want access to all their social media so that I can find out about future shows and other tours they may be doing in the future.

## Features

### Existing Features
#### Jumbotron

The main entrance to the site was designed to be very simple. One large image to give the audience an idea of the show and a link to the booking page.

#### About Page

As with the whole page I tried to keep this very simple and keep it to another striking image and the blurb which was written by the director.

In mobile view the text followed by the image doesnt work so below a certain screen size, it just becomes the text.

#### Cast and Crew 

As this would be acting as a digital programme for the show, I wanted to make sure each person had enough space and links to any personal social media that they wanted to promote. I found when I got the details back from each member of the cast that a lot of them did not have social media or did not want to promote it so I haven't got the links for every person.

I decided to use the Cards componant on Bootstrap as it is fairly flexible and if more people get involved in the production then I can easily add them on.

The cards have a hover feature which means that whilst at rest they are slightly opaque so you can see the image behind but when you hover over them they become solid and easier to read. I felt this wouldnt be functional on smaller screens so all the cards are solid at medium screens and below.

#### Bookings
I went through a few different options on how to display the dates before settling on this one which I arrived at after researching various other theatre websites. I feel that putting it in a table with the times being a link to the booking website would make it easier to read and would mean that I would be able to make the google maps plugin bigger and more prominent.

Currently all of the links in this section lead to the Brighton Fringe website as the tickets are not on sale at the Brighton Fringe box office or at the venue itself. When they are released I will update this and point it towards the actual venue website as the Brighton Fringe website incurs booking charges on the audience and the performers.


### Features Left to Implement
Other features which will be implemented or could be implimented in the future

#### Company/Venue information
Putting more details about the venue and the company to add more professionality to the webpage is a must which will be done relatively soon but is not crucial for the launch of the fringe programme.

#### Contact form
I would like to introduce a modal contact form for any other theatres to contact the company and invite them to perform. This will help the company to get further work.

#### Reviews
Once reviews start coming in, both audience reviews and industry reviews, I will create a section that will give quotes of the best lines and links to the full reviews. This will help to sell the show further.

#### Videos and Photos
Once the production gets closer to being released and they have more promotional materials I will put in another page to see production shots as well as a trailer and any other videos that they would like uploaded.

#### News and Updates
After May the dates will need to be updated as the company will hopefully be taking the show on to other fringes and other theatres. It might be possible to insert a news or blog page so that fans and audience can keep up to date with any exciting developments.

I would also like to update the bookings page so that the links change color when the performances are fully booked or when it has gone past that date but that is currently beyond my ability.

## Technologies Used
I have used mostly HTML5 and CSS3 to put together this site along with the following librarys and frameworks:

* [Bootstrap](https://getbootstrap.com/)
    * For basic formatting and layout.
    * v4.4.1

* [Font Awesome](https://fontawesome.com/)
    * For icons to social media.
    * Version 5.12.1 

* [Google Fonts](https://fonts.google.com/)
    * For the use of Roboto and Limelight.

* [JQuery](https://jquery.com/)
    * For the navbar dropdown.
    * v.3.4.1

## Testing

My first piece of testing involved the navbar. All of the links took me to the appropriate part of the page but I found that orginally, as it was transparent, it was hard to see the items on the navbar. I added a transparent background and this helped. However I found that upon first arriving at the site and navigating between the different sections using the links, the navbar would hang over some of the pictures or text which didnt look good. I added padding and a border to some of these elements to make sure the navbar had enough room.

On mobile view I realised that there was an alignment issue which meant that the logo and the hamburger were not on the same line. I realised that this was because of a line of code in the CSS called flex-wrap which only affected it upon smaller screens. After changing this it seemed to fix the problem.

The links throughout the pages all worked but the cast and crew cards needed a lot of testing. There were some alignment issues to begin with in regards to padding which meant some of the cards were dissapearing off the screen but this has been fixed. I've also reduced the borders so there is more room for text in each of the cards and there isnt a lot of empty space on mobile devices.

The biggest problem I discovered was that the images I used as the background have a fixed feature which means the text and cards scroll over it on desktop but on some mobile devices it can't handle this. I added some code which meant the image scrolls with the text on such devices. This created a different problem however. For the jumbotron the issue was solved however on the cast and crew section, as the section takes up more vertical space on mobile view, the background image was stretch so much you couldnt discern what it was at all. In this case I decided to make it swap to a plain dark background for mobile devices.

## Deployment

To deploy this onto GitHub Pages I went to settings, changed the source to 'master branch' and uploaded the page. I then bought the domain from GoDaddy and followed the following steps
1. On the DNS Management page I added the following
    * Four type A rows with these IP addresses
        1. 185.199.108.153
        2. 185.199.109.153
        3. 185.199.110.153
        4. 185.199.111.153
    * A CNAME row with "https://github.com/JDBennison"
2. On the github settings I then added my domain name which added a CNAME file to the document and connected up the domain.

To clone this project, follow these steps.
1. Click on [this link](https://github.com/JDBennison/marylyn-the-star).
2. Under the repository name, click Clone or download.
3. To clone the repository using HTTPS, under "Clone with HTTPS", click the copy button. 
4. Open Terminal.
5. Change the current working directory to the location where you want the cloned directory to be made.
6. Type git clone, and then paste the URL you copied in Step 3.
7. Press Enter. Your local clone will be created.

## Credits
### Content
The text in this website was written by Duncan Hopper and the biographies by the cast and crew themselves

### Media
The photos used in this site were taken specifically for the show by Miles Davies photography

### Acknowledgements
I received inspiration for this project from Towngate Theatre in regards to displaying the dates available for booking.