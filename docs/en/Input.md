# Input
A basic widget for getting the user input is a text field.

## Props
| Prop | Type | Default | Note |
|---|---|---|---|
| [TextInput props...](https://facebook.github.io/react-native/docs/textinput.html) |  |  | Input inherits all the properties of the TextInput
| size | string | 'md' | - lg: large<br/>- md: medium<br/>- sm: small
| disabled | bool | false | Tell if the input is disabled
| underlineColorAndroid | string | 'rgba(0, 0, 0, 0)' | Inherited from TextInput and modify the default values.

## Events
| Event Name | Returns | Notes |
|---|---|---|
| [TextInput props...](https://facebook.github.io/react-native/docs/textinput.html) |  |  | Input inherits all the properties of the TextInput

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
<Input style={{  width: 200  }} />
```

Using the value and size attributes
```js
<Input
  style={{  width: 200  }}
  size="lg"
  value={this.state.value}
  onChangeText={value => this.setState({ value })}
/>
```

Read only
```js
<Input style={{  width: 200  }} editable={false} />
```

Disabled
```js
<Input style={{  width: 200  }} disabled />
```

Customize style
```js
<Input
  style={{  width: 200 , backgroundColor: '#fcf8e3', borderColor: '#8a6d3b', color: '#8a6d3b', textAlign: 'right' }}
  value={this.state.valueCustom}
  onChangeText={value => this.setState({ value })}
/>
```


## Screenshots
![](https://github.com/rilyu/teaset/blob/master/screenshots/04-Input.png?raw=true)
