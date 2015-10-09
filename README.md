# react-scroll-up
React component to add custom button (it can be something what you want) for scroll to top of page


## Install

```npm
npm install react-scroll-up
```

## How to use it

You have to define children element, for example `<span>UP</span>`

```jsx
<ScrollToTop showUnder={160}>
  <span>UP</span>
</ScrollToTop>
```

## Parameters

### showUnder:number in px (required) 

What position (and below) the button will be displayed.

### topPosition:number in px (optional)

default: 0

The position to which the scrollbar be moved after clicked.

### easing:string (optional)

default: easeInCubic

Type of scrolling easing. You can specify some of this type of easing: https://github.com/chenglou/tween-functions

In graphical representation: http://sole.github.io/tween.js/examples/03_graphs.html

### duration:number in miliseconds (optional)

default: 250

Time to reach the `topPosition`

### style:object (optional)

default:  

```javascript
{
  position: 'fixed',
  bottom: 50,
  right: 30,
  cursor: 'pointer',
  transitionDuration: '0.2s',
  transitionTimingFunction: 'linear',
  transitionDelay: '0s'
}
```

You can specify you own style and position of the button.

Hide/show button is based on opacity, so this styles `opacity` and `transitionProperty` will be all time overwrite.

If you can positioned button to left site, you have to reset css property `right: 'auto'`, and similar.

