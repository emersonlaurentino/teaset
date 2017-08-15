# Select
Select

## Props
| Prop | Type | Default | Note |
|---|---|---|---|
| [TouchableOpacity props...](https://facebook.github.io/react-native/docs/touchableopacity.html) |  |  | Select inherits all the properties of the TouchableOpacity
| size | string | 'md' | - lg: large<br/>- md: medium<br/>- sm: small
| value | any |  | 
| valueStyle | Text.style |  | 
| items | array |  | You can select an array of arrays, and the array elements can be of any type
| getItemValue | func |  | Take the value of the items array element, the incoming parameters are (item, index), item = items [index], the default direct use of item
| getItemText | func |  | 
| pickerType | string | 'auto' | - auto<br/>- pull<br/>- popover
| pickerTitle | string |  | 
| editable | bool | true | Whether it can be edited
| iconTintColor | string |  | 
| placeholder | string |  | 
| placeholderTextColor | string |  | 

## Events
| Event Name | Returns | Notes |
|---|---|---|
| [TouchableOpacity events...](https://facebook.github.io/react-native/docs/touchableopacity.html) |  | Select inherits all the properties of the TouchableOpacity
| onSelected | (item, index) | When the selector chooses an item array when an item is called, item = items [index]

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
this.items = [
  'Apple',
  'Banana',
  'Cherry',
  'Durian',
  'Filbert',
  'Grape',
  'Hickory',
  'Lemon',
  'Mango',
];

<Select
  style={{  width: 200  }}
  value={this.state.value}
  items={this.items}
  placeholder='Select item'
  pickerTitle='Default'
  onSelected={(item, index) => this.setState({ value: item })}
/>
```

Customize
```js
this.customItems = [
  {
    text: 'Long long long long long long long',
    value: 1,
  },
  {
    text: 'Short',
    value: 2,
  }
];

<Select
  style={{ width: 200, backgroundColor: '#fcf8e3', borderColor: '#8a6d3b'}}
  value={this.state.valueCustom}
  valueStyle={{ flex: 1, color: '#8a6d3b', textAlign: 'right' }}
  items={this.customItems}
  getItemValue={(item, index) => item.value}
  getItemText={(item, index) => item.text}
  iconTintColor='#8a6d3b'
  placeholder='Select item'
  pickerTitle='Custom'
  onSelected={(item, index) => this.setState({ valueCustom: item.value })}
/>
```


## Screenshots
![](https://github.com/rilyu/teaset/blob/master/screenshots/05-Select1.png?raw=true) ![](https://github.com/rilyu/teaset/blob/master/screenshots/05-Select2.png?raw=true)
![](https://github.com/rilyu/teaset/blob/master/screenshots/05-Select3.png?raw=true)
