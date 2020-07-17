# SMACSS and Responsive Web Design

**Responsive web design** is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.

### Responsive vs. Adaptive vs. Mobile

![](https://www.richswebdesign.com/wp-content/uploads/2018/04/AWR-vs-RWD.png)

Currently the most popular technique lies within responsive web design, favoring design that dynamically adapts to different browser and device viewports, changing layout and content along the way.

### Flexible Layouts
flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.

##### Relative Viewport Lengths

| relative length unit | what does it represent |
| ------------- | ------------- |
| vw | Viewports width |
| vh | Viewports height |
| vmin | Minimum of the viewport’s height and width |
| vmax | Maximum of the viewport’s height and width |

##### Flexible Grid

Using the flexible grid formula we can take all of the fixed units of length and turn them into relative units.

- **Note** : Taking the flexible layout concept, and formula, and reapplying it to all parts of a grid will create a completely dynamic website, scaling to every viewport size.

##### Media Queries

- Media queries were built as an extension to media types commonly found when targeting and including styles.

- There are a couple different ways to use media queries, using the `@media` rule inside of an existing style sheet, importing a new style sheet using the `@import` rule, or by linking to a separate style sheet from within the HTML document.

- There are three different logical operators available for use within media queries, including and, not, and only.

###### Media Features in Media Queries
1. Height & Width Media Features
2. Orientation Media Feature
3. Aspect Ratio Media Features
4. Pixel Ratio Media Features
5. Resolution Media Feature
6. Media Query Browser Support

##### Flexible Media

As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.

#### All About Floats

**Float** is a CSS positioning property. 
**What are floats used for?**
Aside from the simple example of wrapping text around images, floats can be used to create entire web layouts.

![](https://css-tricks.com/wp-content/csstricks-uploads/web-layout.png)

**Clearing the Float** 
Float’s sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float. Again an illustration probably does more good than words do.

![](https://css-tricks.com/wp-content/csstricks-uploads/unclearedfooter.png)
![](https://css-tricks.com/wp-content/csstricks-uploads/clearedfooter.png)

**Note** : Collapsing almost always needs to be dealt with to prevent strange layout and cross-browser problems. We fix it by clearing the float after the floated elements in the container but before the close of the container.

##### SMACSS
SMACSS is a way to examine your design process and as a way to fit those rigid frameworks into a flexible thought process. It is an attempt to document a consistent approach to site development when using CSS.