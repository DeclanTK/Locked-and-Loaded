# Locked-and-Loaded
An escape the room type puzzle game coded in python for a class project at Drexel University.

Thanks for checking out our project. This is a self designed GUI based puzzle game, developed in Python with a team of 5 students. Using custom images, and game concepts we created an escape the room game that involves various puzzles with the goal of "escaping" the virtual room. Python concepts we used include, pickle (a simple stack-based serialization method), database, randomizing and self made functions, as well as, cursor coordinate tracking and event recognition, and conditional statements and loops.

We we're the only group in the class to receive a score of 100% on our project and I think if you take a look our efforts will become evident.

You'll find all of the images and necessary data files, as well as all python files are included in this repository. When coding our project we ran into problems as all programmers do. However we managed to overcome many of them thanks to hours spent collaborating in the engineering building and the library. The issues we could not over come are listed below. In order to make the gaming experience more smooth and to avoid any confusion it is recommended that you read on to understand what may occur and how to avoid these bugs.

Please note: The GUI's we make in our game use Tkinter and therefore many of these issues can be attributed to the limitations of Tkinter as a game development platform.

**Note #1 (Double clicking):**
We designed our game so that there were as few "Tkinter buttons" as possible. I made many of our in-game images in photoshop and because of this we had the ability to customize where certain things would be on our screen. Therefore we were able to designate regions of the canvas to a certain button click. However despite our efforts in using time.sleep we could not figure out a way to stop "bad things" from happening when a user clicked rapidly in a certain region ("button") on the screen. What happens is a window will open as it should, but when that game is won, lost or exited, another game window appears because the user double clicked thus executing the file again once the first file has run its course. We decided that this was due to Tkinter being limited __*to an extent*__ for our purposes.

**Note #2 (Delayed clicking):**
This too had to do with our using regions of the screen as buttons as opposed to using the built in "Tkinter buttons". When playing, a game a GUI opens in front of the "main_screen" GUI. If this game GUI is aligned incorrectly over the "main_room" GUI and the user clicks the "return to the room" arrow on the bottom left of current GUI the user's machine will execute whatever was behind the user's mouse on the current GUI as well as the "main_room" GUI behind it. For example, if the user positions their windows such that the "return to the room" button is directly over the locked door in the "main_room" GUI, when the user clicks the button their current game will exit as it should, however the "final_door" game GUI will immediately be opened due to the mouse click registering in a delayed fashion on both GUI's. We tried to solve this using time.sleep again however this impeded gameplay too much and wasn't a *perfect fix* so we removed it.

**Note #3 (Maze Game clicking):**
We use regional clicking in the maze game as well. This works properly on some machines but not on all for some reason. On Trung's laptop it works ideally, on mine however it does not, I personally think it has to do with the users hardware and what resolution their screen is (mine is 1920x1080). This isn't so much an issue as something to be aware of and as such isn't listed as a weakness for our group. When your cursor changes on the screen for the mouse game that is the indication that you can click and your triangle (player) will move in that direction.

**Note #4 (Maze Game rendering):**
Again this isn't listed as a weakness because the code itself is a huge strength for our group. Trung developed code that would randomly generate a maze albeit a pixelated one. This maze is relatively hard because of the visuals being empty black and white squares or filled black and white squares. My best advice would be to squint your eyes a bit and you will start to see the path to the end of the maze. I also will say the more times you play the maze game the more accustomed your eyes will get to seeing the maze and how to solve it.

**Note #5 (Windowed game play):**
It is included in our how to play section but I wanted to reiterate. It is important that you play in windowed mode for the best visual gaming experience. It is also important that you reposition each window as it opens so that you are able to see the entire window. This will ensure you don't miss any labels or potential game play pieces that would otherwise be occluded.

Other than that I sincerely hope you enjoy our game. We worked very hard on it and extremely proud to put our names on it. Enjoy!
