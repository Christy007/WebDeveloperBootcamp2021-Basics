# WebDeveloperBootcamp2021 -- In progress!!!!

# HTML Boilerplate
- It is the structure of the html file.
- It starts with a flag **< !DOCTYPE html >** which specifies the html version and type of document that we are building.
- Then we have **< html >** tag which basically represents the elements in the entire web page.
- < html > tag has **< head >** and **< body >** tags within html, **head** represents the metadata( contents that's not visible for the user) and **body** represents all the the contents that are visible to the user.
- **< title >** tag represents the title for the document tab.
- **!+tab** shortcut can be used to generate a sample boilerplate in Visual Studio Code.

Sample of proper HTML structure is written in the file **"ProperHTMLStrucute.html"**<br>
- Few main things that we have to take care while building a html page
  - Try to **build semantic webpages**, avoid using non-semantic wrappers like < div > and < span >  unless it's necessary
  - Building a semantic webpage makes your script more meaningfull and readable
  - In body tag, start with **< header >** tag which contains the header of the webpage
  - Then, if there is a navigation tab, define a **< nav >** tag after header tag
  - Define the **< main >** tag next, which will contain the main contents of the web page
    - **< article >** : encloses a block of related content that makes sense on its own without the rest of the page. Examples include: a forum post, a magazine or newspaper article, or a blog entry, a product card, a user-submitted comment, an interactive widget or gadget, or any other independent item of content.
    - **< section >** : grouping together a single part of the page that constitutes one single piece of functionality (e.g., a mini map, or a set of article headlines and summaries), or a theme. It's considered best practice to begin each section with a heading. Section can also be a group of buttons
    - **< aside >** : contains content that is not directly related to the main content but can provide additional information indirectly related to it (glossary entries, author biography, related links, etc.).
    - **< time >** : represents a specific period in time. **datetime** attribute translates date into machine readable format<br>
     Example: next interview preparation class is on <strong>< time datetime="2021-06-08">8th June< /time></strong> which starts at <strong>< time datetime="18:00">18:00<            /time></strong>. With the help of this element we can make our code more semantic.
    - **< figure >** : This is again a html element that we can use to make our code more semantic. Using this element we can **containerize image and its caption** together
  - At the end we can define **< footer >** which represents a group of end content for a page.

# < HTML >
  
  ## HTML Elements
  * **< p >** element **represents** a paragraph. Paragraphs are usually represented in visual media as **blocks of text** separated from adjacent blocks by blank lines and/or first-line indentation, but HTML paragraphs can be any structural grouping of related content, such as images or form fields.
  * The **< h1 > to < h6 >** HTML elements represent six levels of section headings. **We should never select different heading elements, just to adjust the size**. We should atmost have only one < h1 > in our file. We should not have an < h3 > without h2 and h1, simillarly for other header elements as well.
  * **< ol >** is ordered list which lists the elements with numbers <br>
    **< ul >** is unordered list which lists the elements with bullets <br>
    Permitted contents in both < ol > and < ul > are **< li >, < script > and < template >** <br>
    Its not good design to add other components in ol and ul
  * **< a >** Anchor tags are defined with the href attribute. Attribues are special words inside a open tag which controls the elements behaviour.<br>
    **href** attribute specifies the link to which the anchor tag has to be redirected.
    href can redirect user to another website or to webpages within the same website.
  * **< img >** is used to add image to our webpage.<br>
    Main attributes for img element are **src** to sepecify the location of the image. It can be local pictures or any online links<br>
    Next attribute is **alt** which describes the image making it more accessible to all users using screen readers
  * **< div >** : Content Division Element: basically a container to group elements together. It's a block level element(which takes up the whole line)
  * **< span >** It's also a container, usually used to group elements ot texts in the same line.
  * **< hr>** represents a thematic break between paragraph elements as implemented before and after the nav section at the begining of this webpage<br>
  * **< br>** is used as a line break in paragraph
  * **< sup>** Superscripts are usually rendered with a raised baseline using smaller text.<br>
    Example: x<sup><a href="https://github.com/Christy007/WebDeveloperBootcamp2021/edit/master/README.md">2</a></sup> + y<sup>**2**</sup>
  * **< sub>** Subscripts are typically rendered with a lowered baseline using smaller text
    Example: C<sub>**8**</sub>H<sub>**10**</sub>N<sub>**4**</sub>O<sub>**2**</sub>
  * **Entity codes** with entity code we can display symbols or specials characters in our html to build a strucuted html code
    * Usually starts with ampersand and ends with a semicolon, example: "&**amp**;"
    * Browser will intrpret this code and will render the correct code
  * **< table >** It is structured set of data built using rows and columns <br>
    * **< caption>** displays the caption for the table <br>
    * **< td>** represents a cell of the table that contains data <br>
    * **< tr>** represents row of cells in a table <br>
    * **< th>** represents a cell as header. Text entered in in this cell are default Bold<br>
    * **< thead>** defines set of rows defining the head of the columns <br>
    * **< tbody>** defines set of rows that below to the body of the table <br>
    * **< tfoot>** defines a set of rows summarizing the columns of the table <br>
    * <strong>colspan</strong> this attribute indicates how many columns the cell extends <br>
    * <strong>rowspan</strong> this attribute indicates how many rows the cell extends
  * **< form >** represents a document section containing interactive controls for submitting information <br>
    * main attributes of form are: <br>
      1. <strong>action</strong> : which specifies where the form data should be sent. <br>
      2. <strong>method</strong> : specifies which HTTP method to be used.
    * <strong>< input></strong> element is used to create different form controls <br>
      * <strong>type</strong> attribute alters the input's behaviour and appearance <br>
        * <strong>search</strong> attribute value for type element represents a single-line text field for entering search strings. May include a delete icon in supporting                 browsers that can be used to clear the field <br>
        * <strong>checkbox</strong> attribute value for type element allows single values to be selected/deselected. <br>
        * <strong>radio</strong> attribute value for type element allows a single value to be selected out of multiple choices with the same name value. <br>
        * <strong>range</strong> attribute value for the type element displays as a range widget. <br>
        * **password** type encrypts the value entered by the user
        * **color** type displays a color widget where user can select a color
      * <strong>name</strong> attribute helps to link the data in the input fields with the query parameters of the server, when a form is submitted <br>
      * <strong>placeholder</strong> attribute gives the input field a default text. <br>
    * <strong>< label ></strong> element is used to link the input/form control to a text/label.
      * Value of <strong>for</strong> attribute in label tag should match with the value of <strong>id</strong> attribute in respective input tag <br>
    * <strong>< button ></strong> element declared inside a form is by default of submit type. To chnage the functionality of the button inside a form we use the attribute                 <strong>type</strong>. type="button" makes a button inside a form behave just like a normal button. <br>    
    * <strong>< select ></strong> element creates a dropdown and the values in the dropdown is defined by **< option >** tag
    * <strong>< textarea ></strong> element represents a multi-line plain-text editing control, useful when you want to allow users to enter a sizeable amount of free-form text, for example a comment on a review or feedback

# CSS
  
  * CSS stands for Cascading Style Sheet
  * CSS describes how document are presented visually
  * Basic pattern for CSS is
    * selector{ <br>
      property: value;<br>
      }
  * There are 3 possible ways to add style to your html page
    1. You can specifify the stle in htnl tag <br>
       < h1 **style="background-color: red"** >
    2. With the help of **< style >** tag we can define the style properties in < head > tag <br>
        **< style >** <br>
        selector{ <br>
        property: value; <br>
        } <br>
        **< / style >**
   * Above listed 2 ways of styling a html element is **NOT RECOMMENDED**
   * Best way to add style is to create a .css file and link it to html tag using **< link >** tag
     * **rel** attribute specifies the relation of the linked file to the document
     * **href** specifies the location of the file
 
## CSS properties
  *Sample file:* ***common.css***
  * **color** property sets the foreground color of the element's **text**
  * **background-color** sets the background color of an element
  * **text-align** sets the horizontal alignment of the content inside a block element
  * **font-weight** sets the boldness of the element
  * **text-decoration** sets the appearance of decorative lines on text
  * **line-height** sets the height of the line(to maintain a proper gap between lines)
  * **letter-spacing** sets the horizontal spacing behavior between text characters
  * **font-size** basically sets the size of the text, it increases both height and width of the text
  * **font-family** specifies which font to be used. We can also build a font stack, if user's system doesn't support the intial font, then it can pick-up any font listed in the stack.
  * **text-transform** specifies how to capitalize an element's text
  
  <hr>
  
 ###### References:
  * https://developer.mozilla.org/
  - https://docs.github.com/en/github/writing-on-github
