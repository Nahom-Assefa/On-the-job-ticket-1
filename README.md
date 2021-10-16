# Code Refactor Starter Code

**Version 1.0.0**

## The Purpose
The purpose of this project was to refactor existing code, and condense it where sensible in order to elicit seamless future adjustments and improve performance.

## Significant Changes
In the header alterations were made to make the h1 element clickable, and introduced a nav bar floated to enable all elements in header to be on the same plane.
In the section with the id of "contents" is where most of the html adjustments preside. I was able to condense multiple classes into larger more applicable classes.
The id contents was the parent element to its child elements that I was able to use the position of styling of relative and absolute to manipulate accordingly.
Within CSS we took advantage of the classes we cleaned up in html to delete repetitive class selectors in line with the dry principle. Also adjusted multiple individual styling
that was either unnecessary or applying in the child elements when they could be directed to the parent and vice versa. Lastly, again, within HTML got rid of the div and footer 
class as the footer tag already sufficed for our purposes.

### Challenges 
On this particular challenge I noticed I had some trouble getting the benefits class to play nice within its parent element. I had wrapped the benefits class with the content class 
and grouped them accordingly as children of id contents. The benefits class when floated right didn't tuck in the right corner how I hoped. It took some effort playing with different
versions of the positioning style until I realized the parent needed a relative positioning so the child benefits could be absolutely manipulated accordingly. Once I figured this the 
issue became the margin bottom of 20px applying to each inividual content section. To deal with this instead of adding a second class selector to the third content box I used the 
styling property nth-of-type to loop over until it reached the third child to set the margin bottom to 0px. This allowed the benefits class to be in line with the third content box instead of being longer by 20px due to the margin bottom issue.

#### License and Copyright 
© Xander Rapstine, Trilogy Education Services/2U
