# Label
Used for text display, typically a single line of text.

## Props
| Prop | Type | Default | Note |
|---|---|---|---|
| [Text props...](https://facebook.github.io/react-native/docs/text.html) |  |  | Label inherits all the properties of the Text component.
| type | string | 'default' | - default: font-color: #333333<br/>- title: font-color: #000000, font-size: 1.1<br/>- detail: font-color: #898989, font-size: 0.9<br/>- danger: font-color: #a94442
| size | string | 'md' | - xl: oversized<br/>- lg: large<br/>- md: medium<br/>- sm: small<br/>- xs: tiny
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
