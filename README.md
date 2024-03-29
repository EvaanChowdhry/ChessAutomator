# ChessCom Automater.

Hello, wild chess player. This tool is a Python script for Windows or MacOS that uses the chess engine [Stockfish](https://stockfishchess.org/) to automatically play the best move.
In addition to that, this automator script has features that make it play like a human. Like levels of accuracy and delays.

You will not have to move any piece in the game, let the script do it's thing and you would probably win depending on this mistake rate, and/or your opponent's skill level.

**You may have some problems with your Chrome version. If it doesn't work once, try it with another version. I believe it was Chrome 119 or 120.**

Here are the different accuracy levels (1-4, stockfish, random):

1. Level 1: 50% chance of a move being a mistake.
2. Level 2: 25% chance of a move being a mistake.
3. Level 3: 10% chance of a move being a mistake.
4. Level 4: 1% chance of a move being a mistake.
5. **Stockfish**: No mistake rate, **but occasional mistakes done by stockfish** and not the mistake algorithm. **Be careful using this in public matches**.
6. Random

# Steps to use

The steps to get started using this chesscom automator are pretty easy.

## First step: 
Download the Repository.

First, click on the green `Code` Button. It should look something like this:   
![Code](https://i.ibb.co/Z1FC8z0/image.png)  

Then click on Download ZIP.

Extract the ZIP file, then delete any unnecessary files, like the macOS folder if you're on windows and vice versa. 

## Step 2:

Navigate to the respective folder you kept in step 1, then install everything listed in requirements.txt. Use these commands:
`pip install -r requirements.txt`

## Step 4: 

Now that you're in your folder and you have the packages installed, open `.env` in a text editor. (For example, Notepad for Windows, TextEdit for MacOS)

The .env file should look something like:

```
chromedriver_path=''
chrome_profile_path=''
stockfish_path=''
level=''
```

## Step 5:
Replace all the variables in .env with what you see in the next few fields.

### chromedriver_path:

Replace the chromedriver_path field with either one of these paths:

For Windows:
`./chromedriver.exe`

For macOS:
`./chromedriver`

### chrome_profile_path:

Replace the chrome_profile_path with the `Profile Path` you get when you visit
`chrome://version` on your Google Chrome.

### stockfish_path

Replace the stockfish_path with either one of these paths:

For Windows:
`./stockfish.exe`

For MacOS (you need `homebrew` for this):
If you don't have homebrew installed, install it from: [brew.sh](https://brew.sh).

When you finish that, install stockfish with homebrew if you haven't already.
`brew install stockfish`

Then run this command to find its path.
`where stockfish`

Replace the stockfish_path with the path you get.

### level
Replace it with the level you chose.

Levels must be either a number between `1` (**worst**) and `4` (**best, but still makes mistakes**), `'stockfish'` (just the stockfish engine, **BE CAREFUL WITH THIS, VERY RISKY**), or `random` which chooses from 1-4.

Now you're all set to enjoy automated chess with the ChessCom Automator! Good Luck!



**I do not take responsibility for what chaos you create. If your chess com account gets banned/locked/or any form of punishment, I am not responsible.**

If you try it and get a chrome version error, try updating chromedriver by downloading the new version.

Credits to [Jad AlHakim](https://github.com/DreamedOfIt)
