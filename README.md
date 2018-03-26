# Project: Portfolio Site

### Needs to be changed!

This project creates a website server-side, to display the users favorite movies. The user can click any of the movies, to open a window to view the trailer of the movie.

## Architecture
The page is created server-side, by the following process:
* `media.py`: `Movie` Class, to store movie information in.
* `entertainment_center.py`: Constructors of class `Movie`, which hold the movie information of the favorite movies, i.e. title, description, image-url and youtube link for trailer. Calls function `open_movies_page` of `fresh_tomatoes.py` with a array of the movies, to create the page.
* `fresh_tomatoes.py`: Front-end contents (JS, HTML, CSS) and functions, to generate page.  

## Technology
* Python
* HTML, CSS, Javascript
* Bootstrap

## Deploy code
1. Install [Python](https://www.python.org/).
2. Clone this repository to your local drive.
3. In your terminal, cd into the folder of the cloned repository.
4. In your terminal, run `python entertainment_center.py`, to create the .html file. After which, the browser will open the newly created `fresh_tomatoes.html`-page with the user's favorite movies.
5. That's it - have fun! :-)

- Strategy: Bootstrap

Requirements:
- at least 4 images
- title text (h1, h2, etc.)
- regular (paragraph) text
- a logo.
- HTML5 semantic tags such as <header>, <footer>, <article>, <section> etc. are used to add meaning to the code.
- No <div> or <section> tags are without a CSS class or id.
- If you're using Bootstrap: the rows and columns of the grid must be wrapped in an element with a container class.
- An image's associated title and text renders next to the image in all viewport sizes.


Featured work should be:
- Item Catalog
- Travel Planner
- Set-up Linux server
- Multi-user blog


To-dos!:
* Code, test, refine
1. Structure by boxifying it
2. Write HTML tags with contents
3. Apply CSS styles (from BIGGEST to smallest) 
4. Smaller details, polish.



** Check for responsiveness (emulsion in Chrome)
** Make images responsive with media queries or css class of framework, whatever applicable.
Desktop
Mobile: Google Nexus 5
Tablet: Apple iPad
** review project rubric.

Notes:
- Create boxes around the design. Start with the biggest design; the whole design.
- Responsive design: use % instead of px to define width.

- Strategy
1) Grid fluid system: Columns grabs to the next line, as screen gets smaller (most simple) Use grids. Depending on the width:show less or more columns.
2) Flexbox: makes it easy to position items without using float.
display: flex;
flex-wrap: wrap; (boxes wraps, as width changes)
<order></order> (to decide order of elements in flexbox.

And then adding breakpoints:
@media screen and (min-width: 550px){
	.dark-blue: 50%;
}
etc.

Margin: outside of box. 
Padding: inside of box.

Bootstrap
Use class “img-responsive”.


- Media queries: to change design in relation to the size of the screen.
@media only screen and (max-width: 300px) {
	// Styles to be applied.
}

@media screen and (min-width: 500px) {
	body { background-color: green; }
}

<link rel=“stylesheet” media=“screen and (min-width):500px)” href=“over500.css”>

Don’t import media queries, as they are heavy to import.
Don’t use min-device-width! As it measures the whole screen and not the window.

Breakpoints
Breakpoints: number of times site is changing.
Decide number of breakpoints: look at the content.


- I often use EMs for my font sizes, but when it comes to margins and padding, I stick to px because it’s almost impossible to align text of different sizes along an edge if there are different font sizes involved.
em refers to the font size. 50 em * 16px (font size) = 800 px.
Why not use pxs? Because, when responsive, you need to change the pxs manually for each screen size.

“Ems” (em): The “em” is a scalable unit that is used in web document media. An em is equal to the current font-size, for instance, if the font-size of the document is 12pt, 1em is equal to 12pt. Ems are scalable in nature, so 2em would equal 24pt, .5em would equal 6pt, etc. Ems are becoming increasingly popular in web documents due to scalability and their mobile-device-friendly nature.