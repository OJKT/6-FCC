# 6-FCC
Lesson Notes of OJKT
<link href="https://fonts.googleapis.com/css?family=Khand:500" rel="stylesheet">
<link href="https://fonts.googleapis.com/css?family=Lobster+Two" rel="stylesheet">
# FCC-6-Responsive Web Design Challenges
Responsive Web Design Challenges Lesson Notes of OJKT
<!DOCTYPE: html>
<html>
	
<div id="page-wrapper">
	<style>
	 body, html {
	  font-family: "Khand", sans-serif;
	  background: lightgrey;
	 }

	/*toolbar&title*/
	#title {
		position: static;
		top: 0;
		right: 0;
		padding-left: 15vh;
		padding-right: 15vh;
		padding-bottom: 5vh;
		padding-top: 4vh;
	  	margin-top: 5px;
		margin-left: 1vw;
		margin-right: 0.3vw;
		color: black;
		background: repeating-linear-gradient(180deg, black 0px, orange 40px, black 80px);
	  	font-size: 4vm;
		font-size: 5vh;
	 	font-family: font-family: 'Lobster Two', cursive;
		text-align: center;
		text-transform: uppercase;
	}	
	/*toolbar&title*/

	/*footer*/
	footer {
		position: static;
		bottom: 0;
		right: 0;
	  	margin-top: 10px;
		margin-left: 0px;
		padding-left: 10px;
		margin-right: 1px;
	  	background-color: #C0C0C0;
		border: 4px solid #000;
		border-radius: 4px;
		color: darkgrey;
		font-size: 2vm;
		font-size: 2vh;
	}
	span {
	    margin-right: 10px;
	    display: flex;
	    justify-content: flex-end;
	    font-size: 0.9em;
	    color: #eee;
	}
	/*footer*/

	/*navlinks*/
	  ul {
		position: fixed;
		Padding-top: 0vh;
		margin-top: 1vh;
		margin-left: 90vw;
		font-family: font-family: 'Lobster Two', cursive;
		text-transform: none;
		font-size: 3vm;
		font-size: 3vh;
		background-color: white;
		transform: rotate(-45deg);
		border: solid black 1vh;
		border-radius: 4vh;
	}
	#nav-link {
		padding-left: 0px;
		padding-right: 5px;
		color: red;
		font-size: 3vh;
	    }
	/*navlinks*/

	/*two boxes*/
	  #box-container {
	    	display: flex;
	    	height: 500px;
	  }
	  #box-1 {
	    	background-color: dodgerblue;
	    	width: 250px;
	    	height: 250px;
	  }
	  #box-2 {
	    	background-color: orangered;
	    	width: 250px;
	    	height: 250px;
	  }
	/*two boxes*/
	
	p {
		margin-right: 30px;
		margin-left: 5px;
	}

	#subtitles {
		color: red;
	}
	</style>

	<header id="header"></header>
	<head class="head">
		<h1 id=title><u>Introduction to the CSS Flexbox Challenges</u></h1>
		<div id="nav-bar">
				<ul>
				 <strong><a class="nav-link" href="#header" id="nav-link">Jump to top</a></strong>
					<br>
				 <strong><a class="nav-link" href="#footer" id="nav-link">Jump to bottom</a></strong>
				</ul>
		</div>
	  	</nav>
		<hr>
	</head>


	<div id="Learning_Objectives">
		<p><u>Learning Objectives :</u><p>
	    <ol>
			<li><a class="nav-link" href="#box">Use display: flex to Position Two Boxes</a></li>
			<li>Add Flex Superpowers to the Tweet Embed</li>
			<li><a class="nav-link" href="#box">Use the flex-direction Property to Make a Row</a></li>
			<li>Apply the flex-direction Property to Create Rows in the Tweet Embed</li>
			<li><a class="nav-link" href="#box">Use the flex-direction Property to Make a Column</a></li>
			<li>Apply the flex-direction Property to Create a Column in the Tweet Embed</li>
			<li><a class="nav-link" href="#justify_content,_align_items_&_wrap">Align Elements Using the justify-content Property</a></li>
			<li>Use the justify-content Property in the Tweet Embed</li>
			<li><a class="nav-link" href="#justify_content,_align_items_&_wrap">Align Elements Using the align-items Property</a></li>
			<li>Use the align-items Property in the Tweet Embed</li>
			<li><a class="nav-link" href="#justify_content,_align_items_&_wrap">Use the flex-wrap Property to Wrap a Row or Column</a></li>
			<li><a class="nav-link" href="#box">Use the flex-shrink Property to Shrink Items</a></li>
			<li><a class="nav-link" href="#box">Use the flex-grow Property to Expand Items</a></li>
			<li><a class="nav-link" href="#box">Use the flex-shrink Property to Shrink Items</a></li>
			<li><a class="nav-link" href="#box">Use the flex-basis Property to Set the Initial Size of an Item</a></li>
			<li><a class="nav-link" href="#box">Use the flex-shrink Property to Shrink Items</a></li>
			<li><a class="nav-link" href="#shortcut_flex_&_order">Use the flex Shorthand Property</a></li>
			<li><a class="nav-link" href="#shortcut_flex_&_order">Use the order Property to Rearrange Items</a></li>
			<li><a class="nav-link" href="#justify_content,_align_items_&_wrap">Use the align-self Property</a></li>
	   </ol>
		<br><hr>
	 </div>	

	<div id="box">
		<h2> Two Boxes</h2>
		<div id="box-container">
			<div id="box-1"></div>
			<div id="box-2"></div>
		<br>
	</div>
		<p>These two boxes can fall into normal flow with, display: flex; | they can swap places in a row with flex-direction: row-reverse; |  you can put them back into a column wih flex-direction: column; <br>| there are probably more to look up <a href="https://www.w3schools.com/">here</a>
		</p>
		<p>
		The <i>flex-shrink</i> property takes numbers as values. The higher the number, the more it will shrink compared to the other items in the container. For example, if one item has a <i>flex-shrink</i> value of 1 and the other has a flex-shrink value of 3, the one with the value of 3 will shrink three times as much as the other. so i suppose you can guess what <i>flex-grow</i> does...
		</p>
		<p>The flex-basis property specifies the initial size of the item before CSS makes adjustments with flex-shrink or flex-grow.
		</p>
		<br>
		<p>
		The units used by the flex-basis property are the same as other size properties (px, em, %, etc.). The value auto sizes items based on the content.</p>
		<p>for more infor go <a href="https://www.w3schools.com/">here</a></p>

	<br><hr>
		</div>

	<div id="justify_content,_align_items_&_wrap">
		<p>justify-content property set to any of these values: center, flex-start, flex-end, space-between, or space-around. The align-items property is similar to justify-content. Recall that the justify-content property aligned flex items along the main axis. For rows, the main axis is a horizontal line and for columns it is a vertical line.
		<strong>Different values available for align-items include:</strong></p>
	 <ul>
		<li>	flex-start: aligns items to the start of the flex container. For rows, this aligns items to the top of the container. For columns, this aligns items to the left of the container.</li>
		<li>flex-end: aligns items to the end of the flex container. For rows, this aligns items to the bottom of the container. For columns, this aligns items to the right of the container.</li>
		<li>center: align items to the center. For rows, this vertically aligns items (equal space above and below the items). For columns, this horizontally aligns them (equal space to the left and right of the items).</li>
		<li>stretch: stretch the items to fill the flex container. For example, rows items are stretched to fill the flex container top-to-bottom.</li>
		<li>baseline: align items to their baselines. Baseline is a text concept, think of it as the line that the letters sit on.</li>
	 </ul>
		<p>
		CSS offers the align-items property to align flex items along the cross axis. For a row, it tells CSS how to push the items in the entire row up or down within the container. And for a column, how to push all the items left or right within the container.
		</p>
		<p>
		The final property for flex items is align-self. This property allows you to adjust each item's alignment individually, instead of setting them all at once. This is useful since other common adjustment techniques using the CSS properties float, clear, and vertical-align do not work on flex items.

	align-self accepts the same values as align-items and will override any value set by the align-items property.
		</p>
		<p>
		However, using the flex-wrap property, it tells CSS to wrap items. This means extra items move into a new row or column. The break point of where the wrapping happens depends on the size of the items and the size of the container.
		</p>
		<p><strong>**CSS also has options for the direction of the wrap:**</strong></p>
		
		<ul>
			<li>nowrap: this is the default setting, and does not wrap items.</li>
			<li>wrap: wraps items from left-to-right if they are in a row, or top-to-bottom if they are in a column.</li>
			<li>wrap-reverse: wraps items from bottom-to-top if they are in a row, or right-to-left if they are in a column.</li>
		</ul>
		
		<p>for more infor go <a href="https://www.w3schools.com/">here</a></p>
		<hr>
	</div>

	<div id="shortcut_flex_&_order">
		<h2>CSS Flexbox: Use the flex Shorthand Property</h2>
		<p>There is a shortcut available to set several flex properties at once. The flex-grow, flex-shrink, and flex-basis properties can all be set together by using the flex property.

	For example, flex: 1 0 10px; will set the item to flex-grow: 1;, flex-shrink: 0;, and flex-basis: 10px;.

		The default property settings are flex: 0 1 auto;.</p>
		<p>for more infor go <a href="https://www.w3schools.com/">here</a></p>
		<p> use the <i>order</i> property with values numerical, to order them how you wish... even with the boxes above</p>
	</div>

	<footer id="footer">
			<ol>
				<i><a href="#">Privacy  .</a></i><br>			
	      <i><a href="#">Terms  .</a></i><br>
	      <i><a href="https://www.facebook.com/Active-Boardom-1433050133615965/?__tn__=kC-R&eid=ARDxFnA2JMu6bjlwqWvI3V1d0Rce9HdYBzDGGtJp0BhH-ueOlTAQbh0whATwwgFna9sm9jkboRpjWJnD&hc_ref=ARQaDkOV-XEkdyZItVQH9yuafF_narIIMZukBWJoaFoVgKTTBr5qBLQ1pDtdCP1cxF0&fref=nf&__xts__[0]=68.ARDYkTx9CsRT4OGTCvkO4FfhIcApAmkjQ-zBxaLHt1nqutrcdBfuonVlBKBXLg-l6giN-MiLriy2iHhYK3-uZ7l8efaHcYfOQPPUo3YknyBCljz10jZVwawd_JPGlqxxUxpaKdDVOc7vv4zQb1gvTtbiga9MLXcGfadpQU6YN_ZFZFBORq0wTJ2gjwQWf-hqAyErVWR_HM-_tje583zlZDxOBvyFSIb71aWN5zby5u-Ar3tr-Zn6BXKJ03w-KH30lCsYY8yrgpdS7DWA_-M3ogU_9pI9jGXFww4iDR6qmOdznSinEPP_J0pCY3maDJ4_2n1-a3Uq57kDKz4vC98">Contact  .</a></i> <!--contact-->
			</ol>
		    <span>&copy Copyright 2018, OJKT STYLES</span>
		</footer>
	
</div>
