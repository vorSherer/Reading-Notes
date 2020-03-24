# Read 12 - Components

#### 2020-03-24

## RESOURCES:
#### EJS Partials <br>
https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433 <br>
#### Watch EJS tutorial from WalkThroughCode on YouTube, Video 7, Partials <br>
https://www.youtube.com/watch?v=3_xEEH4fTEk&t=0s&index=7&list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt <br>

### Using EJS Partials
__Partials__ are a native feature of EJS. *The typical use case* for partials is to hold any reuseable, static (i.e., non-changing) code, such as a common nav bar or footer. You define that reusable code in a file and include it wherever you need it. <br>
A typical path to the partial files would be __views/partials/__(files go here). A nav bar partial might be called __navbar.ejs__, a footer __footer.ejs__, and so on. <br>
Syntax for a partial can be as simple as <br>
__<%- include('relativePath/fileName') %>__ <br>
The __<%- %>__ tags allow us to output the unescaped content onto the page (notice the __-__). This is important when using the __*include()*__ statement since you don’t want EJS to escape your HTML characters.
Simply add this include statement where ever you want the code to appear. <br>
This also simplifies maintaining your code, as any changes get made once in the source file, rather than on every page where it appears!
