<img alt="React Native Basic Modal" src="assets/logo.png" width="1050"/>

[![Battle Tested ✅](https://img.shields.io/badge/-Battle--Tested%20%E2%9C%85-03666e?style=for-the-badge)](https://github.com/WrathChaos/react-native-basic-modal)

[![Basic & Elegant UI Modal for React Native](https://img.shields.io/badge/-Basic%20%26%20Elegant%20UI%20Modal%20for%20React%20Native-lightgrey?style=for-the-badge)](https://github.com/WrathChaos/react-native-basic-modal)

[![npm version](https://img.shields.io/npm/v/react-native-basic-modal.svg?style=for-the-badge)](https://www.npmjs.com/package/react-native-basic-modal)
[![npm](https://img.shields.io/npm/dt/react-native-basic-modal.svg?style=for-the-badge)](https://www.npmjs.com/package/react-native-basic-modal)
![Platform - Android and iOS](https://img.shields.io/badge/platform-Android%20%7C%20iOS-blue.svg?style=for-the-badge)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![styled with prettier](https://img.shields.io/badge/styled_with-prettier-ff69b4.svg?style=for-the-badge)](https://github.com/prettier/prettier)

<p align="center">
  <img alt="React Native Basic Modal"
        src="assets/Screenshots/example.png" />
</p>

# Installation

Add the dependency:

```ruby
npm i react-native-basic-modal
```

## Peer Dependencies

###### IMPORTANT! You need install them

```js
"react": ">= 16.x.x",
"react-native": ">= 0.55.x",
"react-native-modal": ">= 11.4.0"
```

# Usage

## Import

```js
import BasicModal from "react-native-basic-modal";
```

## Default Usage

```js
<BasicModal isVisible />
```


## Customizable Usage

```js
<BasicModal 
  isVisible
  title="Warning!" 
  desciption="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book."
  firstButtonOnPress={()=> {}}  
  secondButtonOnPress={()=> {}}  
/>
```

### How can I hide the modal by pressing outside of its content?

The prop `onBackdropPress` allows you to handle this situation:

```javascript
<BasicModal
  isVisible={this.state.isVisible}
  onBackdropPress={() => this.setState({ isVisible: false })}
/>
```

# For more FAQ about Modal: 

## [Modal FAQ](https://github.com/react-native-community/react-native-modal#frequently-asked-questions)

# Configuration - Props

| Property                    |   Type    |  Default  | Description                                  |
| --------------------------- | :-------: | :-------: | -------------------------------------------- |
| width                       |  number   |    90%    | change the modal's width                     |
| height                      |  number   |    185    | change the modal's height                    |
| isVisible                   |   bool    |   false   | set the modal's visibility                   |
| title                       |  string   | Hold on!  | set your own title text                      |
| description                 |  string   | too long  | set your own description text                |
| titleColor                  |   color   |  #212121  | change the title's text color                |
| descColor                   |   color   |  #b5b5b5  | change the description's text color          |
| titleStyle                  |   style   |   style   | set your own style for title text            |
| descStyle                   |   style   |   style   | set your own style for description text      |
| backgroundColor             |   color   |   #fff    | change the modal's background color          |
| firstButtonText             |  string   |   SKIP    | set your own button text                     |
| secondButtonText            |   color   |   NEXT    | set your own button text                     |
| firstButtonTextColor        |   color   |   #fff    | change the first button's text color         |
| secondButtonTextColor       |   color   |   #fff    | change the second button's text color        |
| firstButtonBackgroundColor  |   color   |  #b5b6cf  | change the first button's background color   |
| secondButtonBackgroundColor |   color   |  #895aaf  | change the second button's background color  |
| firstButtonOnPress          | function  | undefined | set your own onPress function                |
| secondButtonOnPress         | function  | undefined | set your own onPress function                |
| firstButtonComponent        | component |  default  | set your own button component for first one  |
| secondButtonComponent       | component |  default  | set your own button component for second one |

## Future Plans

- [x] ~~LICENSE~~
- [ ] Halloween Theme
- [ ] Write an article about the lib on Medium

# Change Log

Change log will be here !

## Author

FreakyCoder, kurayogun@gmail.com

## License

React Native Basic Modal is available under the MIT license. See the LICENSE file for more info.
