# Button
To trigger an operation.

## Props
| Prop | Type | Default | Note |
|---|---|---|---|
| [TouchableOpacity props...](https://facebook.github.io/react-native/docs/touchableopacity.html) |  |  | Button inherits all the properties of the TouchableOpacity
| type | string | 'default' | - default<br/>- primary<br/>- secondary<br/>- danger<br/>- link
| size | string | 'md' | - xl: oversized<br/>- lg: large<br/>- md: medium<br/>- sm: small<br/>- xs: tiny
| title | string<br/>number<br/>element |  |
| titleStyle | Text.style |  | The title style is invalid when the title type is element
| disabled | bool | false | 

## Events
| Event Name | Returns | Notes |
|---|---|---|
| [TouchableOpacity props...](https://facebook.github.io/react-native/docs/touchableopacity.html) |  |  | Button inherits all the properties of the TouchableOpacity

<!--
## Methods
None.

## Static Props
None.

## Static Methods
None.
-->

## Example
Simple usage
```js
<Button title='Default' onPress={() => alert('Hello world')} />
```

Using the type and size attributes
```js
<Button type='primary' size='xl' title='Primary' />
```

Customize style
```js
<Button style={{backgroundColor: '#fcf8e3', borderColor: '#8a6d3b'}}>
  <Image style={{width: 16, height: 16, tintColor: '#8a6d3b'}} source={require('../icons/search.png')} />
  <Label style={{color: '#8a6d3b', fontSize: 16, paddingLeft: 8}} text='Search' />
</Button>
```


## Screenshots
![](https://github.com/rilyu/teaset/blob/master/screenshots/02-Button.png?raw=true)
