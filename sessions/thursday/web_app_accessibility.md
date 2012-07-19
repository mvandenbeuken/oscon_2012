# Web Application Accessibility - Alice Boxhall

## Resources

[Accessibility Developer Tools](goo.gl/8irxZ)
[ChromeVox](goo.gl/ddR5A)

## Assistive Technology

* screen readers
* braille display
* screen magnifiers
* voice control device
* built-in, software, hardware

## ChromeVox

Screen reader developed by Google

Looks at the DOM, so can determine if an element acts like a button even if it's not explicitly a button

## Accessibility in HTML5

* Use clean HTML and use standard tags whenever possible
	* don't use a div as a button when you can use a button. Not all screen readers can read the DOM.
* Provide text alternatives (if it's not text, it's as good as invisible)
	* Use labels on form elements
	* Use alt on images (if you don't do this, screen readers will read out file names... imagine a page full of these)
* Manage focus
	* note - after a javascript event opens a div or a modal, put focus on that div or modal. This results in a more relevant context for the user of screen readers
	* use tabindexes
		* tabindex=0 for natural order
		* tabindex=1 or similar for manual tab order
		* tabindex=-1 to remove from tab order
* Add key handlers
* Add ARIA for screen readers
	* search for WAI ARIA - it's part of the HTML5 standards
	* Use aria-label or aria-labelledby to provide text on other elements, or where label is insufficient
	* Use aria-hidden attribute to hide element from the screen reader's view. Really nifty. In the pop-up example, you could remove the original document from the view in favor of the modal until the modal has been interacted with
	* aria-valuemin aria-valuemax aria-valuenow => useful for ranges (sliders, voting widgets)
	* aria-valuetext is helpful for providing a more meaningful description of the value of an element
	* aria-live => polite will not interrupt what's going on, assertive will. Polite is really valuable for anything that is being dynamically updated
	* Aria is considered by Chrome's Developer Tools. Will show up in an accessibility audit of a page.
* Be aware of contrast ratios


	


