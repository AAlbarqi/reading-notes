# CSS Transforms, Transitions, and Animations

#### 2D Transforms
![](https://www.ekioh.com/wp-content/uploads/opacity.gif)
##### Transform Syntax
`div {`
  `-webkit-transform: scale(1.5);`
     `-moz-transform: scale(1.5);`
       `-o-transform: scale(1.5);`
          `transform: scale(1.5);`
`}`

##### 2D Rotate
HTML
`<figure class="box-1">Box 1</figure>`
CSS
`.box-1 {transform: rotate(20deg);}`
##### 2D Scale
CSS
`.box-1 { transform: scale(.75);}`
##### 2D Translate
CSS
`.box-1 {transform: translateX(-10px);}`
##### 2D Skew
CSS
`.box-3 {transform: skew(5deg, -20deg);}`

#### 3D Transforms

![](https://i2.wp.com/css-tricks.com/wp-content/uploads/2017/06/cube_min_ani.gif)

##### 3D Rotate

- `.box-1 {transform: perspective(200px) rotateX(45deg);}`
- `.box-2 {transform: perspective(200px) rotateY(45deg);}`
- `.box-3 {transform: perspective(200px) rotateZ(45deg);}`

##### 3D Scale
`.box-1 {transform: perspective(200px) scaleZ(1.75) rotateX(45deg);}`

##### 3D Translate
`.box-1 {transform: perspective(200px) translateZ(-50px);}`

##### 3D Skew
- Skew is the one two-dimensional transform that cannot be transformed on a three-dimensional scale.
