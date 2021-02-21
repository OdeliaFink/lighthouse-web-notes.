# Bubbling & Capturing 

## Bubbling:
* An event happens on an element, runs the handler then its parent and all the way up
* Called bubbling because bubbles from the inner element up to the parent elements
* Can stop the bubbling process through event.stopPropogation() but you don't need to add this 

## Capturing:
### Three phases of event propogation: 
* Capturing phase: event goes down to the element. Used rarely 
* Target Phase: event reaches element
* Bubbling Phase: event bubbles back up from element 