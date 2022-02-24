# Class-14a

## Read the following articles and/or review the following examples on CSS animations

## [Read this article on CSS Transforms](http://learn.shayhowe.com/advanced-html-css/css-transforms/)

- these are vendor prefixes used if the users browser doesn't support the transform property
  - -webkit-transform: scale(1.5);
  - -moz-transform: scale(1.5);
  - -o-transform: scale(1.5);

- transform: rotate(20 deg); will rotate the element clockwise
- transform: rotate(-20 deg); will rotate the element counter clockwise
- transform: scale(.75); will shrink or grow the element depending if the number is above or below zero
- transform: translate(-10px, 25%); will move the element specified by the amounts in the (). first number x axis, second is y axis
- Make a simple cube by using something similar to this in CSS and making the classes in html with cube as the container:
  - .cube {
      position: relative;
    }
  - .side {
      height: 95px;
      position: absolute;
      width: 95px;
    }
  - .top {
      background: #9acc53;
      transform: rotate(-45deg) skew(15deg, 15deg);
    }
  - .left {
      background: #8ec63f;
      transform: rotate(15deg) skew(15deg, 15deg) translate(-50%, 100%);
    }
  - .right {
      background: #80b239;
      transform: rotate(-15deg) skew(-15deg, -15deg) translate(50%, 100%);
    }

## [Read this article on CSS Transitions & Animations](http://learn.shayhowe.com/advanced-html-css/transitions-animations/)

- Animations and transitions are new with CSS3 and allow you to make elements move without javascript or flash
- Use this to get the element you wants background to change from red to blue over the duration of 3 seconds
  - .classname {
        background: red;
        transition-property: background;
        transition-duration: 3s;
        transition-timing-function: linear;
      }
      .classname:hover {
        background: blue;
      }

- What that code should look like using vendor prefixes
  - .box {
        background: #2db34a;
        -webkit-transition-property: background;
          -moz-transition-property: background;
            -o-transition-property: background;
                transition-property: background;
        -webkit-transition-duration: 1s;
          -moz-transition-duration: 1s;
            -o-transition-duration: 1s;
                transition-duration: 1s;
        -webkit-transition-timing-function: linear;
          -moz-transition-timing-function: linear;
            -o-transition-timing-function: linear;
                transition-timing-function: linear;
    }
  - .box:hover {
      background: #ff7b29;
    }

- Other trasitional properties. Can only transition if property has two trasnitionable properties of the same value type
  - background-color
  - background-position
  - border-color
  - border-width
  - border-spacing
  - bottom
  - clip
  - color
  - crop
  - font-size
  - font-weight
  - height
  - left
  - letter-spacing
  - line-height
  - margin
  - max-height
  - max-width
  - min-height
  - min-width
  - opacity
  - outline-color
  - outline-offset
  - outline-width
  - padding
  - right
  - text-indent
  - text-shadow
  - top
  - vertical-align
  - visibility
  - width
  - word-spacing
  - z-index

## [8 simple CSS3 transitions that will wow your users](http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)

- 8 transitions from article:
  1. Fade in
  2. Change color
  3. Grow & Shrink
  4. Rotate elements
  5. Square to circle
  6. 3D shadow
  7. Swing
  8. Inset border

## [6 Buttons animated](http://codepen.io/retyui/pen/ByoaXV)

## [CSS3 Animations: Keyframes](http://codepen.io/akshaychauhan/pen/oAfae)

## [404](http://codepen.io/kieranfivestars/pen/MYdQxX)

## [Pure CSS Bounce Animation](http://codepen.io/dp_lewis/pen/gCfBv)

- After playing with these animations, it was clear to me how cleverly some of them were set up, particularly the bouncing ball. If you adjust some of the settings just a little bit it makes the animation look off.
