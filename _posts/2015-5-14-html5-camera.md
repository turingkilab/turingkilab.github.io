---
layout: post
title:  "Using HTML5 and little JavaScript code to display the camera videos"
date:   2015-05-14 14:34:33
categories: HTML5
---
##Display
<script type="text/javascript" src = "{{site.baseurl}}/public/js/photobooth_min.js"></script>
<div id="example" style="width: 470px; height: 300px;"></div>
<div id="gallery"></div>
 
 
<script type="text/javascript">
$(function(){

    $( '#example' ).photobooth().on( "image", function( event, dataUrl ){
        $( "#gallery" ).show().html( '<img src="' + dataUrl + '" >');
    });

});
 </script>

 