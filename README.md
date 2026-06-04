Commit title and explanations

commit-1    Completed Coding challenge-1 and challenge-2

challenge-1 
This just about headings,paragraphs,tags,links,lists and no extra css ,semantically dividing sections into header ,nav ,footer 

challenge-2
It is simple Product card which contains basic html code and no css

................................................


commit -2  Concepts of class and ids

This is all about tag name, class and id selectors
priority level- as below

1.!important
2.id 
3.class
4.element 
5.universal selector 
even pseudo-classes has high priority than normal a styling 
.................................................

commit- 3 Absolute Positioning ,Adding Margin ,padding, width of container,centering page using margin but only horizontally not vertically

Pseudoclasses
1. State-based pseudo-classes-   These depend on the state or interaction of an element.
   
:hover
:focus
:active
:visited
:link

2. Structural pseudo-classes-     can be applied to  element, class, ID, and universal selectors.
   
:first-child
:last-child
:nth-child()

This both 1. State-based pseudo-classes and 2. Structural pseudo-classes can be applied to all elements such as link ,button,p etc

In the above first five are the pseudoclasses for link and below are for elements 
-page reset by , margin: 0; padding: 0;
-if we use any particular notation(eg: rgba ,hexa) in project try to use same in notation over entire project
-while centering div we shld always define particular width ,align-items ,justify-content to center .
-without flexbox we can center a div only horizontally by margin:auto,for vertical we shld use flex
-for applying margin and padding for inline elements ,-only horizontal padding and margins will be applying  ⚠️Top and bottom padding are visible, but don't affect layout normally,❌ Top and bottom margins generally don't work as expected,to make this vertical padding and margins work we have to convert it to block or inline-block elements

Types of Boxes
1.inline- takes only necessary space,dont create line-breaks,only horizontal padding and margins will work
2.block - takes entire line ,create line break ,both vertical and horizontal margins and padding can be applied 
3.inline-block - takes space like inline element without creating line-break but all properties such as margins and padding can be applied like block elements ,inline from outside block from inside 

Absolute psoitioning-  relative for parent which will be in normal document flow,absolute for child which needs to be make out of the flow ,once its out of flow it wont affect normal flow ,wtevr v define in normal flow will go below it and this absolute positioned element will  appears above oit
..................................................
commit-4 Pseudo-elements

Pseudo-elements- A pseudo-element is a CSS feature that lets you style a specific part of an element or create a virtual element that doesn't exist in the HTML.
1.to  Add decorative content such as badges,labels,icons,ribbons
 ::before and ::after

2.Style part of text
p::first-letter ,p::first-line 

3. Decorative shapes
   .card::after {
  content: "";
  width: 100%;
  height: 3px;
  background: red;
}

4. Overlays and effects
.card {
  position: relative;
}

.card::before {
  content: "";
  position: absolute;
  inset: 0;
  background: rgba(0,0,0,.5);
}

.........................................................
Commit -5 floats 

By default browser will be content box ,for good building we should use box-sizing:border-box;
In border box , width will not seperately add border ,padding ,width ,its just width include all
three ways of building layout float ,flexbox ,grid
Float is neither 1D nor 2D.


using float:right ,left and clearing floats 
when float is applied the text will be flowed outside the normal flow like absolute positioning ,remaining elements will just wrap around
after applying float ,inline or anything will be converted as block level 
The clear:both property is intended for block-level elements

...........................................................
commit-6 

FLEXBOX

Default values 
Flex Container Properties...

| Property          | Default Value |
| ----------------- | ------------- |
| `flex-direction`  | `row`         |
| `flex-wrap`       | `nowrap`      |
| `justify-content` | `flex-start`  |
| `align-items`     | `stretch`     |
| `align-content`   | `stretch`     |

Flex Item Properties


Property 	Default
order     	0
flex-grow	0
flex-shrink	1
flex-basis	auto
align-self	auto

order - -1 to make left first one ,if we wanna put another left to it then -2 ,right last one shld be 1 ,if we wanna put one extra element next to it is 2 
margin was not good enough to make space betwn flex-items so thy invented gap

defaults of flex property
flex-grow:0;
flex-shrink:1;
flex-basis:auto;

if we give- flex-basis: 200px in flex-container, it is just a recommendatio width ,its not exact width ,if there is enough space then it will be 200 ,if not it will be below 200 ,coz by automatically flex container shrink coz by default shrink will be 1 ,if we make it to 0 then it will be 200px and items overflow flex container 
flex-grow:1 , will equally divide the flex-items in flex container ,if we make it 0 then it will take only necessary space

.........................................................
