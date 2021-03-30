# Week 11B - Client-side web applications

## I. Overview & Agenda
 - Creating a PHP *proxy server*
 - Downloading and parsing web services (review)

<hr>

## II. Lecture Notes
 - [PHP Web Service Part V - creating a proxy server](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-php-web-service-5.md)
  - this reviews how to utilize a simple web API - http://www.boredapi.com - we'll create **bored-client.html** to download this data
  - we look at a web service that our client-side JavaScript is unable to download - http://shoutcloud.io - but it CAN be downloaded by a PHP script
  - thus we will create a PHP *proxy server* that will download the data from shoutcloud, and then send this data to our client application
  - this walks through the creation of **shout-proxy.php** and **shout-client.html**

<hr>

## III. HW Assignments

 - [PHP Web Service Part V - creating a proxy server#submission](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-php-web-service-5.md#submission)
 - [HW - Improved Giphy Web Service App](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-improved-gif-finder.md):
   - you already did the Giphy Finder HW (and a web service project) in IGME-230/235 - so this is an opportunity to review that exercise, and add to it. To help your review of the material, we recommend that you re-do the Giphy Finder HW "from scratch" - rather than download and reuse the code you handed in before

<hr>

## IV. Videos

- [PHP and Web Services-5: Building a PHP proxy server I. (11:21)](https://video.rit.edu/Watch/php-proxy-server-1)
- [PHP and Web Services-5: Building a PHP proxy server II. (12:40)](https://video.rit.edu/Watch/php-proxy-server-2)


<!--
# Week 11B - More About Web Services
-->

<!--
## I. Topics
- Creating a web service using PHP:
  - PHP Basics (from IGME-230) - [PHP Intro - About this PHP Tutorial Series](https://github.com/tonethar/IGME-230-Master/blob/master/notes/php-0.md)
  - Let's make our own JSON web service - [demo-php-web-service-json.md](https://github.com/tonethar/IGME-330-Master/blob/master/notes/demo-php-web-service-json.md)
    - we will learn how to download this data both by utilizing a JS console app with Node.js, and also with JS running in the browser
    - we will look at 2 techniques for getting around CORS restrictions:
      - setting the `Access-Control-Allow-Origin` HTTP response header
      - utilizing a *Proxy Server*
  - Let's make our own XML web service - [demo-php-web-service-xml.md](https://github.com/tonethar/IGME-330-Master/blob/master/notes/demo-php-web-service-xml.md)
  - ***Understanding JSON and cross-origin issues will really help you on project 2!***
-->

<!--
- The Google Maps API:
  - [HW-maps-1.md](https://github.com/tonethar/IGME-330-Master/blob/master/notes/HW-maps-1.md) - see mycourses dropbox for due date
  - The data files you will need are here - [map_data.zip](_files/map_data.zip)
  - https://www.impactmedia.co.uk/google-are-now-charging-for-using-google-maps/
  - Don't want to deal with Google Maps? Use the free Mapbox API on your HW instead - https://www.mapbox.com
  - Here's a little Mapbox demo we put together --> [mapbox-intro.md](https://github.com/tonethar/IGME-330-Master/blob/master/notes/mapbox-intro.md)
-->

<hr><hr>

| <-- Previous Unit | Home | Next Unit -->
| --- | --- | --- 
| [**week-11A-notes.md**](week-11A-notes.md)     |  [**IGME-330 Schedule**](../schedule.md) | [**week-12A-notes.md**](week-12A-notes.md)
