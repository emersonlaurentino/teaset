# Teaset
[🇨🇳 中文完整文档版](../cn/README.md)

React Native UI Component, more than 20 pure JS (ES6) components, focused on content display and operational control.

Teaset design is compact, do not rely on any third-party library, all the source code is compressed only 300 + k, even if the icon file is less than 600k, if only need to use a small number of components, you can also use the on-demand loading only need to use the components.

The Teaset component is written in the same style as React Native native components and can be seamlessly integrated with React Native. You do not need too much learning costs to master. Due to the use of pure JS development, so in iOS and Android under the form of almost the same.

With Teaset, you can quickly build App page, rich UI components to greatly improve the efficiency of page development, powerful Overlay floating layer of you from the cumbersome interactive control in the liberation, so you can focus on business and logic.


# Get started

## Install
```shell
npm install --save teaset
```

## Usage
```js
import { Label } from 'teaset';
ReactDOM.render(<Label size="xl" text="Hello world!" />, mountNode);
```
## Load on demand
```js
import Label from 'teaset/components/Label/Label';
```

## Development
```
$ git clone git@github.com:rilyu/teaset.git
$ cd teaset/example
$ npm install
```
Run on iOS:
```
react-native run-ios
```
Run on Android:
```
react-native run-android
```

## Customization
[Theme](./Theme.md)

## Basic
[Label](./Label.md)

[Button](./Button.md)

[Checkbox](./Checkbox.md)

[Input](./Input.md)

[Select](./Select.md)

[Stepper](./Stepper.md)

[SearchInput](./SearchInput.md)

[Badge](./Badge.md)

[Popover](./Popover.md)

## Composite
[NavigationBar](./NavigationBar.md)

[ListRow](./ListRow.md)

[Carousel](./Carousel.md)

[Projector](./Projector.md)

[SegmentedBar](./SegmentedBar.md)

[SegmentedView](./SegmentedView.md)

[TabView](./TabView.md)

[TransformView](./TransformView.md)

## Floating
[Overlay](./Overlay.md)

[Toast](./Toast.md)

[ActionSheet](./ActionSheet.md)

[ActionPopover](./ActionPopover.md)

[PullPicker](./PullPicker.md)

[PopoverPicker](./PopoverPicker.md)

[Menu](./Menu.md)

[Drawer](./Drawer.md)

[ModalIndicator](./ModalIndicator.md)

## Page
[TeaNavigator](./TeaNavigator.md)

[BasePage](./BasePage.md)

[NavigationPage](./NavigationPage.md)

# License
MIT