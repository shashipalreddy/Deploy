# Deploy
## How to deploy MVC Application into IIS step-by-step process

1. [link](https://www.youtube.com/watch?v=PPaqVyBkwMk)

## How can we return the data from Controller to View 

 - we can do it using ViewBag, ViewData, ViewModel
 - Both ViewBag and ViewData doesn't provide compile time error checking.
 - ViewBag are stored as a name/value pair in ViewData dictionary internally.
 - It will be always a good practice to use strongly typed ViewModel over ViewData or ViewBag.
 
## what can't we return a ViewResult instead of Base Class ActionResult

 - Because controller can return more than just returning a view
 
 ## A CDN is an external resource and beyond our control. So, what if, CDN is down? How can we fall back from CDN to use local copy of Jquery.

The following code checks if jQuery is loaded and if it isn't, the jquery script will be loaded from our web server.  
```
<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js" type="text/javascript"> </script> 
<script type="text/javascript"> 
    window.jQuery || document.write('<script src="/MVCDemo/Scripts/jquery-1.7.1.min.js">\x3C/script>') 
</script> 
```
\x3C is hexadecimal for <
