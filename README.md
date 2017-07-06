# FLAS ( Under Development)
## Functional Layout And Style ( FLAS) Alternative  dynamic layout  to Html and CSS

### Proposed dynamic language for HTML and Styles.



The  web design languages such as Html and CSS are great and staying for long time in the internet web development.
However,there are lot of limitations for designing dynamic web applications  using these languages since these are originally designed for the static web site.
Lot of templates and languages (e,g: - Angualr, flex, vue etc) are proposed   to overcome the limitation of html and CSS. However, those framework and languages are just mixed with HTML and CSS  but not replacing the HTML and CSS.

We are trying to  propose new language for dynamic web site design without using HTML.

The following criteria  has  been considered for  the developing new proposed language:


Should have dynamic layout
Should  have dynamic style
Easy to define component.
Should be able to manipulate layout easily
Should  contains    data or variables.
Should have api to get and post data to server
Should be about to define functions and events 

Based on  above requirement, we started to develop new layout language FLAS ( Functional Layout and Style) for alternative to HTML and CSS.

### Sample  FLAS (Working condition - Subject to change)

~~~~ 

//// inline comment


//*
 comment block
*//

//import the another page layout or javascript file
@import "anotherpage.cs"

//define variable
var x;

//define variable with initial value
var y = 0;

// assign string to variable y
y = "hello ";

//layout for heading
h1(background-color:"red", width:"100%"){"this is heading"}


// table with rows and cols in array. Array start with [ and end with ]
table(style:"classname"){
   [tr(style:"trheading"{
       [td{"heading 1"},
       td{"heading 2"}];
   },

 tr{
       [td(background-color:"green"){"data 1"},
       td{"data 2"}];
   }];

}

// id is the object. this layout element can be easily manipulate using  id. 
div(id:"divid"){"this is div"}

// change the content of div  using id 
divid.content("this is new content);

//  onclick event for div element
div(id:"divid2"){"this is function div";
onclick = function (target){....}
}

// or attach the event  function to object
divid2.onclick = function (target){....}

~~~~ 


