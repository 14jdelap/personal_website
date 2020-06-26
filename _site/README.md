# Welcome!
You're in my personal website. I coded the site as a way to improve my design and coding skills. 

## Main learnings

1. People skim, not read
    - Optimize for that with appropriate formatting and layout
    - Tight column widths 
    - Generous font size
    - Short paragraphs with compelling content first
    - Use headers and formatting to make a clear visual heirarchy
2. People have a poor sense of orientation online
    - Clearly convey what's a link
    - Special formatting for links that have been visited (so users know where they've previously navigated)
    - Prominent navigation system and site logo
    - Make it clear where users currently are 
    - Give several options to teach the same destination, when possible
    - `a` (anchor) tags should open in a new window to minimize the chance users struggle to get back to the page
3. Optimize for mobile
    - Fluid typography: its font size continuously changes based on viewport size
    - Images resize based on viewport width
    - Responsive design
        - The most significant change is a **mobile navigation system** based on Luke W's design (still in use in his personal website) 
        - There's one breakpoint where the design changes using a media query to optimize for tablet/mobile sizes
        - Also use a class to hide and show elements using the media queries
4. Use modern layout tools
    - `grid` and `flexbox` work wonders
5. Need for speed: how did I get a 95 in lighthouse?
    - WebP (a next-gen image format with better compression) using the `<picture>` tag and an `<img>` fallback file with PNG versions (in case the user's browser doesn't support WebP)
    - Minimize HTTP requests: 1 stylesheet linked in the `head`, no scripts barring the Substack `iframe`
    - Optimize images
        - Compress all images with the `loading` attribute of the `img` tag
        - Lazy load those under the initial loading screen
    - Minimize HTML/CSS to reduce file size
6. Insert metadata in the `head` and meet accessibility requirements in Lighthouse
    - Lighthouse is reasonably comprehensive — just follow its suggestions 
7. Use a typography that contributes to your objective
    - This is **arguably the most important visual design decision I made**
    - I wanted to use a friendly but firm and professional sans serif
    - Chose to use Myriad Pro, with Helvetica and Sans as backups 