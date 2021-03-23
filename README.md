# Pre-work - *Memory Game*

Remember Me? is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Tommy Kim

Time spent: 7 hours spent in total

Link to project: https://glitch.com/edit/#!/button-scratch-duckling

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [x] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [x] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [x] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:
![x]

    http://g.recordit.co/RrlX5JXeUN.gif

    http://g.recordit.co/RrlX5JXeUN.gif
    


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

One challege I encountered while creating this submission was when I was working on the limited
time feature for each guess. I was having trouble figuring out when and how to start and stop the 
timer. When it comes to challenging parts of code, I like to break it up into pieces. First, I 
made a timer that simply counts down from 5 and stops at 0. Then, I synced up the timer to only 
start when the start button was pressed. Next, the challenge was to figure out how to add the 
delay to start the timer at the right time. The timer should start after it goes through the pattern, 
so I deduced I need to use setTimeout with the value of the accumulated delay. This part was challenging
because it required me to use the setTimeout function within the setInterval function. However, I 
was able to solve it by rereading the playClueSequence code and keeping track of the value of delay
in the developr console to see how it changes after each pattern. Seeing the final value of the delay 
after the loop made me realize it was when the pattern ended. Therefore, I was able to overcome this 
challenge by tackling code in smaller parts, debugging using my developer console, and rereading code.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

One question I have about web development is the difference of scopes between var, let, and const.
I know about their general usage and that they have different scopes, but I am still unsure exactly 
how they are different. Another question I have is how prevalent regular Javascript is in the 
industry. I know how popular React is, but is regular Javascript still used in large companies?
With how powerful React is, I don't see any reason to use Javascript without any libraries.
My last question is whether more frontend or backend developers are needed in the industry. Is
one more in demand than the other right now, or are they equally needed? 

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

If I had a few more hours to work on this project, I would add a feature for the user to input
the length of the pattern. That way, the user can set the difficulty instead of simply always 
doing a pattern of length 8. Another thing I would change is the display of the timer. Right 
now, the timer is in text form, but I would like to change it to a visual countdown of a real 
clock so that the user can see their time more clearly. Another quick feature I would add is
to count the number of patterns the user has completed. It would save the count on a page refresh 
too. I would also add the option to change the sound effects for the buttons. I would experiment 
with different sounds and allow the user to choose which sound he or she likes. Finally, I would
add a volume slider so the user could adjust the sound of the sound effects. This would allow the
user to mute sound if he or she only wants to play remembering the visuals of the pattern.


## License

    Copyright [Tommy Kim]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.