# WebDeveloperBootcamp2021 -- In progress!!!!

# HTML Boilerplate
- It is the structure of the html file.
- It starts with a flag **< !DOCTYPE html >** which specifies the html version and type of document that we are building.
- Then we have **< html >** tag which basically represents the elements in the entire web page.
- < html > tag has **< head >** and **< body >** tags within html, **head** represents the metadata( contents that's not visible for the user) and **body** represents all the the contents that are visible to the user.
- **< title >** tag represents the title for the document tab.
- **!+tab** shortcut can be used to generate a sample boilerplate in Visual Studio Code.

Sample of proper HTML structure is written in the file **"ProperHTMLStrucute.html"**<br>
- Few main things that we have to take care while building a html page.
  - Try to **build semantic webpages**, avoid using non-semantic wrappers like < div > and < span >  unless it's necessary
  - Building a semantic webpage makes your script more meaningfull and readable
  - In body tag, start with **< header >** tag which contains the header of the webpage.
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
        1. <strong>search</strong> attribute value for type element represents a single-line text field for entering search strings. May include a delete icon in supporting                 browsers that can be used to clear the field <br>
        2. <strong>checkbox</strong> attribute value for type element allows single values to be selected/deselected. <br>
        3. <strong>radio</strong> attribute value for type element allows a single value to be selected out of multiple choices with the same name value. <br>
        4. <strong>range</strong> attribute value for the type element displays as a range widget. <br>
        5. **password** type encrypts the value entered by the user
        6. **color** type displays a color widget where user can select a color
      * <strong>name</strong> attribute helps to link the data in the input fields with the query parameters of the server, when a form is submitted <br>
      * <strong>placeholder</strong> attribute gives the input field a default text. <br>
      * <strong>value</strong> attribute is used to specify the initial value, and from then on it can be altered
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
     * **href** specifies the location of the file.
 
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
         
  ### More Css selectors
  *Sample file:* ***css2.css***
  * **&#42;** this represents a universal selector, changes to the proerties made using this selector will apply to all element
 * **h1,h2** represents a selector list, css style will be applied to all the elements listed
  * **descendant selector**, selector **li a** represent that css style will be applied to all  anchor tags nested inside li tag
  * **adjacent selector**, selector **h3 + p** represent that the css style will be applied to all paragraph tags that is immediately preceeding(can be sibling) after h3
  * **direct child**, selector **form > h4** selects all h4 which is direct-child/direct-descendant of form
  * **attribute selector**, ex: h4[class*="eForm"] selects all h4 where class contains the text "eForm"
  * **pseudo classes** are the keywords added to a selector that specifies a special state of the element selected<br>
         :hover<br>
         :active<br>
         :checked<br>
         :nth-of-type(n)
  * **pseudo elements** are the keywords added to a selector that lets you style a particular part of the selected elemnets<br>
         ::first-letter<br>
         ::first-line<br>
         ::selection
         
  ### Specificity
  * Specificity is how the browser decides which rules to apply when multiple rules could apply to the same element
  * Specificity is calulated based on three main elements:
    * **ID selector** is extremely specific, it beats out the total number of class selectors (ID selectors)
    * **class selector** is pretty specific, it beats out the total number of element selectors (Class, Attribute and Pseudo-class selectors)
    * **element selector** is least specific (element, Pseudo-element selector)
  * **!important** keyword can override specificity, properties assigned !important will be applied compulsorly no matter what is the 
         
  ### Inheritance      
  * If the child elements doesnt have any property values set, then they can inherit the parent properties<br>
    **ex:** childElementSelector{<br>
    color: **inherit** ;<br>
    }<br>
  
  ### CSS Box Model
  *Sample file:* ***CSS Box Model/boxmodelStyles.css***
  * 4 main aspects of box model are
    * **Content box**
    * **Border**
    * **Padding**
    * **Margin**
  * **width** sets the width of the content area
  * **height** defines the height of the content area
  * **border** sets the element's border. We have three main border properties:
    * **border-width** : sets the width of the border element. px is the most commonly used unit as the border-width is constant all the time
    * **border-color** : sets the color of border element
    * **border-style** : sets the line style for all four sides of an element's border
  * **box-sizing** this property can be used if you dont want the element to takeup extra space to implement the border<br>
    ex: box-sizing: **border-box**
  * Also width, style and color for each sides of the border can be set separately using properties like **border-left-color**, **border-right-width**....
  * **border** can be used to set all three main properties at once, instead of writing different line of code for each property<br>
    ex: border **width** **style** **color**
  * **border-radius** this property is used to round the corners of the element's outer border edge. Commonly used unit is %
  * **padding** is the space/gap between the actual content box and the border
    * padding can be set individually for each side or we can use the shorthand<br> 
      ex: padding: 10px 20px;
  * **margin** is the space/gap between the two elements, basically the margin area on all four sides of an element
    * margin can also be set individually for each side or we can use the shorthand<br> 
      ex: margin: 10px 20px;
  * **body** element by default has margin set to a default value, to remove this margin we can use margin property and set it to 0
   
  ### Display property
  *Sample file:* ***Display/displayStyle.css***
  * **display** property sets whether an element is treated as a block or inline element. we have three main values for display
    * **inline** width and height are ignored. Margin and padding push elements away horizontally but not vertically
    * **block** block elements break the flow of a document. Width, Height, Margin and Padding are respected
    * **inline-block** behaves like an inline element but Width, Height, Margin and Padding are respected
         
  ### Units
  *Sample file:* ***CSS units/cssUnitStyles.css***       
  **Absolute**
    <li> **px** is the most commonly used **absolute** unit</li>
         
  **Relative**
    <li> **%** sometimes, it's a value from the parent and other times it's a value from the element itself</li>
    <ul> <li>**width: 50%** - half the width of the parent</li>
         <li>**line-height: 50%** - half the font-size of the element itself</li>
    </ul>
    <li> **em** there are **relative** units. With **font-size** property, 1em equals the font-size of the parent. 2 em's is twice the font-size of the parent. With **other** properties, 1 em is equal to the computed font-size of the element itself.</li>
    <li> Disadvantage of **em** is that, if we have same elements nested, there are chances that the child elements increase or decrease their size drastically as each child elements size depends on its immediate parent font-size.</li>
    <li> **rem** Root EMS are relative to the **root** html element's font-size. Often easier to work with.</li>
         
  ### Opacity and Alpha channel (rgba)
   *Sample file:* ***OpacityAndAlpha/oAa.css***
   * **Alpha channel** in rgb**a** and hex value #000000**ff** represents the color's transparency.
   * **opacity** css property is the degree to which content behind an element is hidden. Applies to the **whole element** including its content
  
  ### Position
   *Sample file:* ***Position\position.css***
   * position property determines how the element should be positioned in the document. The **top**, **right**, **bottom**, and **left** properties determine the final location of positioned elements
   * **static** Positioned according to the normal flow. The top, right, bottom, left, and z-index properties have no effect.
   * **relative** this element is positioned according to the normal flow of the document, and then offset relative to itself based on the values of top, right, bottom, and left.
   * **absolute** The element is removed from the normal document flow, and no space is created for the element in the page layout. It is positioned relative to its closest positioned ancestor, if any; otherwise, it is placed relative to the initial containing block.
   * **fixed** Fixed positioning is similar to absolute positioning, with the **exception** that the element's containing block is the initial containing block. This can be used to create a "floating" element that stays in the same position regardless of scrolling.
  
  <hr>
  
 ###### References:
  * https://developer.mozilla.org/
  - https://docs.github.com/en/github/writing-on-github
