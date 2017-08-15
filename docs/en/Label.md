# Label
Used for text display, typically a single line of text.

## Props
| Prop | Type | Default | Note |
|---|---|---|---|
| [Text props...](https://facebook.github.io/react-native/docs/text.html) |  |  | Label inherits all the properties of the Text component.
| type | string | 'default' | - default: The font color defined is dark gray (#333)<br/>- title: The font color defined is black (#000), the font size is 1.1 times<br/>- detail: The font color defined is light gray (#989898), the font size is 0.9 times the default<br/>- danger: The font color defined is red
| size | string | 'md' | - xl: oversize, the size of the font defined is 26<br/>- lg: large, the size of the font defined is 20<br/>- md: default, the size of the font defined is 14<br/>- sm: small, the size of the font defined is 10<br/>- xs: tiny, the size of the font defined is 8
| text | string<br/>number |  | Display text
| numberOfLines | number | 1 | Show the number of rows

## Example
Simple usage
```js
<Label text='Hello world' />
```

Using the type and size attributes
```js
<Label type='title' size='xl' text='Hello world' />
```

Customize style
```js
<Label style={{color: '#8a6d3b', fontSize: 16}} text='Hello world' />
```

## Screenshots
![](https://github.com/rilyu/teaset/blob/master/screenshots/01-Label.png?raw=true)
