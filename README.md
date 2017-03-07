# popup-video
When it comes to content, video is king. It is the most consumed content on the web. If you had to choose from a range of media types to get a message across, a video should always be your first consideration. Visual communication is the top tier form of getting your messaging to stick. While graphics and copy can make the difference between a website visit and a sale, video can go even further. Why not have the best of both worlds?  

Simply making your hero a video or designing your hero with a graphic overlayed with some copy is the typical approach to homepage hero sections. There is a way to have both and it involves Magnific Popup, a jQuery plugin that displays content when an HTML element is clicked. In our example, the hero image and overlaying copy is still prominent. Our Call-to-Action (CTA), however, is a button. This button does not simply take them to another page with more copy and graphics, it opens a popup video. In this scenario, you can maintain your hero image and overlaying text and provide the option for website visitors to view a video further describing your product or service.

## Tutorials

For detailed instructions, view Solodev's [Adding a Popup Video to your Hero Image](https://www.solodev.com/blog/web-design/adding-a-popup-video-to-your-hero-image.stml) article.

## Demo

Try out a working example on [JSFiddle](https://jsfiddle.net/solodev/u43vsyzu/).

## HTML

The hero image with a popup video contains the following HTML markup.

```
<div class="content">
   <h1><span>INTRODUCING</span>
      WebCorpCo 2 . 0
   </h1>
   <a href="#videoStory" class="button more" id="videoLink">Watch Video<i class="fa fa-play-circle" aria-hidden="true">&nbsp;</i></a>
   <div id="videoStory" class="mfp-hide" style="max-width: 75%; margin: 0 auto;">
      <iframe width="853" height="480" src="https://www.youtube.com/embed/oXoe3GWygq0?rel=0" frameborder="0" allowfullscreen></iframe>
   </div>
</div>
```
## CSS

All required CSS is contained in popup-video.css

## JavaScript

This tutorial utilizes the JavaScript below.

```
$('#videoLink')
.magnificPopup({
          type:'inline',
          midClick: true // Allow opening popup on middle mouse click. Always set it to true if you don't provide alternative source in href.
})
```

## External Includes

This tutorial includes the following third party resources.

```
<link href="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.0.0/magnific-popup.min.css" rel="stylesheet">
<link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
<link href="popup-video.css" rel="stylesheet">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.0.0/jquery.magnific-popup.min.js"></script>
```
