# Getting Started with React Native

Welcome to the world of mobile development! :tada:
In this repository, we will cover the steps needed to setup your environment and create and compile your first React Native Application.
Don't hesitate to refer to the documentations of [react native](https://reactnative.dev/docs/getting-started) and [expo](https://docs.expo.dev/) if needed.

## Environment Setup

Before you start, make sure you have a greater version than `v12` of `NodeJS` installed on your computer by running this command:

```
$ node -v
```

If you don't, install a suitable version of [NodeJS](https://nodejs.org/en/).

- Install Expo CLI

With that out of the way, you can now install `expo-cli` as a global dependency using either `npm` or `yarn`. Expo CLI is a command line app that is the main interface between a developer and Expo tools

```
# using npm
$ npm install -g expo-cli
```

You can check that the installation was successful by running

```
$ expo whoami
```

- Create an account on `expo`

Navigate to [expo.dev](https://expo.dev/) and sign up. Or, if you are a Terminal lover you register to `expo` by running:

```
$ expo register
```

Now that the account is created, you need to login to expo-cli on your local machine to be able to host your projects on expo platform

```
$ expo login
```

- Install Expo Go

Expo Go is a mobile application available on [iOS](https://itunes.com/apps/exponent) and [Android](https://play.google.com/store/apps/details?id=host.exp.exponent). It will allow us to open our projects created with expo-cli on mobile devices.

After downloading the app, you can login to your expo account. There, you can find the list of all your projects.

## Hello World

### Create your first React Native Project

- Navigate to a directory you choose and run the following command to create a new project with expo

```
$ expo init hello_world
```

A new directory will be created containing an empty React Native project.

### Start the Project

- Move to the project directory and open Terminal inside of it.
- Run the project with the following command

```
$ npm start
```

### Inspect and Debug the Project

A QR code will be displayed in the terminal console.

- Open Expo Go app on your phone and scan the code with it. Make sure your phone and computer are on the same LAN.

You'll see the page in your phone.

- If you want to debug or inspect an element, you can give your phone a small `shake` (yes, you read it well) and a menu will appear.

- Click on `Show element inspector`. You can now inspect any element on the screen or follow the requests being sent thanks to the `Network` tab in the developer tools.

- To close the **element inspector**, you can shake your Create a Hello World Application device again and click on `Hide element inspector`

- To open your project on **the browser**, you can run `npm start` and then click on `w`

- To open the **expo developer tools**, you can click on `d` after running `npm start`

- You can also install **emulators** on your Computer if you can't access a phone. Follow these steps to:

  - [Setup an Android Emulator](https://docs.expo.dev/workflow/android-studio-emulator/)
  - [Setup an iOS Emulator](https://docs.expo.dev/workflow/ios-simulator/). You'll need a MAC for this.
  - You can target the emulator after running `expo start` by clicking on `a` or `i`

### Update your project:

For this exercise, we will just update the existing `App` component return a `Hello World` message

- Update the `return` of the `App` component to return a `Text` that says `Hello World`
- Update the `style` of the text to be `bold` and `red`

Feel free to discover the [Components and APIs](https://reactnative.dev/docs/components-and-apisComponents) provided by React Native and creating more components other than the `App` component and complex layouts.
