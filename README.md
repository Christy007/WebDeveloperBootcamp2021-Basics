# WebDeveloperBootcamp2021

# HTML Boilerplate
- It is the structure of the html file.
- It starts with a flag **< !DOCTYPE html >** which specifies the html version and type of document that we are building.
- Then we have **< html >** tag which basically represents the elements in the entire web page.
- < html > tag has **< head >** and **< body >** tags within html, **head** represents the metadata( contents that's not visible for the user) and **body** represents all the the contents that are visible to the user.
- **< title >** tag represents the title for the document tab.
- **!+tab** shortcut can be used to generate a sample boilerplate in Visual Studio Code.

Sample of proper HTML structure is written in the file "ProperHTMLStrucute.html"<br>
- Few main things that we have to take care while building a html page
  - Try to build semantic webpages, avoid using non-semantic wrappers like < div > and < span >  unless it's necessary
  - In body tag, start with **< header >** tag which contains the header of the webpage
  - Then, if there is a navigation tab, define a **< nav >** tag after header tag
  - Define the **< main >** tag next, which will contain the main contents of the web page
    - **< article >** : encloses a block of related content that makes sense on its own without the rest of the page. Examples include: a forum post, a magazine or newspaper article, or a blog entry, a product card, a user-submitted comment, an interactive widget or gadget, or any other independent item of content.
    - **< section >** : grouping together a single part of the page that constitutes one single piece of functionality (e.g., a mini map, or a set of article headlines and summaries), or a theme. It's considered best practice to begin each section with a heading. Section can also be a group of buttons
    - **< aside >** : contains content that is not directly related to the main content but can provide additional information indirectly related to it (glossary entries, author biography, related links, etc.).
  - At the end we can define **< footer >** which represents a group of end content for a page.

# < HTML >
  
  ## HTML Elements
  * **< p >** element **represents** a paragraph. Paragraphs are usually represented in visual media as **blocks of text** separated from adjacent blocks by blank lines and/or first-line indentation, but HTML paragraphs can be any structural grouping of related content, such as images or form fields.
  * The **< h1 > to < h6 >** HTML elements represent six levels of section headings. **We should never select different heading elements, just to adjust the size**. We should atmost have only one < h1 > in our file. We should not have an < h3 > without h2 and h1, simillarly for other header elements as well.
  * **< ol >**
  

  
 ###### References:
  * https://developer.mozilla.org/
  - https://docs.github.com/en/github/writing-on-github
