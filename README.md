# react-native-emoji-keyboard

.

## Usage

```js
import EmojiPicker from '{package-name}';

export default function App() {
  const [isOpen, setIsOpen] = React.useState<boolean>(false);

  const handlePick = (emojiObject: EmojiType) => {
    console.log(emojiObject);
    /* example emojiObject = {    {
        "emoji": "❤️",
        "name": "red heart",
        "slug": "red_heart",
        "skin_tone_support": false,
        "unicode_version": "0.6",
        "emoji_version": "0.6"
      },
    */
  };

  return (
    <EmojiPicker
      onEmojiSelected={handleSelect}
      open={isOpen}
      onClose={() => setIsOpen(false)} />
  )
}
```

## Installation
```sh
yarn add {package-name}
```

or

```sh
npm install {package-name}
```
## Full Example
```js
TODO
```
## Accepted props (current implemented)
| Name | Type | Default Value | Required | Description |
|---|---|---|---|---|
| onEmojiSelected | function | undefined | yes | Callback on emoji selected |
| open | boolean | false | yes | Opens modal picker |
| onClose | function | undefined | yes | Request close modal *runs when onEmojiSelected or backdrop pressed* |
| emojiSize | number | 28 | no | Custom emoji size |
| headerStyles | TextStyle | {} | no | Override category name styles |
| knobStyles | ViewStyle | {} | no | Override knob styles |
| containerStyles | ViewStyle | {} | no | Override container styles |
| hideHeader | boolean | false | no | Hide category names | 
| expandable | boolean | true | no | Show knob and enable expand on swipe up |
| defaultHeight | number | 0.4 | no | Specify collapsed container height (1 is full screen height) |
| expandedHeight | number | 0.8 | no | Specify expanded container height (1 is full screen height) *only if expandable is true* |
| backdropColor | string | "#00000055" | no | Change backdrop color and alpha |
## License
 **MIT**

<br /><br /><br />
## TODO
categories => Specify displayed categories 

language => Use translation