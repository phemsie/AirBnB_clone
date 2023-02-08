
AgeseVictor
/
AirBnB_clone
Public
Code
Issues
Pull requests
Actions
Projects
Security
Insights
AirBnB_clone/web_static/README.md
@AgeseVictor
AgeseVictor grace
 1 contributor
359 lines (321 sloc)  10.8 KB
0x01. AirBnB clone - Web static
Foundations > Higher-level programming > AirBnB clone

Web static, what?
we will build the front end step-by-step.

The first step is to “design” / “sketch” / “prototype” each element:

Create simple HTML static pages
Style guide
Fake contents
No Javascript
No data loaded from anything
Resources
Read or watch:

Learn to Code HTML & CSS (until “Creating Lists” included)
Inline Styles in HTML
Specifics on CSS Specificity
CSS SpeciFishity
Introduction to HTML
CSS
MDN
MDN: Introduction_to_HTML
center boxes
General
Allowed editors: vi, vim, emacs
All your files should end with a new line
A README.md file, at the root of the folder of the project, is mandatory
Your code should be W3C compliant and validate with W3C-Validator
All your CSS files should be in styles folder
All your images should be in images folder
You are not allowed to use !important and id (#... in the CSS file)
You are not allowed to use tags img, embed and iframe
You are not allowed to use Javascript
Current screenshots have been done on Chrome 56 or more.
No cross browsers
You have to follow all requirements but some margin/padding are missing - you should try to fit as much as you can to screenshots
Tasks
0. Inline styling [ 0-index.html ]
Write an HTML page that displays a header and a footer.

Layout:

* Body:
	no margin
	no padding
* Header:
	color #FF0000 (red)
	height: 70px
	width: 100%
* Footer:
	color #00FF00 (green)
	height: 60px
	width: 100%
	text [ Holberton School ] center vertically and horizontally
	always at the bottom at the page
Requirements:

You must use the header and footer tags
You are not allowed to import any files
You are not allowed to use the style tag in the head tag
Use inline styling for all your tags
1. Head styling [ 1-index.html ]
Write an HTML page that displays a header and a footer by using the style tag in the head tag (same as 0-index.html)

Requirements:

You must use the header and footer tags
You are not allowed to import any files
No inline styling
You must use the style tag in the head tag
The layout must be exactly the same as 0-index.html

2. CSS files [ 2-index.html, styles/2-common.css, styles/2-header.css, styles/2-footer.css ]
Write an HTML page that displays a header and a footer by using CSS files (same as 1-index.html)

Requirements:

You must use the header and footer tags
No inline styling
You must have 3 CSS files:
	styles/2-header.css: for header style
	styles/2-footer.css: for footer style
The layout must be exactly the same as 1-index.html

3. Zoning done! [ ]
Write an HTML page that displays a header and footer by using CSS files (same as 2-index.html)

Layout:

* Common:
	no margin
	no padding
	font color: #484848
	font size: 14px
	font family: Circular,"Helvetica Neue",Helvetica,Arial,sans-serif;
	icon in the browser tab
* Header:
	color: white
	height: 70px
	width: 100%
	border bottom 1px #CCCCCC
	logo align on left and center vertically (20px space at the left)
* Footer:
	color white
	height: 60px
	width: 100%
	border top 1px #CCCCCC
	text Holberton School center vertically and horizontally
	always at the bottom at the page
Requirements:

No inline style
You are not allowed to use the img tag
You are not allowed to use the style tag in the head tag
All images must be stored in the images folder
You must have 3 CSS files:
	styles/3-header.css: for the header style
	styles/3-footer.css: for the footer style
4. Search! [ 4-index.html, styles/4-common.css, styles/3-header.css, styles/3-footer.css, styles/4-filters.css, images/ ]
Write an HTML page that displays a header, footer and a filters box with a search button.

Layout: (based on 3-index.html)

* Container:
	between header and footer tags, add a div:
		classname: container
		max width 1000px
		margin top and bottom 30px - it should be 30px under the bottom of the header (screenshot)
		center horizontally
* Filter section:
	tag section
	classname filters
	inside the .container
	color white
	height: 70px
	width: 100% of the container
	border 1px #DDDDDD with radius 4px
* Button search:
	tag button
	text Search
	font size: 18px
	inside the section filters
	background color #FF5A5F
	text color #FFFFFF
	height: 48px
	width: 20% of the section filters
	no borders
	border radius: 4px
	center vertically and at 30px of the right border
	change opacity to 90% when the mouse is on the button
Requirements:

You must use: header, footer, section, button tags
No inline style
You are not allowed to use the img tag *You are not allowed to use the style tag in the head tag
All images must be stored in the images folder
You must have 4 CSS files:
	styles/3-header.css: for the header style
	styles/3-footer.css: for the footer style
	styles/4-filters.css: for the filters style
4-index.html won’t be W3C valid, don’t worry, it’s temporary
5. More filters [ 5-index.html, styles/4-common.css, styles/3-header.css, styles/3-footer.css, styles/5-filters.css, images/ ]
Write an HTML page that displays a header, footer and a filters box.

Layout: (based on 4-index.html)

* Locations and Amenities filters:
	tag: div
	classname: locations for location tag and amenities for the other
	inside the section filters (same level as the button Search)
	height: 100% of the section filters
	width: 25% of the section filters
	border right #DDDDDD 1px only for the first left filter
	contains a title:
		tag: h3
		font weight: 600
		text States or Amenities
	contains a subtitle:
		tag: h4
		font weight: 400
		font size: 14px
		text with fake contents
Requirements:

You must use: header, footer, section, button, h3, h4 tags
No inline style
You are not allowed to use the img tag
You are not allowed to use the style tag in the head tag
All images must be stored in the images folder
You must have 4 CSS files:
	styles/4-common.css: for the global style (body and .container styles)
	styles/3-header.css: for the header style
	styles/3-footer.css: for the footer style
	styles/5-filters.css: for the filters style
6. It's (h)over [ 6-index.html, styles/4-common.css, styles/3-header.css, styles/3-footer.css, styles/6-filters.css, images/ ]
Write an HTML page that displays a header, footer and a filters box with dropdown.

Layout: (based on 5-index.html)

* Update Locations and Amenities filters to display a contextual dropdown when the mouse is on the filter div:
	tag ul
	classname popover
	text should be fake now
	inside each div
	not displayed by default
	color #FAFAFA
	width same as the div filter
	border #DDDDDD 1px with border radius 4px
	no list display
	Location filter has 2 levels of ul/li:
		state -> cities
		state name must be display in a h2 tag (font size 16px)
Requirements:

You must use: header, footer, section, button, h3, h4, ul, li tags
No inline style
You are not allowed to use the img tag
You are not allowed to use the style tag in the head tag
All images must be stored in the images folder
You must have 4 CSS files:
	styles/3-header.css: for the header style
	styles/3-footer.css: for the footer style
	styles/6-filters.css: for the filters style
7. Display results
Write an HTML page that displays a header, footer, a filters box with dropdown and results.

Layout: (based on 6-index.html)

* Add Places section:
	tag: section
	classname: places
	same level as the filters section, inside .container
	contains a title:
		tag: h1
		text: Places
		align in the top left
		font size: 30px
	contains multiple “Places” as listing (horizontal or vertical) describe by:
		tag: article
		width: 390px
		padding and margin 20px
		border #FF5A5F 1px with radius 4px
		contains the place name:
			tag: h2
			font size: 30px
			center horizontally
Requirements:

You must use: header, footer, section, article, button, h1, h2, h3, h4, ul, li tags
No inline style
You are not allowed to use the img tag
You are not allowed to use the style tag in the head tag
All images must be stored in the images folder
You must have 5 CSS files:
	styles/3-header.css: for the header style
	styles/3-footer.css: for footer style
	styles/6-filters.css: for the filters style
	styles/7-places.css: for the places style    
8. More details [ 8-index.html, styles/4-common.css, styles/3-header.css, styles/3-footer.css, styles/6-filters.css, styles/8-places.css, images/ ]
Write an HTML page that displays a header, a footer, a filter box (dropdown list) and the result of the search.

Layout: (based on 7-index.html)

Add more information to a Place article:

* Price by night:
	tag: div
	classname: price_by_night
	same level as the place name
	font color: #FF5A5F
	border: #FF5A5F 4px rounded
min width: 60px
height: 60px
font size: 30px
align: the top right (with space)
* Information section:
	tag: div
	classname: information
	height: 80px
	border: top and bottom #DDDDDD 1px
	contains (align vertically):
		Number of guests:
			tag: div
			classname: max_guest
			width: 100px
			fake text
			icon
		Number of bedrooms:
			tag: div
			classname: number_rooms
			width: 100px
			fake text
			icon
		Number of bathrooms:
			tag: div
			classname: number_bathrooms
			width: 100px
			fake text
			icon
User section:
	classname: user
	text Owner: <fake text>
	Owner text should be in bold
Description section:
	classname: description
Requirements:

You must use: header, footer, section, article, button, h1, h2, h3, h4, ul, li tags
No inline style
You are not allowed to use the img tag
You are not allowed to use the style tag in the head tag
All images must be stored in the images folder
You must have 5 CSS files:
	styles/4-common.css: for the global style (i.e. body and .container styles)
	styles/3-header.css: for the header style	
	styles/3-footer.css: for the footer style
	styles/6-filters.css: for the filters style
	styles/8-places.css: for 
