# Foundations of Web Development
01. In your own words, why do we use Git?
    > There's a few reasons that Git is used, the first is it's popularity in the field. It's *very* common and unless you live under a rock it's something that's expected to be known. The second reason is: accidents happen, having many versions/backups of your code uploaded is extremely helpful.

02. In the terminal, what is the command `mkdir` used for?
    > mkdir is used to create a directory.

03. What is a ***pseudo-class*** and what are some of the most common ones you think you will use?
    > I'm assuming this is referring to pseudo-elements/pseudo-selectors, in that case the most used are easily :active and :hover. They are both (usually) used to add animations to element interactions.

04. What is ***specificity*** and how might you use it to your benefit?
    > Specificity is CSS's way of calculating which style to use in cases of conflicting styles. Full transparency, I'm not sure how this could be used to your benefit but it's definitely helpful to understand where and how styles should be applied especially when using other tools like Bootstrap that make specificity more complex.

05. What problems do you think you could run into if you over-utilized the `!important` feature?
    > Since '!important' throws specificity out the window, once it's applied to an element the only way to change the style is to use another '!important'. This makes it really difficult to layer rules.

06. What are the three components that makeup a `CSS` rule? <br> Example:

    ```css
        h1 {
            color: rgba(255, 210, 33, .75);
        }
    ```

    > The three parts of css rules are selectors (the element being selected/targeted, in this example it's h1), properties (the style being changed, in this example it's color) and values (how the style/property is being changed in this case it's the RGBA value that changes the color).

07. How do you think good design influences people when visiting a website, and what sorts of things could you convey through design alone?
    > A lot of people commonly say that first impressions are everything. If your first impression of a cutting-edge tech corporation was a dated, unevolved and bland website: what faith would you have in them? If you were an investor, would you be interested in investing?

08. What is the purpose of ***wireframing***?
    > There are many purposes of wireframing, the first being for the developer, it's a planned and approved guide to roughly what needs to be done. The second purpose is the approval part, if you're working with a client and you spend all of your time working revisions instead of having a clear cut plan/vision/guide from the beginning.. It's not very efficient.

09. Do you think wireframes are worth the time, energy, and effort that they require? Why or Why not?
    > I think that depends on a few variables: complexitiy, expectations (are you working with a client) and time. Even if those variables say no, I still think it's good practice (and great for experience) to use wireframing.

10. Define the display `:flex property:`
    > Flexboxes are the holy grail of CSS. They allow for easily configurable structuring and alignment. They have a very wide range of options that make them versatile.

11. What `CSS` properties affect the size of a box model?
    > Margin and padding but you also have to consider the space of the content itself.
