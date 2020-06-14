# HTML Tables; JS Constructor Functions
## Tables
- **A table** represents information in a grid format.
`<table>
 <tr>
 <td>15</td>
 </tr>
 <tr>
 <td>45</td>
 </tr>
</table>`

| Tag |  Meaning |
| ------------- | ------------- |
| `<table>` | to create a table. |
| `<tr>` | indicate the start of each row |
| `<td>` | Each cell of a table is represented using a <td>|
| `<th>` | to represent the heading for either a column or a row.|
| `colspan` | indicates how many columns that cell should run across.|
| `rowspan` | indicate how many rows a cell should span down the table.|
| `<thead>` | The headings of the table should sit inside the <thead> element. |
| `<tbody>` | The body should sit inside the <tbody> element. |
| `<tfoot>` | The footer belongs inside the <tfoot> element. |

## Objects
#### Creating an object : Constructor Notation

- Creat an object:
1. LITERAL NOTATION
`var hotel = {} `
2. OBJECT CONSTRUCTOR NOTATION
`var hotel = new Object();` 
- Update an object: 
1. `hotel.name = 'park';`
2. `hotel['name'] = 'park';`

#### Creating an instance from an object 
- `var QuayHotel = new Hotel('Quay',40,25);`

#### DOM model

![](https://www.tutorialspoint.com/javascript/images/html-dom.jpg)

#### This
The keyword this is commonly used inside functions and objects.
Where the function is declared alters what this means. It always refers
to one object, usually the object in which the function operates.

#### SIMPLE OR PRIMITIVE DATA TYPES
JavaScript has five simple (or primitive) data types:
1. String
2. Number
3. Boolean
4. Undefined (a variable that has been declared, but no value has been assigned to it yet)
5. Null (a variable with no value - it may have had one at some point, but no longer has a value) 

#### Date object
`var today = new Date();`

#### Notes :
1. JavaScript also has several built-in objects such as
String, Number, Math, and Date. Their properties and
methods offer functionality that help you write scripts. 
2. Arrays and objects can be used to create complex data
sets (and both can contain the other). 
