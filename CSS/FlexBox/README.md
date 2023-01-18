# Flexbox

## Table of Contents

1. [Introduction](#flexbox-intro)
1. [Flex Container & Flex Items](#flex-container-and-flex-items)
1. [Immediate Child Only](#immediate-child-only)
1. [Flexbox Axes](#flexbox-axes)
1. [Flexbox Module](#flexbox-module)
1. [Parent Properties](#parent-properties)
1. [Display](#display)
1. [block vs inline](#block-vs-inline)
1. [flex-direction](#flex-direction)
1. [flex-wrap](#flex-wrap)
1. [flex-flow](#flex-flow)
1. [justify-content [row]](#justify-content-row)
1. [justify-content [column]](#justify-content-column)
1. [space-around vs space-evenly](#space-around-vs-space-evenly)
1. [align-items [row]](#align-items-row)
1. [baseline](#baseline)
1. [align-items [column]](#align-items-column)
1. [align-content](#align-content)
1. [Child Properties](#child-properties)
1. [order](#order)
1. [flex-grow](#flex-grow)
1. [flex-grow calculation](#flex-grow-calculation)
1. [flex-shrink](#flex-shrink)
1. [flex-shrink calculation](#flex-shrink-calculation)
1. [flex-basis](#flex-basis)
1. [flex-basis vs widths](#flex-basis-vs-widths)
1. [flex](#flex)
1. [align-self](#align-self)
1. [Flexbox Properties](#flexbox-properties)
1. [Flexbox Cheatsheet](#flexbox-cheatsheet)
1. [Aligning with Auto Margins](#bonus-aligning-with-auto-margins)

## #flexbox-intro

### CSS Flex Box

The CSS flexbox is used to make the elements behave predictably when they are used with different screen sizes and different display devices. It provides a more efficient way to layout, align and distribute space among items in the container.

It is mainly used to make CSS3 capable to change its item?s width and height to best fit for all available spaces. It is preferred over block model.

The CSS3 flexbox contains flex containers and flex items.

---

## #flex-container-and-flex-items

### Flex Conatainer (Parent Element)

This is a flex container (the blue area) with three flex items:

![1673962524323](image/README/1673962524323.png)

The flex container becomes flexible by setting the `display` property to `flex`:

###### Example :

```css
.flex-container {
  display: flex;
}
```

The flex container properties are:

- `flex-direction`
- `flex-wrap`
- `flex-flow`
- `justify-content`
- `align-items`
- `align-content`

---

### Flex Item(Child Elements)

The direct child elements of a flex container automatically becomes flexible (flex) items.

![1673965561746](image/README/1673965561746.png)

The element above represents four blue flex items inside a grey flex container.

```html
<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>
  <div>4</div>
</div>
```

The flex item properties are:

- `order`
- `flex-grow`
- `flex-shrink`
- `flex-basis`
- `flex`
- `align-self`

---

## #immediate-child-only

### What is CSS immediate child?

The CSS child combinator `(>)` can be used to select all elements that are the immediate children of a specified element.

A combinator combines and explains the relationship between two or more selectors

One VERY important thing I want to point out is that the flex container only wraps around its immediate children. The flex container doesn't wrap beyond one layer deep. Only the immediate children. So there is NOT a grandchildren or grand-grandchildren relationship. Only Parent ↔️ Immediate Children!

Of course, you can establish a Flexbox as long as there is a parent-child relationship. So a child can also be the flex container to its children. But it will be a separate flex container. And it doesn't carry over the grandparent flex properties.

This is probably one of the most important concepts that helped me understand how Flexbox works. And knowing this will help solve a lot of those "hey, why isn't this working" moments 😅

### Syntax

```css

selector1 > selector2 { style properties }

```

It matches only those elements matched by the second selector (`selector2`) that are the direct children of elements matched by the first selector (`selector1`).

### Example

In this example, add a background-color property to all the immediate child (`p`) elements of the parent (`div`) element.

```html
<div>
  <p>1. Immeditate child.</p>
  <p>2. Immeditate child.</p>
  <section><p>3. Not immeditate child.</p></section>
  <!-- not Child but Descendant -->
  <p>4. Immeditate child.</p>
</div>
```

```css
/* p elements that are immediate
   children of div elements */
div > p {
  background-color: plum;
}
```

### Output

![1674046570719](image/README/1674046570719.png)

### Notice\*

Notice that the CSS property does not apply to the third p element as it is not an immediate child.

---

## Flexbox Axes

## #flexbox-axes

Flexbox operates in a 2 axes system: a main and a cross axis. The main axis is your defining direction of how your flex items are placed in the flex container. Determining the cross axis is very simple, it's in the direction that's perpendicular to your main axis.

CSS flexbox axes works on a vertical(cross-axes) and horizontal(main-axes) when coders need to move items around in their project. The code needed to work along the main-axes is “justify-content: {direction of the content}” and the cross axes code is “align-items: { direction of content }”.

![1674047641658](image/README/1674047641658.png)

### Example 1

In the example below, is flex box axes in action. Let say that you have square blocks of code as your items and your trying to determine how the justify-content on the main-axes. Using the “justify-content: flex-start”, begins on the main axes at the top of the page starting with block “one”.

```html
  <div class="box">
    <div>one</div>
    <div>two</div>
  </div>

```

```css
.box {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  height: 500px;
  border: 2px solid rgb(96, 139, 100);
}
```
### Output

![1674049118264](image/README/1674049118264.png)
### Example 2
In the example below, is flex box axes in action. Let say that you have square blocks of code as your items and your trying to determine how the justify-content on the main-axes. Using the “justify-content: flex-start”, begins on the main axes at the top of the page starting with block “one”.

```html
  <div class="box">
    <div>one</div>
    <div>two</div>
  </div>

```

```css
.box {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 500px;
  border: 2px solid rgb(96, 139, 100);
}
```
### Output

![1674049335892](image/README/1674049335892.png)

The “align-items:{direction of content}” have the same concept as the justify-content property but the difference is the align-items property works on cross-axes. For example, in the display below..if you wrote the “align-items: left”, this would push the items on the screen all the way to the left end to the width box.


```html
  <div class="box">
    <div>one</div>
    <div>two</div>
  </div>

```

```css
.box {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: left;
  height: 500px;
  border: 2px solid rgb(96, 139, 100);
}
```
### Output

![1674049523265](image/README/1674049523265.png)

Here in example #2, if you were to rewrite the code above and change to “align-items: center”, this would push the items to the center of the page.


```html
  <div class="box">
    <div>one</div>
    <div>two</div>
  </div>

```

```css
.box {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 500px;
  border: 2px solid rgb(96, 139, 100);
}
```
### Output

![1674049635538](image/README/1674049635538.png)

Overall the flexbox axes allows you move items using the “justify-content” (main-axes) or the “align-items” (cross-axes) property. Using these two properties can make the CSS3 experience rich when designing and creating a unique application.






