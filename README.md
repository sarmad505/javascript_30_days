Day 1 project link https://sarmad505.github.io/javascript_30_days/Drum_kit/
1. Function removeTransition(e):

Purpose: Removes the "playing" class from an element when a specific transition ends.
Steps:
Checks if the event's property name is 'transform' (likely indicating a CSS transition).
If so, removes the "playing" class from the element that triggered the event.

2. Function playSound(e):
Purpose: Plays a sound and adds a "playing" class to a visual element when a key is pressed.
Steps:
Finds the audio element with a data-key attribute matching the pressed key's code.
Finds the corresponding visual element (div) with the same data-key.
If the audio element is found:
Adds the "playing" class to the visual element.
Resets the audio's current time to 0.
Plays the audio.
3. Event Listeners:
Attaches listeners to elements:
Loops through all elements with the class "key".
For each element, adds a listener for the transitionend event, calling removeTransition when it occurs.
Adds a listener for the keydown event on the window, calling playSound when a key is pressed.

Overall Functionality:
Triggers sound and visual feedback when keys are pressed:
When a key is pressed:
The corresponding audio plays.
The corresponding visual element gets the "playing" class (likely for a visual effect).
When the visual transition ends (presumably a change in appearance), the "playing" class is removed.

Key Points:
The code relies on CSS transitions for visual effects.
The data-key attributes are used to link audio and visual elements to specific keys.
Event listeners handle user interactions and trigger actions.
