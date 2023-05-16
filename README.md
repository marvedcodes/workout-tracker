# Workout Tracker

This is a Vanilla JavaScript Project using Object-oriented programming.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### Screenshot

![workout-tracker-kappa vercel app_(iMac)](https://user-images.githubusercontent.com/108392678/199262804-47b8a9d1-4337-4eb0-a75f-6249eec81b43.png)

### Links

- DEMO:[Link](https://workout-tracker-kappa.vercel.app/)

## My process

### Built with

- [JavaScript (ES6 Classes)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

### What I learned

- Design as a Responsive web
- Use of Local Storage API
- Geolocation API
- Displaying Google map via Leaflet Library
- Using custom icons for Leaflet instead of just normal points on the map
- Abilities to edit & delete workout and delete all workouts
- Ability to sort workouts by certain fields(distance, time)
- Position the map to show all workouts
- Click on popup, move map to corresponding popup
- Map Zoom and View control
- Markup and styling for new created submenus & realistic error message

Here is a code snippet:

```script.js
class Running extends Workout {
  type = 'running';

  constructor(coords, distance, duration, city, country, cadence) {
    super(coords, distance, duration, city, country);
    this.cadence = cadence;
    this._calcPace();
    this._setDescription();
  }

  _calcPace() {
    this.pace = this.duration / this.distance;
  }
}
```


### Useful resources

- [MDN Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes) - This helped me for creating ES6 classes.
- [Leaflet](https://leafletjs.com/) - This helped me for showing Google Maps.


## Author

- Website - [Marvin Morales Pacis](https://marvin-morales-pacis.vercel.app/)
- LinkedIn - [@marventures](https://www.linkedin.com/in/marventures/)
- Twitter - [@marventures11](https://www.twitter.com/marventures11)
