## Bootstrap

### Container Class and Row Class

#### `.container`

Properties:
1. Centers the page.
2. Width is set to 1140px.

#### `.container-fluid`

Properties:
1. Width is set to 100%.

### Breakpoints

Bootstrap uses the following breakpoints for responsive design:

1. Extra Large (≥1200px)
2. Large (≥992px)
3. Medium (≥768px)
4. Small (≥576px)
5. Extra Small (<576px)

### Row Class

The `.row` class should always be used within a `.container` class.

### Col Class

The `.col` class is used within a `.row` class to create columns in your layout.

### Layout Class Sequence

The recommended sequence for creating a Bootstrap layout is as follows:

1. `.container`
   - Contains the entire page content.
2. `.row`
   - Used within a `.container` to create rows.
3. `.col`
   - Used within a `.row` to define columns in your layout.

Make sure to follow this sequence to create responsive and well-structured layouts using Bootstrap.

### W-100
used to break the col
### Row columns class
#### .row-cols-2 - > used to break the col after two col

### Grid col class
`Grid system` - In one row there will only 12 col
### Offset class
In Bootstrap, offset classes are used to create space or gaps on one side of a column. Offset classes are typically applied to columns to push them to the right or left, creating empty space next to them. This can be useful for achieving specific layout designs.

Here's how to use offset classes in Bootstrap:

To offset a column on larger screens (e.g., large or extra-large screens), you can use classes like `.offset-lg-*` or `.offset-xl-*`. The `*` should be replaced with the number of columns you want to offset. For example:

