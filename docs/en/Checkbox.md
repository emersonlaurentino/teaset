# Checkbox
Checkbox

## Props
| Prop | Type | Default | Note |
|---|---|---|---|
| [TouchableOpacity props...](https://facebook.github.io/react-native/docs/touchableopacity.html) |  |  | Checkbox inherits all the properties of the TouchableOpacity
| checked | bool | false | Specifies whether the checkbox is selected |
| size | string | 'md' | - lg: large<br/>- md: medium<br/>- sm: small
| title | string<br/>number<br/>element |  | 
| titleStyle | Text.style |  | The title style is invalid when the title type is element
| checkedIcon | Image.source<br/>element |  | 
| checkedIconStyle | Image.style |  | 
| uncheckedIcon | Image.source<br/>element |   | 
| uncheckedIconStyle | Image.style |  | 
| disabled | bool | false | Inherited from TouchableOpacity, true when the component is displayed as translucent and not touchable
| hitSlop | TouchableOpacity.hitSlop | {top: 8, bottom: 8,<br/>left: 8, right: 8} | Inherited from TouchableOpacity and modify the default values.

## Events
| Event Name | Returns | Notes |
|---|---|---|
| [TouchableOpacity props...](https://facebook.github.io/react-native/docs/touchableopacity.html) |  |  | Checkbox inherits all the properties of the TouchableOpacity
| onChange | checked | When the checked state changes, the value is modified

## Example
Simple usage
```js
<Checkbox
  title='Default'
  checked={this.state.checked}
  onChange={checked => this.setState({checked})}
/>
```

Use the size attribute
```js
<Checkbox
  title='Large'
  size='lg'
  checked={this.state.checked}
  onChange={checked => this.setState({checked})}
/>
```

Customize style
```js
<Checkbox
  title='Custom'
  titleStyle={{color: '#8a6d3b', paddingLeft: 4}}
  checkedIcon={(<Image style={{width: 15, height: 15, tintColor: '#8a6d3b'}} source={require('../icons/checkbox_checked.png')} />)}
  uncheckedIcon={(<Image style={{width: 15, height: 15, tintColor: '#8a6d3b'}} source={require('../icons/checkbox_unchecked.png')} />)}
  checked={this.state.checkedCustom}
  onChange={checked => this.setState({checkedCustom: checked})}
/>
```


## Screenshots
![](https://github.com/rilyu/teaset/blob/master/screenshots/03-Checkbox.png?raw=true)
