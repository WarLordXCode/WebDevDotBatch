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