```html
<div class="container">
  <div class="row">
    <div class="col-md-6">Column 1</div>
    <div class="col-md-6">Column 2</div>
    <div class="col-md-6 offset-md-3">Offset Column 3</div>
  </div>
</div>
```
### UI output
![image](https://github.com/Niltiwari7/bootstrap/assets/93751356/ea55f95c-a24d-48d7-90d2-65d878601d0c)

### CSS order Classes
In Bootstrap, the `order` class is used to control the order of elements within a grid system, specifically in a flexbox-based layout. You can use the `order-*` class to specify the order in which a particular element should appear relative to its siblings.

Here's how it works:

1. By default, all elements within a Bootstrap row have an `order` value of 0, which means they appear in the order they are defined in the HTML markup.

2. You can use the `order-*` classes to change the order of specific elements. Elements with a higher `order` value will appear later in the order compared to elements with a lower `order` value.

Here's an example:

```html
<div class="container">
  <div class="row">
    <div class="col-md-4 order-2">Column 1</div>
    <div class="col-md-4 order-1">Column 2</div>
    <div class="col-md-4 order-3">Column 3</div>
  </div>
</div>
```

In the example above:

- `Column 1` has an `order` of 2, so it will appear after `Column 2`.
- `Column 2` has an `order` of 1, so it will appear before `Column 1`.
- `Column 3` has an `order` of 3, so it will appear last.

This feature is particularly useful for reordering elements in responsive layouts without changing the HTML structure. You can apply the `order` classes at different breakpoints to control the order at different screen sizes.





In the above example, the third column is offset by 3 columns, which means it will be pushed to the right by the width of 3 columns.
Remember to adjust the breakpoint prefix (e.g., `md`, `lg`, `xl`) and the number of columns to suit your specific layout needs. Offset classes are particularly useful when you want to create more complex and responsive grid layouts with Bootstrap.

### .m-auto class
In Bootstrap, the `.m-auto` class is used to horizontally center an element within its parent container. This class applies margin values to both the left and right sides of the element, effectively centering it horizontally.

Here's an example of how you can use the `.m-auto` class:

```html
<div class="container">
  <div class="row">
    <div class="col-6 mx-auto">
      <!-- Content here will be centered horizontally -->
      <p>This element is centered horizontally using .mx-auto.</p>
    </div>
  </div>
</div>
```

In the example above:

- `.col-6` is a Bootstrap column class that specifies the element's width to be half of its parent container's width.
- `mx-auto` is used to center the column horizontally within the parent container.

You can use the `.m-auto` class with various Bootstrap components, such as images, text, and other elements, to easily center them within their parent containers horizontally. It's a convenient way to achieve centering without needing to write custom CSS for each element.

#### .ml-auto
In Bootstrap, the `.ml-auto` class is used to add left margin (or margin-left) to an element, which pushes it to the right, effectively aligning it to the right edge of its parent container. This class is commonly used in conjunction with the Bootstrap grid system to create responsive layouts.

Here's an example of how you can use the `.ml-auto` class:

```html
<div class="container">
  <div class="row">
    <div class="col-6">Left Column</div>
    <div class="col-6 ml-auto">Right Column</div>
  </div>
</div>
```

In the example above:

- The `.col-6` class is used to create two equal-width columns within a Bootstrap row.
- The `ml-auto` class is applied to the second column (`Right Column`), which pushes it to the right, making it align with the right edge of its parent container.

This class is often used for creating layouts where you want one element to be on the left and another on the right, with the right-aligned element taking up any remaining space within its parent container. It's especially useful for responsive designs when you want columns to stack differently on smaller screens.
 
![image](https://github.com/Niltiwari7/bootstrap/assets/93751356/12f71663-667c-46e8-b750-22356def3808)

#### Padding for different class
![image](https://github.com/Niltiwari7/bootstrap/assets/93751356/7afa0737-bf85-4d22-b546-ade0f0033356)

![image](https://github.com/Niltiwari7/bootstrap/assets/93751356/ef190450-1e3a-47dc-822e-6e6ec5069707)
#### Negative margin
![image](https://github.com/Niltiwari7/bootstrap/assets/93751356/a5c9fa9f-2d65-48aa-95ff-f15aec4dfca5)

#### Padding
![image](https://github.com/Niltiwari7/bootstrap/assets/93751356/8e3cc52e-ac3e-4bc6-b271-2b817f55cbe1)

#### justify-content class

1. **`justify-content-start`**: This class aligns flex items to the start (left) of their container along the main axis. It's the default behavior if you don't apply any `justify-content` class.

2. **`justify-content-end`**: Aligns flex items to the end (right) of their container along the main axis.

3. **`justify-content-center`**: Centers flex items horizontally within their container along the main axis.

4. **`justify-content-between`**: Distributes flex items evenly along the main axis, with equal spacing between them and no space at the start or end.

5. **`justify-content-around`**: Distributes flex items evenly along the main axis, with equal spacing around them, including space at the start and end.

6. **`justify-content-evenly`**: Distributes flex items evenly along the main axis, with equal spacing around them, but no space at the start and end.

These classes are primarily used in combination with the Bootstrap grid system (rows and columns) to control the alignment of content within containers. They are particularly useful for creating responsive and neatly aligned layouts.

#### Align item class

1. **`align-items-start`**: Aligns flex items to the start (top) of their container along the cross-axis.

2. **`align-items-end`**: Aligns flex items to the end (bottom) of their container along the cross-axis.

3. **`align-items-center`**: Vertically centers flex items within their container along the cross-axis.

4. **`align-items-baseline`**: Aligns flex items such that their baselines (text baselines) are aligned along the cross-axis.

5. **`align-items-stretch`**: Stretches flex items to fill the entire height of their container along the cross-axis, making them equal in height.

These classes are used in combination with the Bootstrap grid system and flexbox-based components to control the vertical alignment of content within containers. They are valuable for creating responsive layouts and ensuring consistent vertical alignment of elements.

#### align-content-class

1. **`align-content-start`**: Aligns multiple lines of flex items at the start (top) of the flex container.

2. **`align-content-end`**: Aligns multiple lines of flex items at the end (bottom) of the flex container.

3. **`align-content-center`**: Vertically centers multiple lines of flex items within the flex container.

4. **`align-content-between`**: Distributes multiple lines of flex items evenly, with equal spacing between the lines, and no space at the start or end.

5. **`align-content-around`**: Distributes multiple lines of flex items evenly, with equal spacing around the lines, including space at the start and end.

6. **`align-content-stretch`**: Stretches multiple lines of flex items to fill the entire height of the flex container.

These classes are typically used when you have a flex container with multiple rows (lines) of flex items, and you want to control how those lines are aligned within the container along the cross-axis. They help you achieve various vertical alignment and spacing effects in your layouts.

#### align-self

Bootstrap provides several utility classes for manipulating the `align-self` property on individual flex items. Here are some key `align-self` classes in Bootstrap:

1. **`align-self-start`**: Aligns a specific flex item to the start (top) of the cross-axis within its container.

2. **`align-self-end`**: Aligns a specific flex item to the end (bottom) of the cross-axis within its container.

3. **`align-self-center`**: Vertically centers a specific flex item within its container along the cross-axis.

4. **`align-self-baseline`**: Aligns a specific flex item such that its baseline (text baseline) is aligned along the cross-axis.

5. **`align-self-stretch`**: Stretches a specific flex item to fill the entire height of its container along the cross-axis.

These classes are applied directly to the individual flex items (e.g., divs) within a flex container and allow you to control their vertical alignment independently. This can be particularly useful when you want specific items to have different vertical alignments within the same flex container.

#### Flex direction

![image](https://github.com/Niltiwari7/bootstrap/assets/93751356/ffba210b-dd95-4f27-87ce-bdacc1ce0147)
The `flex-direction` property in CSS is used to specify the direction in which flex items are laid out inside a flex container. It determines whether the items are laid out in a horizontal row or a vertical column, and whether they are arranged in the normal order or reversed.

Here are the possible values for the `flex-direction` property:

1. **`row` (default)**: Flex items are laid out in a horizontal row from left to right.

2. **`row-reverse`**: Flex items are laid out in a horizontal row, but in reverse order, from right to left.

3. **`column`**: Flex items are laid out in a vertical column from top to bottom.

4. **`column-reverse`**: Flex items are laid out in a vertical column, but in reverse order, from bottom to top.

Here's an example of how to use `flex-direction` in CSS:

```css
.flex-container {
  display: flex;
  flex-direction: row; /* or any of the other values */
}
```

In this example, the `.flex-container` is set to be a flex container, and `flex-direction` is set to `row`, which is the default value. This means that the flex items within the container will be laid out horizontally from left to right.

Changing the `flex-direction` property can significantly impact the layout of your flex container, allowing you to create various arrangements of flex items, both horizontally and vertically, depending on your design requirements.

#### Display class

![image](https://github.com/Niltiwari7/bootstrap/assets/93751356/d62119a8-a3d8-47f6-8efa-e239e1156915)
In Bootstrap, the `display` classes are utility classes used to control the display property of elements. These classes allow you to change the way elements are displayed on different screen sizes using responsive design principles. Bootstrap provides a set of display classes for hiding or showing elements based on the screen size.

Here are some common `display` classes in Bootstrap:

1. **`.d-none`**: This class is used to hide an element on all screen sizes. It sets the `display` property to `none`, effectively removing the element from the layout.

2. **`.d-block`**: This class sets the `display` property to `block`, making the element a block-level element, which takes up the full width of its container.

3. **`.d-inline`**: This class sets the `display` property to `inline`, making the element inline with the surrounding content.

4. **`.d-inline-block`**: This class sets the `display` property to `inline-block`, making the element inline but allowing it to have block-level properties.

5. **`.d-md-none`**, **`.d-lg-block`**, etc.: These classes are responsive display classes that apply the specified display property only on specific screen sizes. For example, `.d-md-none` will hide the element on medium and larger screens.

6. **`.d-print-block`**: This class is used to display an element when the page is printed, making it visible in print media.

Here are some examples of how to use these classes:

```html
<div class="d-none">This is hidden on all screen sizes.</div>
<div class="d-block">This is a block-level element.</div>
<div class="d-md-none">This is hidden on medium and larger screens.</div>
<div class="d-print-block">This is visible when printing.</div>
```

These display classes are handy for building responsive web designs and controlling the visibility and layout of elements based on different screen sizes and media types.
#### Position

![image](https://github.com/Niltiwari7/bootstrap/assets/93751356/5ad625a9-3dba-4475-9358-6e6e60fdc886)
