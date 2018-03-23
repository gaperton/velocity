# Velocity App for Fitbit Ionic

The Velocity application turns Fitbit Ionic to the smart digital compass and speedometer using the data taken from the onboard GPS receiver. Can be used as a backup navigation solution when hiking and walking, and is an invaluable tool for the small sailboat helping you to understand how well the sails are trimmed or keep the desired course.

## Features

- Shows the current and average speed (tap to switch between units).
- Indicate acceleration/slowdown with a color bar.
- Shows the rotating analog compass directed to the average heading (tap to switch between current/average heading).
- Lock mode to lock the average heading and increase compass resolution (down button to enable/disable)
- Calculates time to sunset/sunrise (time screen, click up button to switch between screens).

## Screens

### Loading screen

When application starts, that will be the first screen you see. When GPS will be connected, it will switch to the compass screen automatically.

### Compass screen

The main application screen showing the rotating compass and speed.

![compass](/compass-screen.png)

- The color bar at the top shows the difference between your current and average speed, indicating with a color if you are accellerating (green) or slowing down (red).
- Average and current speed are displayed below the bar. Tap to switch between the units - knots, mph, kph.
- The rotating compass is below, headed to your average movement direction for 10 seconds. The current heading is shown with an arrow, red if you turning left and green if you're turning right.
- The heading in degrees is displayed at the bottom. Tap to the compass to switch between current and average heading.

### Lock mode

Press "down" button to enter the lock mode. Average speed and heading will be locked, and compass view will increase the resolution showing the sector of 40 degrees which will help you to keep the locked course. Press "down" button again to exit the lock mode.

![lock](/lock-mode.png)

### Time screen

Press "up" button to switch between screens.

![time](/time-screen.png)

Here you can see the current time, speed, and heading. It also shows the time to sunset for you current location, which is important if you want to finish your trip before it will be dark around. When there will less time to sunset than elapsed since the application start (presuming that you started it in the beginning of your trip), time to sunset will become red indicating that you should return immediately.

## FAQ

### GPS can't connect

GPS connection depends on satellites visibility and might take some time, especially for the "cold start" if you're starting it for the first time. Give it a few minutes and make sure you're not inside of a building. Normally, it will take somewhat about half a minute or less to connect if it's not a cold start and you're on open air. If you staying in the middle of the city with a skyscrapers blocking the sky it might take longer.

### Compass doesn't work

Keep in mind that Fitbit Ionic doesn't have the real compass and the heading is being taken from the GPS, and it's actually preferable when you're in a sailboat. It means that you need to be outdoors and move for the app to determine direction properly.

## Support or Contact

If you have any issues or feature suggestions, please create an issue [here](https://github.com/gaperton/velocity/issues/new).
