# ChessCom Automater.

Hello, wild chess player. This tool is a Python script for Windows or MacOS that uses the chess engine [Stockfish](https://stockfishchess.org/) to automatically play the best move.
In addition to that, this automator script has features that make it play like a human. Like levels of accuracy and delays.

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

Create a terminal window in the directory you want the Automator to go to. You can do this by:

Opening a terminal window and run this command:

```bash
cd [replace_this_with_your_directory]
```

## Now you're ready for Step 2:

Clone either the `windows` version of the script or the `MacOS` version. You can do this by:

Running these git commands:

```bash
git clone https://github.com/EvaanChowdhry/ChessAutomater/windows
```

or for `MacOS`:

```bash
git clone https://github.com/EvaanChowdhry/ChessAutomater/MacOS
```

## Step 3:

Navigate to the directory you cloned the files to and then install requirements.txt. Use these commands:
`pip install -r requirements.txt`

## Step 4: 

Now that you're in the directory with the packages installed, open `.env` in a text editor. (For example, Notepad for Windows, TextEdit for MacOS)

The .env file should look something along the lines of:

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
If you don't have homebrew installed, install it from: https://brew.sh.

When you finish that, install stockfish with homebrew if you haven't already.
`brew install stockfish`

Then run this command to find its path.
`where stockfish`

Replace the stockfish_path with the path you get.

### level
Replace it with the level you chose.

Levels must be either a number between `1` (**worst**) and `4` (**best, but still makes mistakes**), `'stockfish'` (just the stockfish engine, **BE CAREFUL WITH THIS**), or `random`.

Now you're all set to enjoy automated chess with the ChessCom Automator! Good Luck!



**I do not take responsibility for what chaos you create. If your chess com account gets banned/locked/or any form of punishment, it is not my fault as you CHOSE to use this**



Credits to [Jad AlHakim](https://github.com/JadXV)
