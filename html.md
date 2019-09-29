# HTML  (Hypertext Markup Language)

- HTML is not a programming language; it is a markup language that defines the structure of a web page and its content.
- An HTML file is simply a text file saved with an .html or .htm extension 

## Getting Started

### Tags

- HTML tag is just opening or closing entity. Tags are used to mark up the start and end of an HTML element.
- For example: `<p> and </p>` are called HTML tags
  
### Elements

- HTML element encompasses opening tag, closing tag, content (optional for content-less tags) Eg:
- `<p>This is the content</p>` : This complete thing is called a HTML element.

### Attributes

- An attribute defines a property for an element, consists of an attribute/value pair, and appears within the element’s start tag. An element’s start tag may contain any number of space separated attribute/value pairs.

- The most popular misuse of the term “tag” is referring to alt attributes as “alt tags”. There is no such thing in HTML. Alt is an attribute, not a tag.

  `<img src="foobar.gif" alt="A foobar.">`

### Case Insensitivity

- In HTML, tag and attribute names are not case-sensitive. It means the tag `<P>`, and the tag `<p>` defines the same thing in HTML which is a paragraph.
- But in XHTML they are case-sensitive and the tag `<P> is different from the tag <p>.`

### Container tags

- The container tag always wraps around text or graphics and comes in a set with an opening and a closing.

    `<html> opening tag`

    `</html> closing tag`

### Empty tag

- The tag `<br>` is one that adds a line break. Empty tags do not have to be wrapped around text and do not require a closing.

### Block-level Elements

- A block-level element always starts on a new line and takes up the full width available (stretches out to the left and right as far as it can).

    | Html                                         | Web              |
    | -------------------------------------------- | ---------------- |
    | `<div> Hello </div>`<br>`<div> World </div>` | Hello <br> World |

### Inline Elements

- An inline element does not start on a new line and only takes up as much width as necessary.

    | Html                                             | Web         |
    | ------------------------------------------------ | ----------- |
    | `<span> Hello </span>`<br>`<span> World </span>` | Hello World |

### HTML Headings

- HTML uses six levels of heading tags `<h1> to <h6>`. h1 being the highest (or most important) level and h6 the least.
 Example :  `<h1>Heading 1</h1>`

### HTML Paragraphs

- used to publish text on the web pages. are defined with the `<p>` tag.

  `<p>This is a paragraph.</p>`

### HTML Line Breaks

- The `<br>` element is used to insert a line break without starting a new paragraph.

  `<p>This is a paragraph <br> with line break.</p>`

### HTML Comments
- An HTML comment begins with `<!--` and ends with `-->`
    
    ` <!-- This is an HTML comment --> `

### HTML Spaces

- Insert `&nbsp;` for creating extra spaces.
    
    `<p> Multiple&nbsp;&nbsp;&nbsp;spaces.</p>`

### HTML Links (Hyperlinks or Web links)

- Links are specified in HTML using the `<a>` tag.

    `<a href="url">Text link</a>`

### Images
- The `<img>` tag is used to insert images in HTML documents.

    `<img src="url" >`
- Setting Width and Height of an Image

    `<img src="sampleImage.jpg" width="300" height="300">`

### Tables

- A table is defined using the `<table>` tag, and 
- contains a number of table cells ( `<td>`, for “table data” ) 
- which are organized into table rows ( `<tr>`). 
- The markup (HTML code) for a table is always based on rows, never columns.
-  Browsers built-in style sheets will display the text in the `<th>` element as bold and centered. 

``` Html
<table>
    <thead>
        <tr>
            <th>Season</th>
            <th>Goals</th>
            <th>Assists</th>
        </tr>
    </thead>
    <tfoot>
        <tr>
            <th>Sum</th>
            <td>65</td>
            <td>63</td>
        </tr>
    </tfoot>
    <tbody>
        <tr>
            <th>2009-2010</th>
            <td>25</td>
            <td>43</td>
        </tr>
        <tr>
            <th>2011-2012</th>
            <td>40</td>
            <td>20</td>
        </tr>
    </tbody>
</table>
```

<table>
    <thead>
        <tr>
            <th>Season</th>
            <th>Goals</th>
            <th>Assists</th>
        </tr>
    </thead>
    <tfoot>
        <tr>
            <th>Sum</th>
            <td>65</td>
            <td>63</td>
        </tr>
    </tfoot>
    <tbody>
        <tr>
            <th>2009-2010</th>
            <td>25</td>
            <td>43</td>
        </tr>
        <tr>
            <th>2011-2012</th>
            <td>40</td>
            <td>20</td>
        </tr>
    </tbody>
</table>

### Lists

- HTML lists are used to present list of information in well formed and semantic way.

    - **Unordered Lists** : Set of related items, in no particular order.
        ``` Unordered lists
        <ul>
            <li>Chocolate Cake</li>
            <li>Black Forest Cake</li>
            <li>Pineapple Cake</li>
        </ul>
        ```
        <ul>
            <li>Chocolate Cake</li>
            <li>Black Forest Cake</li>
            <li>Pineapple Cake</li>
        </ul>

    - **Ordered list** — Set of related items, in a specific order.
        ``` Ordered list
        <ol>
            <li>Mix ingredients</li>
            <li>Bake in oven for an hour</li>
            <li>Allow to stand for ten minutes</li>
        </ol>
        ```
         <ol>
            <li>Mix ingredients</li>
            <li>Bake in oven for an hour</li>
            <li>Allow to stand for ten minutes</li>
        </ol>

    - **Description list** — Used to display a list of terms and their descriptions.  
      - DT tag stands for Definition Term
      - DD tag means Definition Description
        ``` Description list
        <dl>
            <dt>Bread</dt>
            <dd>A baked food made of flour.</dd>
            <dt>Coffee</dt>
            <dd>A drink made from roasted coffee beans.</dd>
        </dl>
        ```
         <dl>
            <dt>Bread</dt>
            <dd>A baked food made of flour.</dd>
            <dt>Coffee</dt>
            <dd>A drink made from roasted coffee beans.</dd>
        </dl>

### Forms 
- HTML Forms are required to collect different kinds of user inputs, such as contact details like name, email address, phone numbers, or details like credit card information, etc.

    - **Input Element**: Depending on the type attribute, an input element can be of type text field, checkbox, password field, radio button, submit button, reset button, etc.
    
        - Text Fields - `Name:  <input type="text" name="username" id="username">`
        - Password Field - `Password:  <input type="password" name="user-password" id="user-pwd">`
        - Radio Buttons - ` <input type="radio" name="sex" id="male"> Male`
        - Checkboxes - `<input type="checkbox" name="sports" id="soccer"> Soccer`
        - File Select box - `Upload: <input type="file" name="upload" id="file-select">`
        - Textarea - `Address: <textarea rows="3" cols="30" name="address" id="address"></textarea>`
        - Select Boxes - Dropdown list of option
            ``` box
                <select name="city" id="city">
                    <option value="sydney">Sydney</option>
                    <option value="melbourne">Melbourne</option>
                    <option value="cromwell">Cromwell</option>
                </select>
            ```
        - Submit Button - `<input type="submit" value="Submit">`

``` Notes

Markup Language
Xhtml vs html
html vs html5
List block level elements
List Inline elemnts

```
