# Swipe -- 2024 BCS Hackathon

## Inspiration
The idea was sparked by the desire to make digital navigation as natural and intuitive as gesturing during a conversation. We aimed to bridge the gap between human intent and digital response, envisioning a world where your computer understands your hand movements as clearly as your words.

## What it does
Our Chrome extension expands upon a sophisticated TensorFlow hand-pose model to detect and interpret specific hand gestures via your webcam, translating them into common browser commands like scrolling, zooming, and tab switching. This creates a seamless browsing experience without the need for a mouse or keyboard.

[Watch a demo here](https://www.youtube.com/watch?v=LBj3UQgiR1Y)

<!-- Resizing image to 200x200 pixels -->
<img src="https://github.com/maxbueckert/Swipe/assets/122507377/7fdad400-2d84-4e96-b692-561c5f740c66" width="400" height="255">

<!-- Resizing image to 100x100 pixels -->
<img src="https://github.com/maxbueckert/Swipe/assets/122507377/bc943ab5-9d39-43ee-b2a3-92e0a4e5d829" width="400" height="255">

## How we built it
We expanded upon the capabilities of TensorFlow's hand-pose model, integrating it with a Chrome extension framework. The extension processes live video feed from the webcam, analyzing hand positions and movements. Through meticulous programming and optimization, we mapped specific gestures to browser actions, ensuring a smooth and responsive user experience.

## Challenges we ran into
Developing an intuitive gesture recognition system that could accurately interpret a wide range of human hand movements was our biggest challenge. We had to balance sensitivity and specificity to minimize false positives and negatives. Additionally, optimizing the extension for low-latency performance without overwhelming the user's CPU posed significant technical hurdles.

## Accomplishments that we're proud of
We're particularly proud of creating an extension that enhances the browsing experience. Achieving a high degree of accuracy in gesture recognition, thereby reducing the learning curve for users, stands as a testament to our team's dedication and technical prowess.

## What we learned
This project deepened our understanding of machine learning models, especially in real-time applications. We gained invaluable insights into optimizing performance for live video processing and the importance of a user-centric design approach in developing new technologies.

## What's next for Swipe
Building on our foundation, we aim to introduce more complex gestures and motion controls to cover a broader spectrum of commands. Additionally, we're exploring the development of our own supplementary machine learning model to enhance gesture recognition accuracy and introduce new functionalities that could further transform user interaction with digital devices.

 --------------------------

## Installing

1. Check if your `Node.js` version is >= **14**.
2. Change or configurate the name of your extension on `src/manifest`.
3. Run `npm install` to install the dependencies.

## Developing

run the command

```shell
$ cd swipe

$ npm run dev
```

### Chrome Extension Developer Mode

1. set your Chrome browser 'Developer mode' up
2. click 'Load unpacked', and select `swipe/build` folder

### Nomal FrontEnd Developer Mode

1. access `http://0.0.0.0:3000/`
2. when debugging popup page, open `http://0.0.0.0:3000//popup.html`
3. when debugging options page, open `http://0.0.0.0:3000//options.html`

## Packing

After the development of your extension run the command

```shell
$ npm run build
```

Now, the content of `build` folder will be the extension ready to be submitted to the Chrome Web Store. Just take a look at the [official guide](https://developer.chrome.com/webstore/publish) to more infos about publishing.

---

Generated by [create-chrome-ext](https://github.com/guocaoyi/create-chrome-ext)
