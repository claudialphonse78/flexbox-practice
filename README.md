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