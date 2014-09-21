Amazon-like Multi Level Responsive Dropdown Menu
========

This plugin was created based on the Amazon-like dropdown menu by JavaScript Kit (www.javascriptkit.com)

You are free to use this plugin in any project, but make sure the credits are NOT removed

For live demo, go to http://clay6.com/qa/ and mouse over "Explore Categories" button. A separate demo.html file is included in this project for reference.

Usage
========

Important: For this example to work, you need to set the doctype of html as html5 as shown below:

    <!doctype html>
    <html>
        .....
        .....
        .....
        .....
        .....
    </html>


Include the amazonmenu.css file in the head section as below:

    <link rel="stylesheet" type="text/css" href="amazonmenu.css" />


Include jQuery (either from CDN or you can host it yourself) and amazonmenu.js before closing the body tag:

    <script type="text/javascript" src="//code.jquery.com/jquery-1.11.0.min.js"></script>
	<script type="text/javascript" src="amazonmenu.js"></script>


Put your menu's html inside a div with some id, and a class amazonmenu:

    <div id="my_menu" class="amazonmenu">
        <ul>
			<li>
				<a href="#">View Menu</a>
				......
				......
				......
				......
				......
			</li>
		</ul>
    </div>


Initialize the plugin by passing the id of the above div:

	<script type="text/javascript">
    	$(document).ready(function() {
			amazonmenu.init({
				menuid: 'my_menu'
			});
		});
	</script>


Options
========

You can pass below options when initializing the plugin (all are optional):

	1) animateduration: 100 //in milliseconds, this option mostly need not be passed

	2) showhidedelay: [500, 500] //first element of array is show delay, and next is the hide delay in milliseconds

	3) addBodyOverlay: true //whether to dim the background when menu is shown, default true


Look at demo.html for further reference. Happy menu-ing !!!
