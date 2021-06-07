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
  
 ###### References:
  * https://developer.mozilla.org/
  - https://docs.github.com/en/github/writing-on-github
