# iOS: Custom UIViewController circular transition animation

Based on YouTube video [iOS Swift Tutorial: Create a Circular Transition Animation (Custom UIViewController Transitions)](https://youtu.be/B9sH_VxPPo4)

## Steps

Create single view application

Drag an additional View Controller onto Storyboard

Drag an Image View onto initial View Controller

- resize to fill entire View Controller
- in Size Inspector > Autoresizing, click all constraints to have Image View stretch to fill the view and maintain its aspect ratio

Drag a background image to Assets.xcassets and rename it to background

In Storyboard > Attributes Inspector

- set the Image View to background
- set View > Content Mode to Aspect Fit

Drag a Button above Image View - this will act as the Menu button

- 40 x 40 pixels
- set text to M
- set background color to orange-yellow
- set text color to white, size to 17, style to Heavy
- set Autoresizing mask to only have the top constraint, so that it's always centered horizontally
- set Y position to 50
- duplicate Button onto second View Controller, and ensure Y position is 50
- set text of second Button to X - this will act as a Dismiss button
