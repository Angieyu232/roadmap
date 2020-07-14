# CSS basics


https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Floats

## Floats

The floats properties defines the inline position of a container. Allowing text and inline elements to wrap around it.

```

float: none;
float: left;
float: right;

```

## Positions

The position properties determines whether an element is static or relatively positioned.

relative refers to relative to its container;
sticky refer to the position of browser 

```
position: static;

position: -webkit-sticky;
position: sticky;
top: 20px;

```


## Flexbox

Displaying 60 box using felx-flow. 
flex-flow key value pair defines flex-direction and flex-wrap properties.

容器默认存在两根轴：水平的主轴（main axis）和垂直的交叉轴（cross axis）。主轴的开始位置（与边框的交叉点）叫做main start，结束位置叫做main end；


justify-content: property defines how the browser distributes space between and around content items along the main-axis of a flex container, and the inline axis of a grid container. 

```
body {
      margin: 0px;
      display: flex;
      flex-flow: row wrap;
    }

    .box {
      font-size: 3rem;
      color: #000;
      width: 9vw;
      min-width: 50px;
      height: 9vw;
      min-height: 50px;
      border: 3px #000 solid;
      margin: calc((1vw / 2) - 3px);
      display: flex;
      justify-content: center;
      align-items: center;
    }

    #two {
      background-color: #eee;
      position: static;
    }
```
## Display

The display value sets whether an element is treated as a block or inline element and the layout used for its children, such as flow layout, grid or flex.

```
div {
  display: inline;        /* Default of all elements, unless UA stylesheet overrides */
  display: inline-block;  /* Characteristics of block, but sits on a line */
  display: block;         /* UA stylesheet makes things like <div> and <section> block */
  display: run-in;        /* Not particularly well supported or common */
  display: none;          /* Hide */
}

```

## Overflow
when content of a container exceeds it size, how browser will handle the rest of the content.

```
overflow: hidden;
overflow: scroll;

```

Reference: https://developer.mozilla.org/en-US/docs/Web/CSS/


## Notes on CSS Box Model

- the width and height of an element include the content and padding, not margin
- inline element can not adjust height and width

**What these means is that:**
1. for in-line element with fixed height and width, adding a padding value, let's say 5px, would shrink the content size;
2. When you want content with fixed or assigned size e.g. 10%, do not mess with padding and adjust the margin instead


**Sound's like an inhumane design right?** Box-sizing comes to rescue

Here is a link to learn about box-sizing property: https://learnlayout.com/box-sizing.html
```css
* {
  -webkit-box-sizing: border-box;
     -moz-box-sizing: border-box;
          box-sizing: border-box;
}
```
Basically, with box-sizing property on an element, the padding and border of that element no longer increase its width.


## Media Queries
Although it's an increasing common practice to use SCSS and other css preprocessors tools to manipulate the Media Query, it's a good idea to start from the good old days of specified media breakpoint using css media queries to have a basic understanding how the underlying things work

Reference Link: https://learnlayout.com/media-queries.html

