# EJS PARTIALS

### 

> Partials come in handy when you want to reuse the same HTML across multiple views. Think of partials as functions, they make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file andinclude it wherever you need it.

- Including a partial in EJS is quite straightforward. You use <%- include( PARTIAL_FILE ) %> where the partial file is relative to the template you use it in.
* Note: The <%- %> tags allow us to output the unescaped content onto the page (notice the -). This is important when using the include() statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’
- In EJS, any JavaScript or non-HTML syntax you include in your templates is always surrounded by <% %> delimiters
-
- Delimiters could be changed if it was necessary.
- used to avoid repetition of the same code on several pages
-  Need Node.js installed before you can use EJS
- Make sure EJS and express are both installed before
- home.ejs file has a link to the partial.ejs file which serves as the partial. (In this instance)
- server = app.js
- `<%- include('partials/partial') %>`
- views folder which is the default template engine location for express
- Express is a reserved folder name where express checks for template engine by default
- Can save time by reusing code
- Functional programming can make our lives easier
- Partial application starts with a function.
- Create new functions on the fly

Reference:  https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433

Reference: https://www.includehelp.com/node-js/ejs-partials.aspx