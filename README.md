## Website Performance Optimization portfolio project

PageSpeed Insights:

index.html:
* Mobile: 94/100
* Desktop: 95/100

## Changelog:

* Optimized images
* refactored /views/js/main.js:
  * Line 516: moved document query out of for loop, no forced reflow
  * Line 520: changed DOM call to getElementsByClassName
  * Line 538: changed the cols and s values to 12 and 512 respectively
  * changePizzaSizes(size) function refactored to use % and not query the document inside the for loop
* On code review:
    * resizePizzas(size) refactored to use getElementById
    * changePizzaSizes(size) refactored to use getElementsByClassName
    * changePizzaSizes(size) refactored to declare variable outside of for loop
    * cols and s values set back to default
    * Number of pizzas changed from 200 down to 24
    * Declared movingPizzas variable outside of for loop for performance gains

* Refactored /views/css/style.css:
  * added img {will-change: transform} to allow layering of redrawn elements

# To run:

Download all files in this repo to you computer, and navigate to index.html
