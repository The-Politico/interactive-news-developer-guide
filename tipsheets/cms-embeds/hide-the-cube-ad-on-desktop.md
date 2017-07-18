## That cube ad is cutting into my graphic

###### Use this code sparingly, be creative in your layout -- ideally we would not have to deploy this code.

Sometimes, on desktop the cube ad gets in the way on desktop, chopping up your graphic. Here's how to hide the first cube ad on **DESKTOP ONLY**


```html
.story-interrupt.pos-alpha.predetermined {

display: none;

}

@media\(max-width: 60.25em\){

.story-interrupt.pos-alpha.predetermined {

display: inline;

}

}
```
