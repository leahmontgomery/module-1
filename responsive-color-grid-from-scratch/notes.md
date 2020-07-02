The order of the Box Model from inside out

1. Content (the element's context such as text)
2. Padding (the spacing between the content and the element's border)
3. Border (the element's border)
4. Margin (the spacing between the elements border and other neighboring elements)


Responsive Design
    - Designing a webpage so that a user may access your site on any sized device, mainly mobile, tablet and desktop, and your website will respond appropriately.
    
    - Common method for approach is Mobile First, meaning to do your mobile design first and then use media queries to style the tablet and desktop views.


*{        /*Resets and Default styling*/
    margin: 0;
    padding: 0;
}

/*Mobile Design*/
#box {
    border: 2px solid black;
}

#box > h1 {
    background-color: dodgerblue;
}

/*Larger phones*/
@media (min-width: 400px) {
    #box {
        border: 2px dashed green;
    }

    #box > h1 {
        background-color: firebrick;
    }
}

//*    only= old browser, ignore code(can't support)   screen= what is this query for? screen/print/etc
@media only screen and (min-width: 400px)

/*Tablet*/
@media only screen and (min-width: 650px){
    
    #box {
        border: 5px dashed purple;
    }

    #box > h1 {
        background-color: cornflowerblue;
    }
        
}


@media only screen and (min-width: 650px) and (max-width: 700px){
    body {
        background-color: yellow;
    }
}