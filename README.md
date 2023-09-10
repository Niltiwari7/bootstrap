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

In the above example, the third column is offset by 3 columns, which means it will be pushed to the right by the width of 3 columns.

Remember to adjust the breakpoint prefix (e.g., `md`, `lg`, `xl`) and the number of columns to suit your specific layout needs. Offset classes are particularly useful when you want to create more complex and responsive grid layouts with Bootstrap.
