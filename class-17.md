# MUSTACHE and FLEXBOX

**Mustache** is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.
- Mustache is **NOT** a templating engine. Mustache is a specification for a templating language.

###### Mustache-Express

If you intend you use mustache with Node and Express, you can use mustache-express. Mustache Express lets you use Mustache and Express together easily.

###### FLEXBOX
Properties for the Parent (flex container):
1. display `.container {display: flex; /* or inline-flex */}`
2. flex-direction
![](https://css-tricks.com/wp-content/uploads/2018/10/flex-direction.svg)
3. flex-wrap
![](https://css-tricks.com/wp-content/uploads/2018/10/flex-wrap.svg)
4. flex-flow
`.container {flex-flow: column wrap;}`
5. justify-content
![](https://css-tricks.com/wp-content/uploads/2018/10/justify-content.svg)
6. Align items
![](https://css-tricks.com/wp-content/uploads/2018/10/align-items.svg)
7. align-content
![](https://css-tricks.com/wp-content/uploads/2018/10/align-content.svg)

###### Properties for the Children (flex items)
1. order 
![](https://css-tricks.com/wp-content/uploads/2018/10/order.svg)

2. flex-grow
![](https://css-tricks.com/wp-content/uploads/2018/10/flex-grow.svg)

3. flex-shrink 
`.item { flex-shrink: 3; /* default 1 */}`

4. flex-basis
`.item {flex-basis:  | auto; /* default auto */}`

5. flex 
`.item {flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]}`

6. align-slef
![](https://css-tricks.com/wp-content/uploads/2018/10/align-self.svg)
