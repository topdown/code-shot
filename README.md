# Code Shot
Simple Electron desktop app to create nice JPG pictures of code for Instagram and Twitter.

This app is just me playing around and learning more about building Electron apps.
So don't expect to much 😀

## Install / Run
```bash
# Clone this repository
git clone https://github.com/topdown/code-shot
# Go into the repository
cd code-shot
```

### Add Backgrounds
__Before running or building__ the app you need to add some background images. Wallpapers or something similar in (high) resolution is best.

Add your background images to `assets/backgrounds/`

The should be named like the following.
```bash
background1.jpg
background2.jpg
background3.jpg
background4.jpg
background5.jpg
background6.jpg
background7.jpg
background8.jpg
background9.jpg
background10.jpg
```

It will randomly load the background 1 - 10.

### Now you can run the app
```bash
# Install dependencies
npm install
# Run the app
npm start

```

__NOTE: The app will open to the size of a typical Instagram photo.__

Changing the window size changes the saved image size later.

## Build
I have only tested this on MacOS High Sierra

I used `electron-packager` which is already a dependency in the `package.json`

```bash
# MacOS
electron-packager . --overwrite --platform=darwin --arch=x64 --icon=assets/icons/Code-Shot2.icns --prune=true --out=release-builds
```

Your app will be in the __release-builds__ directory and you can drag it into Applications on your Mac to install.

## Using the App

There are __key commands__ for using the app or see the __Help menu__.

### Commands (MacOS tested)

* The normal App commands, see the __Edit Menu__ 
* `Command+R` to __reload__ this will refresh the app and choose a new random background.
* `Command+Q` to __quit__ the app.
* `Command+H` to __hide__ the app.
* `Option + N` __opens the form__ to add code and select highlighting (PHP, CSS, JS, Bash)
* `Option + Enter` to __insert__ the code.
* `Option + S` to generate and __save an image__ of it.

Now you can upload to your Instagram.

