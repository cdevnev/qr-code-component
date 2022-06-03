This project is my first attempt at a Frontend Mentor challenge. My goal at the end of the project was to have a complete, working solution that matches the design spec as closely as possible and to solve any problems encountered during the challenge.

Problems I expected to encounter:
        - Figuring out how to make a responsive design

Problems I didn't expect:
        - Centering a single element, specifically the vertical centering
        - Default styling causing issues

The first problem I ran intp was figuring out how to round corners--this one was simple enough to solve with basic research. 

Another problem was centering. Horizontal centering was easy enough to resolve, with lots of options to achieve the result I was looking for. A problem I kept encountering was preventing the div from expanding in width as the page was scaled up -- primarily a responsive design problem but also a lack of practical understanding and application of the width attribute on elements. More on this in a moment.

With the basic styling working as expected and the padding/margins working mostly how I wanted them, I began tackling the responsiveness issues. The width of images was expected but I had to sort out how to fill the space within a container with the image. The width of the parent div was a recurring issue as I began tinkering with centering everything both horizontally and vertically by adjusting margin: 0 auto; and trying to keep the width in check. Lots of research led me to zeroing out the padding and margins across the page (normalization) which fixed a lot of issues and allowed the horizontal centering to work. 

Width was still scaling up with the page but I was able to eventually solve that as well after doing more research on responsiveness--which also led me to a realization. So many pages I'd viewed were wrapping everything in divs, and I thought I understood why but came to understand that vertical centering within the body of a page required a bit of div trickery. Giving the wrapper div a display: table; property and a nested div the table-cell allowed for easy centering using table styles. Finally, setting a max-width (of course!) prevented the div from expanding as the viewport changed, while the margins did their work to keep things centered. And while I had initially expected @media queries to be essential to keeping the design responsive, the percentages and em units allowed for things to scale well without it.

I obviously learned a lot during this challenge! Most valuable and unexpected was the page wrapping realization--although I'm sure there's more to unpack on that topic as I move forward. 


Thanks for reading and for any feedback you may happen to send my way!