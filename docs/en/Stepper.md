# Stepper
Stepper

## Props
| Prop | Type | Default | Note |
|---|---|---|---|
| [View props...](https://facebook.github.io/react-native/docs/view.html) |  |  | Stepper inherits all the properties of the View
| defaultValue | number | 0 | Initial value
| value | number |  | Current value
| step | number | 1 | The step can be an integer or a decimal
| max | number |  | Maximun value
| min | number |  | Minimum value
| valueStyle | Text.style |  | Style of value
| valueFormat | func |  | Format the value of the function, the incoming parameter is value, the default direct use of value
| subButton | string<br/>element | '-' | The "Minimum" button can be a string or a React Native component.
| addButton | string<br/>element | '+' | The "Maximun" button can be a string or a React Native component.
| showSeparator | bool | true | Whether to display the separation between the button and the value of the line, for a complete customize component style can be set to false.
| disabled | bool | false | Tell if the input is disabled
| editable | bool | true | Whether it can be edited.

## Events
| Event Name | Returns | Notes |
|---|---|---|
| [View events...](https://facebook.github.io/react-native/docs/view.html) |  | Stepper inherits all the properties of the View
| onChange | value | Called when input value change

## Example
Simple usage
```js
<Stepper />
```

Using defaultValue, min and max
```js
<Stepper defaultValue={1} min={1} max={10} />
```

Using step and valueFormat
```js
<Stepper
  defaultValue={0.8}
  step={0.005}
  valueFormat={v => (v * 100).toFixed(1) + '%'}
  valueStyle={{ minWidth: 60 }}
/>
```

Customize style
```js
<Stepper
  style={{borderWidth: 0 }}
  value={this.state.valueCustom}
  valueStyle={{ color: '#8a6d3b' }}
  min={0}
  max={100}
  subButton={
    <View style={{ backgroundColor: '#fcf8e3', borderColor: '#8a6d3b', borderWidth: 1, borderRadius:4, width: 20, height: 20, alignItems: 'center', justifyContent: 'center' }}>
      <Text style={{ color: '#8a6d3b' }}>－</Text>
    </View>
  }
  addButton={
    <View style={{ backgroundColor: '#fcf8e3', borderColor: '#8a6d3b', borderWidth: 1, borderRadius:4, width: 20, height: 20, alignItems: 'center', justifyContent: 'center' }}>
      <Text style={{color: '#8a6d3b'}}>＋</Text>
    </View>
  }
  showSeparator={false}
  onChange={value => this.setState({ value })}
/>
```


## Screenshots
![](https://github.com/rilyu/teaset/blob/master/screenshots/05a-Stepper.png?raw=true)
