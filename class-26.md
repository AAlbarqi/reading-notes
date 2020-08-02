# EJS PARTIALS

Partials come in handy when you want to reuse the same HTML across multiple views. 

- To make the same navigation bar and footer appear in the home and the other pages:

1. Under the `views/partials/` directory create a file callednavbar.ejs which will contain only the HTML for the navigation bar at the top of the home and post pages, and a file called footer.ejs in that same directory.

Example of how the main directory should look like:

![](https://ncoughlin.com/static/32a39dff02fb0f9d41dfa990a2d950b5/859af/3.png)


**Note** : In EJS, any JavaScript or non-HTML syntax you include in your templates is always surrounded by <% %> delimiters (you could change these delimiters if you really wanted to).

2. You use <%- include( PARTIAL_FILE ) %> where the partial file is relative to the template you use it in.

**Note** : Note: The <%- %> tags allow us to output the unescaped content onto the page (notice the -). This is important when using the include() statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’, etc…

3. Let’s create the homepage template in views/home.ejs and include the navbar and footer partial we just created:
    `<body>
        <div class="container">
            <%- include('partials/navbar') %>
            <div class="jumbotron"></div>
            <div class="row"></div>
            <%- include('partials/footer') %>
        </div>
    </body>`

