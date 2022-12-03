# Change Fall Guys Music
**I DID NOT MAKE THIS, @FGMuffins on twitter did :)**
This is purely a demo on how github is more convienent :p

# Installation

1. **Download the handy dandy python script by using these commands in a command prompt! (open a command prompt by typing `cmd` into the search bar):**
```
cd C:\Users\%USERNAME%\Downloads
```
and
```
curl https://raw.githubusercontent.com/20kzhan/change-fg-music/main/decode_content_v2.py --output decode_content_v2.py
```
(in that order!)

2. **Getting the production strings!**

Open file explorer, and in the bar at the top type `%appdata%`

Then, click the back button in the top left. Now, open the `LocalLow` folder. Scroll down until you see the `Mediatonic` folder.

Open it, then open `FallGuys_client` as well.

Copy the `content_v2.gdata` file into your downloads folder.

3. ***spooky python stuff***

In your command prompt, run this command:
```
decode_content_v2.py content_v2.gdata
```

4. **Changing the music!**

Now, double click the file to open it in notepad. Hit `Ctrl+F` to open the search function! Look up the term `"levels_round"` (quote marks included) and you'll be taken to the list of all the round declarations in the game. What all this means isn't important right now, all we care about here is two variables: 

**"ingame_music_soundbank"** and **"ingame_music_event"** (*Shown below!*)
![image](https://user-images.githubusercontent.com/49377371/205427282-b4800fe8-fb59-4d57-951e-c1ac457c301c.png)

As you can probably guess, changing these will change what music plays on that round! I don't fully know what the difference is between the soundbank and the event, but both of these have to match or it won't work! I've taken the time to compile all the track names for you guys in a document here, as well as the internal round names so you can find them!

You can find the spreadsheet [here.](https://docs.google.com/spreadsheets/d/1wusidMJCEFIgZfC757F08wmsawP5RbqYj1noBzLtdWM/edit?usp=sharing)

### Example

For an example here, let's change the music of Fall Ball to play Survive the Fall instead of Beans of the Round Table. This is harder than you think, as you either need to find the exact version of Fall Ball in Squads, OR you need to change ALL versions of it to be safe. As I know the exact name for Fall Ball in Squads, I'll provide it here so you can follow along. Search for "round_fall_ball_squads_non_final", then click through the results until you find the one that has the music section. It should look like the picture below!
![image](https://user-images.githubusercontent.com/49377371/205427814-597d33ef-22c4-4f04-9b8e-bb69914e0db8.png)

Now all we need to do is replace "BNK_Music_Beans_Round_Table" with the new track we want, in this case "BNK_Music_Survive_The_Fall". We ALSO need to replace the property below it, which starts with "MUS_InGame_" so that it matches the name with the one above. Once you have done both of those, you're all set!

Take care not to make any typos in these track names, as that will make the music not work and leave the level silent!

Feel free to change as many tracks as you like, then save the file in your Downloads folder by hitting `Ctrl+S` on your keyboard!

[patty, put the rest of the instructions here tmrw]
