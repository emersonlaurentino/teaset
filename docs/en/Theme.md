# Theme

Theme is a style definition object for Teaset that defines the default style for components.

Most of the components provided by Teaset support style definitions through the style attribute, which can be modified by code to modify the style of Teaset components. Based on the App Uniform style, it is recommended to modify the style of the Teaset component by redefining the properties of the Theme object.

Teaset provides [ThemeDefault.js](/themes/ThemeDefault.js), [ThemeBlack.js](/themes/ThemeBlack.js) and [ThemeViolet.js](/themes/ThemeViolet.js), you can customize the color scheme using one of the above options and modify some of the default values.

It is recommended that you set the Theme definition at the code entry. If you modify the Theme definition during the App run, you will need to reload the rendered page.
## Example
Modify collor theme
```js
import {Theme} from 'teaset';

Theme.set(Theme.themes.black);
```

Modify some of the default values
```js
import {Theme} from 'teaset';

Theme.set({
  primaryColor: '#f55e5d',
  backButtonTitle: '返回',
});

```

## Screenshots
![](https://github.com/rilyu/teaset/blob/master/screenshots/00a-Theme2.png?raw=true) ![](https://github.com/rilyu/teaset/blob/master/screenshots/00a-Theme3.png?raw=true)
