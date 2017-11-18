# [JavaScript and CSS Clock](https://gk-hynes.github.io/js-and-css-clock/)

An analog clockface built with JavaScript for Wes Bos' [JavaScript 30](https://javascript30.com/) course.

[![Screenshot of JavaScript clock](https://screenshots.firefoxusercontent.com/images/60e26703-4af6-4f40-9716-5c10b11e4712.png)](https://gk-hynes.github.io/js-and-css-clock/)

## Notes

### CSS

Set the hands to start at 12 o clock using ```transform: rotate(90deg);```.

By default elements rotate at their centre. Set the hands to rotate from their right end using ```transform-origin: 100%;```. 

Give the hands a realistic 'tick' using a cubic-bezier transition-timing function: ```transition-timing-function: cubic-bezier(0.1, 2.7, 0.58, 1);```.

### JavaScript

Use a setInterval function to run the ````setDate()``` function every second. 

Use ````const now = new Date();``` and ```const seconds = now.getSeconds();``` etc. to gte the current time. 

Convert seconds, minutes and hours to degrees by dividing them by 60 or 12 and then multiplying the result by 360. Add 90 to offset the original move to 12 o clock. 

