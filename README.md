# Typewriter JS
Typing effect using JS. Used in my own person site.

## Usage
To start using this effect, you need to import them to the respective sections in the HTML file.
```
<link rel="stylesheet" href="typewriter.css" />
<script src="typewriter.js"></script>
```
Any element in the HTML containing the `typewriter` class will have the effect automatically added to it. It must also contain the `data-content` attribute.
```
<p class="typewriter" data-contents='["Testing 1", "Testing 2", "Testing 3"]'>
    <span class="wrap"></span>
</p>
```
The `data-content` attribute takes in a json formatted array as shown in the example above.

## Modifiers
There're a few modifiers that can be used to change how the effect will take place. All unit of speed is milliseconds.

### Typing Speed
By adding `data-speed` you can change the typing speed of the effect. 
```
<p class="typewriter" data-speed="150" data-contents='["Testing 1", "Testing 2", "Testing 3"]'>
    <span class="wrap"></span>
</p>
```
The default typing speed is 200.

### Period Speed
By adding `data-period` you can change the period between each sentence/content. 
```
<p class="typewriter" data-period="1000" data-contents='["Testing 1", "Testing 2", "Testing 3"]'>
    <span class="wrap"></span>
</p>
```
The default period is 2000.

### Randomized
By adding `randomized` as an attribute, you can randomize the array.
```
<p class="typewriter" randomized data-contents='["Testing 1", "Testing 2", "Testing 3"]'>
    <span class="wrap"></span>
</p>
```

## Changing Constants
By default, the constants are set at the top of the `typewriter.js` file and can be change to fit your need.
```
const DEFAULT_SPEED = 200;
const DEFAULT_PERIOD = 2000;
const DEFAULT_WAIT = 500;
```