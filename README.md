# react-sidebar-ui

> Sidebar component for React projects with customizable design

[![NPM](https://img.shields.io/npm/v/react-sidebar-ui.svg)](https://www.npmjs.com/package/react-sidebar-ui) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

![React Sidebar UI Black](https://i.imgur.com/gXPJtJW.gif)
![React Sidebar UI Light](https://i.imgur.com/QT86Om0.gif)
![React Sidebar UI Blue](https://imgur.com/gHZQYo6.gif)
## Install

```bash
npm install --save react-sidebar-ui
```

## Usage

```jsx
import React from 'react'
import {Sidebar, InputItem, DropdownItem, Icon, Item, Logo, LogoText} from 'react-sidebar-ui'
import 'react-sidebar-ui/dist/index.css';

const App = () => {
  return (
    <div>
      <Sidebar bgColor='black' isCollapsed={false}>
        <Logo
          image='https://media2.giphy.com/media/eNAsjO55tPbgaor7ma/source.gif'
          imageName='react logo'/>
        <LogoText>React Sidebar UI</LogoText>
        <DropdownItem
          values={['First', 'Second', 'Third']}
          bgColor={'black'}>
          Menu
        </DropdownItem>

        <Item bgColor='black'>
          <Icon><i className="fas fa-home"/></Icon>
          Home
        </Item>
        <Item bgColor='black'>
          <Icon><i className="fas fa-info"/></Icon>
          About
        </Item>
        <Item bgColor='black'>
          <Icon><i className="fas fa-sitemap"/></Icon>
          My Website
        </Item>
        <Item bgColor='black'>
          <Icon><i className="far fa-address-book"/></Icon>
          Contacts
        </Item>
        <Item bgColor='black'>
          <Icon><i className="fas fa-rss-square"/></Icon>
          Blog
        </Item>
        <InputItem type='text' placeholder={'Search...'}/>
      </Sidebar>
    </div>
  )
};
```
You should import FontAwesome in order to use the icons.
## Props

Common props you may want to specify include:
### Sidebar
- `bgColor` - change the color of the sidebar it can be `black`, `light`, `blue`, `purple`, `aqua`, `peach`
- `isCollapsed` - add start position of the sidebar if it will be collapsed or not
- `classes` - add your custom classes if you want to add custom style to the component
### DropdownItem
- `bgColor` - change the color of the sidebar it can be `black`, `light`, `blue`, `purple`, `aqua`, `peach`
- `values` - items that will be displayed
- `classes` - add your custom classes if you want to add custom style to the component
### Item
- `bgColor` - change the color of the sidebar it can be `black`, `light`, `blue`, `purple`, `aqua`, `peach`
- `classes` - add your custom classes if you want to add custom style to the component
### Logo
- `image` - url to the image
- `imageText` - alt tag of the image
- `classes` - add your custom classes if you want to add custom style to the component
### InputItem
- `type` - type of the input field
- `placeholder` - placeholder of the input field
- `classes` - add your custom classes if you want to add custom style to the component

## Customization
If you want to change the style of a component, you can do it by adding your own classes to the component
## Contribute 
Contributions are always welcome!
Please read the [contribution guidelines](contributing.md) first.

### ⭐ If you liked the component, please consider giving me a star. Thank you!
## License

Copyright © [Svetloslav Novoselski](https://github.com/Svetloslav15)
