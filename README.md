What is React Theme Provider?

A generic theme provider and (very) simple CSS styler

now it is under development, see live demo, and this README

scheme
Use React Theme Provider in follow cases:
if you don't use Material-UI:

    Provide the theme data to your React Components via context. You don't need to have Material-UI in dependencies if you just want to pass your created theme to your non Material-UI components.
    Add style to your html elements - it will be based on your theme settings.
    Switch your created themes via API.

if you use Material-UI:

    Add simple style to you non material html elements. They will have same appearance with the marerial ones if wrapped in this provider.
    Override some part of your app with another theme.
    Have an API to switch themes on the client side.

What is Theme?
It's just plain javascript object, typically with two levels of nesting.

Usage

    install

npm i react-theme-provider --save

    import

import ThemeProvider from 'react-theme-provider';

    wrap

<ThemeProvider>
  <YourThemedComponentOrPlainHTML />
</ThemeProvider>

