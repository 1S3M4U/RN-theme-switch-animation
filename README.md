# react-native-theme-switch-animation

A Plug & Play Animations for Switching (Dark/Light) themes. 🌗

### 🦄 Features
- ✅  Supports multiple animation types.
- ✅  Blazing fast - [60/120]fps
- ✅  Plug and Play, doesn't matter whay you use for switching themes 
- ✅  Can be used for different theme colors, not necessarly for dark/light
  
<p align="center">
<img src="https://github.com/WadhahEssam/react-native-theme-switch-animation/assets/24798045/54ea2110-0c5b-42ca-9e6e-75e0e787ad1f" width="600"/>
</p>

## Installation

```sh
npm install react-native-theme-switch-animation
```
OR
```sh
yarn add react-native-theme-switch-animation
```

## Link
(if you are using expo managed project, do a prebuild - `npx expo prebuild`)
```
npx pod-install
```

## Usage

```js
import switchTheme from 'react-native-theme-switch-animation';

export default function Example() {
  const [theme, setTheme] = React.useState('light');

  return (
    <Button
      title="Switch Theme"
      onPress={() => {

        switchTheme({
          switchThemeFunction: () => {
            setTheme(theme === 'light' ? 'dark' : 'light'); // your switch theme function
          },
          animationConfig: {
            type: 'fade',
            duration: 900,
          },
        });

      }}
    />
  );
}
```



## License

MIT

