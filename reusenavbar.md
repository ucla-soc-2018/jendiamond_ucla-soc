My navigation bar is in the body tag. Entire code for navigation bar is in nav.html file (without any html or body tag, only the code for navigation bar). 

In the target page, this goes in the head tag:

<script src="https://code.jquery.com/jquery-1.10.2.js"></script>

Then in the body tag, a container is made with an unique id and a javascript block to load the nav.html into the container, as follows:

<!--Navigation bar-->
<div id="nav-placeholder">

</div>

<script>
$(function(){
  $("#nav-placeholder").load("nav.html");
});
</script>
<!--end of Navigation bar-->