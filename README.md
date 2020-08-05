# Psychic-Game

### Before You Begin
1. Create a new GitHub repo.Then, clone it to your computer.

2. Inside your local git repository, create an `index.html`.

  * Also create `composer.json` and `index.php` files, if you are deploying to Heroku.

  * Fill in the appropriate content in the composer.json and index.php files to be able to deploy your game to Heroku when it is finished.

3. While still in your local git repo, create a directory called `assets`.
  * `cd` your way into the `assets` folder, then make three additional folders: `javascript`, `css` and `images`.
    * In the `javascript` folder, make a file called `game.js`. Use the `src` attribute of the `script` tag to link to this file, rather than embedding the code directly in your HTML document.
    * In the `css` folder, make a file called `style.css`.
    * Also in the `css` folder, make a file called `reset.css`. Paste into it the code from the Meyerweb reset stylesheet. If you opt to use Bootstrap instead of writing your own CSS, skip this step, and simply include a link to Bootstrap via CDN.
    * In the `images` folder, save whatever images you plan on using.

4. Push the above changes to GitHub.

5. Push your selected game to `gh-pages`. Alternatively, if using Heroku:

  * `heroku login`
  * `heroku create`
  * `git push heroku master`

# Psychic-Game

![Psychic](Images/1-Psychic.jpg)

1. [Watch the demo](psychic-game-demo.mov).

2. You're going to make a game just like the one in the video. Essentially, the app randomly picks a letter, and the user has to guess which letter the app chose. Put the following text on your page:

  * Guess what letter I'm thinking of

  * Wins: (# of times the user has guessed the letter correctly)

  * Losses: (# of times the user has failed to guess the letter correctly after exhausting all guesses)

  * Guesses Left: (# of guesses left. This will update)

  * Your Guesses So Far: (the specific letters that the user typed. Display these until the user either wins or loses.)

3. When the player wins, increase the Wins counter and start the game over again (without refreshing the page).

4. When the player loses, increase the Losses counter and restart the game without a page refresh (just like when the user wins).
