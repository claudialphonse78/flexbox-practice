 # Flexbox
>This is a practice repo for flexbox and exercises based on it

> A good guide for flex box is the [css tricks flexbox snippets](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

 We can use an emmet shortcut to do this
`.container>.box.box1*10`
- We are using `normailize.css` which resets the default browser settings to make  our code have the same look across browsers
- without flexbox the elements i.e. div tags are stacked on top of each other
![](images/02_00.png)
- To start using flexbox we simply have to write `display:flex` on the parent container
using flex we get and our flex container goes all the way across
![](images/01_00.png)
inline-flex will just wrap around the content
![](images/03_00.png)
- The parent container is called the **flex container** and the immediate children are called **flex items** and we dont explicitly need to define display flex on the children

### flex-direction
- In flexbox we have main and cross axis
- `flex-direction:row` is the default value and it goes from left to right 
- `flex-direction:column`stacks from top to bottom
- The min-height property in CSS is used to set the minimum height of a specified element. The min-height property always overrides both height and max-height
- When we use flex-direction  we get two axises : _main axis and cross axis_
Below is the depiction for main and cross axis when using `flex-direction:row`
![](images/05_00.png)

### flex-wrapping
- flex-wrap is put on the flex-container(parent) and not flex-item(immediate children)
- It's default value is `flex-wrap:nowrap`
- default flex items take the height of the element .and strtches to fit it
- To divide the screen into equal space for divs to avoid whitespace we  can use `100/3 viz 33.3333%` or just use calc() `width:calc(100% / 3);`
- if we put `flex-direction:column` and have a 100vh and wrap is set, it  wraps the elements within the screen space
- If we set height to min-height it will wrap cause min-height is set and height is not fixed

_without min-height and with in-height:_
![](images/06_00.png)

if we want to add margin then we can do 
`width:calc(33.3333% - 20px);` 20px cause 10px on either side left & right
![](images/07_00.png)

### flex-ordering
- `flex:1;` takes the width and evenly spreads it 
- We can set it on the `flex-items`,by default all are set to _zero_
`.box{order:0}` and when we do `.box{order:2}` it sets it at the end of last element with `order:0`
![](images/08_00.png)

Also works with negative values .box3{order:-1}
![](images/09_00.png)
- not to be used to copy texts but only to order certain elements