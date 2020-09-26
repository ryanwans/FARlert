# FARlert
Fast-Asynchronous-Responsive Alert
<br>
![example of alert](https://raw.githubusercontent.com/ryanwans/FARlert/master/exampleAlert.png)
<br>
### Create an alert
`var Alert = new FAR.popup({options...});`
<br>
### Hoist an alert
`Alert.hoist();`
<br>
### Retract an alert
`Alert.retract();`
<br>
### Options
`pageBlur`: Boolean. Blur the page behind an alert (defualt false)<br>
`borderFlash`: Boolean. Flash the border of an alert red & yellow (default false)<br>
`jQuery`: Boolean. Choose to disable the usage of jQuery (default true)<br>
`ding`: Boolean. Ding sound effect upon the hoisting of an alert (default false)<br>
`moveable`: Boolean. Allow the alert to be dragged around (default true)<br>
`escapeKey`: Boolean. Allow the usage of escape key to close alert (default true)<br>
`title`: String. The title of the alert box (default "User Action Required")<br>
`html`: String. The inner html content of the alert (default "null")<br>
`buttons`: Array. An array of object (see below) for the escape buttons (default Close)<br>
`newWindow`: Boolean. Open the alert in a seperate window. (default false)<br>
<br>
### Example of Buttons
`[{name: 'Ignore', func: 'doThis()'}, {name: 'Browse...', func: 'doThat()'}]`
