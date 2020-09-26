# FARlert
Fast-Asynchronous-Responsive Alert

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
### Example
``
var Alert1 = new FAR.popup({
            borderFlash: true,
            jQuery: false,
            moveable: true,
            ding: true,
            html: "<span style='font-size:24px;font-weight:600'>Suspicious Login Attempt</span><br><br>We have detected that somebody has tried to enter your account without authorizaton!<br><br>We recommend you go to your settings to change your password.",
            title: 'Account Security Alert',
            buttons: [
                {
                    name: 'Settings',
                    func: 'doSomething()'
                },
                {
                    name: 'Ignore',
                    func: 'Alert1.retract()'
                }
            ]
        });
 Alert1.hoist();
``
