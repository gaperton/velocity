# Velocity App for Fitbit Ionic

The Velocity application turns Fitbit Ionic into a smart digital compass and a speedometer using the data taken from the onboard GPS receiver. It can be used as a backup navigation solution while hiking or walking, and it is an invaluable tool for a small sailboat that helps you understand how well the sails are trimmed and keep to the desired course.

## Features

- Shows the current and average speed (tap to switch between units).
- Indicates acceleration/slowdown with a color bar.
- Shows the rotating analog compass directed to the average heading (tap to switch between current/average heading).
- Lock mode to lock the average heading and increase compass resolution (down button to enable/disable)
- Calculates time to sunset/sunrise (time screen, click up button to switch between screens).

## Screens

### Loading screen

This will be the first screen you'll see opening the app. When GPS connects, it will switch to the compass screen automatically. You can press the "up" button to switch to the time screen and back.

![loading](/loading-screen.png)

### Compass screen

The main screen that shows the rotating compass and the speed.

![compass](/compass-screen.png)

- The color bar at the top shows the difference between your current and average speed, indicating with a color if you are speeding up (green) or slowing down (red).
- Average and current speeds are displayed below the bar. Tap to switch between the units - knots, mph, kph.
- The rotating compass is below, aligned with the direction of your average movement in 10 seconds. The current direction is shown with an arrow, red if you are turning left and green if you're turning right.
- The direction of travel in degrees is displayed at the bottom. Tap the compass to switch between current and average direction.

### Lock mode

Press the "down" button to enter the lock mode. Average speed and direction will be locked, and compass view will increase the scale resolution showing a sector of 40 degrees which will help you keep to the locked course. Press the "down" button again to exit the lock mode.

![lock](/lock-mode.png)

### Time screen

Press the "up" button to switch between screens.

![time](/time-screen.png)

Here you can see the current time, speed, and direction. It also shows the time left until sunset for your current location, which is important if you want to finish your trip before the dark. When there will be less time left until sunset than time passed since the application start (presuming you launched it in the beginning of your trip), time to sunset will become red indicating you should return immediately.

## Cost and payment

Velocity has a 24 hour trial period and will cost 2.99 USD to unlock when the trial will end.

## FAQ

### Why doesn't the GPS connect?

The GPS connection depends on satellite visibility and might take some time, especially for the "cold start" if you're starting it for the first time. Give it a few minutes and make sure you're not inside of a building. Normally, it will take about 30 seconds or less to connect if it's not a cold start and you're outside. If you standing in the middle of a city with skyscrapers blocking the sky it might take longer.

### Why doesn't the compass work?

Keep in mind that Fitbit Ionic doesn't have a real compass and the direction is being taken from the GPS; if you're in a sailboat the GPS direction is actually preferable. You need to be outdoors and move for the app to determine direction properly.

## Support or Contact

If you have any issues or feature suggestions, please create an issue [here](https://github.com/gaperton/velocity/issues/new).
