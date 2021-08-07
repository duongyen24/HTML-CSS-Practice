# HTML-CSS-Practice
when create HTML- work in desktop mode first then move to CSS- work in mobile mode first

making web page responsive with HTML and CSS
HTML: 
	
	-structure everything, insert class, div, section,container
	- having an overview eyes, how many column?
	

CSS:
	-move to small detail:padding, font size,..
	-setup  using ruleset - custom properties so we dont need to set color again, just use  in root set
	
	:root {
 		 --main-bg-color: brown;
	}

	- using padding: for spacing
	-using container: keep content off the side in screen
	-when custom image always use this:
		img{
			display: block;
			max-width: 100%;
		}

	-when split EQUAL column in responsive web
			.split{
			display: flex;
			flex-direction: column; /* reset thing to normal, flex-box*/
		}

		/* query media */
		@media(min-width: 40em){
			.split{
				flex-direction: row;
			}
			.split > * {
				flex-basis: 100%;
			}
		}
