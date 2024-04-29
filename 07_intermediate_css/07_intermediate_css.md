# Intermediate CSS

## The Cascade: Specificity & Inheritance

What happens if you have conflicting rules targeting a single element?

- The lowest level rule is the one that takes precedence

Take this HTML:

```html
<ol>
  <li>One</li>
  <li style="color: red">Two</li>
</ol>
```

With this CSS

```css
li {
  color: green;
}
```

The list item with the "Two" content will display red as it is the lowest level.

### Position

```css
li {
  color: red;
  color: blue;
}
```

Both attributes are applied, but the `color: blue;` is applied last, therefore it will take precedence.

### Specificty

Take this HTML

```html
<li id="first_id" class="first_class" draggable>One</li>
```

With this CSS:

```css
li {
  color: blue;
}
.first_class {
  color: red;
}
li[draggable] {
  color: purple;
}
#first_id {
  color: orange;
}
```

Here there is multiple parts of CSS targetting the selector.

Specificity is important when determining what will be applied.

The order of precedence is as follows:

1. Element Selector
1. Class Selector
1. Attribute Selector (some sources will say class aand attribute are on the same level)
1. ID Selector

### Type

CSS can be applied in 3 ways. If CSS is applied in multiple ways, there is an order of precedence.

The order of precedence is as follows:

1. External
1. Internal
1. Inline

### Importance

```css
color: red;
color: green !important;
```

The !importance flag overrides everything.

### Exercise

![goal](./src/7.0%20CSS%20Cascade/goal.png)

See [answer](./src/7.0%20CSS%20Cascade/index.html)

## Grouping CSS Selectors

There are different ways of grouping multiple selectors

1. Grouping
1. Child
   1. Apply to direct child only
1. Descendant
   1. Apply to all descendants
1. Chaining
   1. Apply where all are true

### Exercise

1. Use a group combination to change the h1 and h2 color to blue violet
1. Set the first paragraph tag to a firebrick color using a child combination
1. Set the 3 bullet points using the descendant combination
1. Only select the last two bullet points and turn them seagreen
1. Turn the other item bullet point 0.5rem

See [answer](./src/7.1%20Combining%20Selectors/index.html)
