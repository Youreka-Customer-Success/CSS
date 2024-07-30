# Youreka CSS Snippets 

A comprehensive collection of CSS Snippets that can be applied to your Youreka 
Form Templates.

## Features

CSS code snippets that provide a simple way to style and customize various aspects of your 
Youreka Forms.

Each snippets value can be adjusted as needed to, for instance, position, increase/decrease size, 
change color ect. Additionally, each CSS snippet will work in combination with 
other snippets to style your template and forms as needed.

## Snippets

| CSS Sections                                             | Description                                             |
| -------------------------------------------------------- | ------------------------------------------------------- |
| [Text Styling](#text-styling)  			   | Adjust font family, text size, text color              |
| [Button and Icon Adjustments](#button-and-icon-adjustments)| Adjust the format and size of Buttons and Icons              |
| [Form Design](#form-design)    			   | Update form design including layout and styling  |




## Text Styling




#### Font Family

```css
body, p, h1, h2, h3, h4, h5, h6, div, span, th, td {
font-family: cursive !important;
}
```    


#### Font Color

```css
body, p, h1, h2, h3, h4, h5, h6, div, span, th, td, a {
color: #ff9900 !important;
}
```    

## Font Size

      
### Set Base Font Size
All font sizes in the sections are set to be relative 
to this .slds class font-size. If you want to change everything 
proportionally, change just the font-size in the .slds class here.
If you want to change font-sizes relative other ones, change 
the indvidual styles in the Set Relative Font Size section below.

```css
.slds-scope *, .slds-scope :after, .slds-scope :before {
font-size: 24px !important;
}
```    

### Set Relative Font Size
NOTE: The "em" unit of measure is proportional to the parent size. 
For example, if .slds has a font-size of 14px, a another class 
that has a size of 2em will have a font-size of 28px on the page 
(e.g. 2 x 14).

#### Template Name Relative Font Size

```css
.slds #formContent h1.formName {
	font-size: 2.285em;
}
``` 

#### Form Name Relative Font Size

```css
.slds-text-heading_small.slds-m-vertical_small.form-number {
	font-size: 1.8em;
}
```

#### Attachment Upload Button Font Size

```css
span.slds-file-selector__button.slds-button.slds-button_neutral.OR-upload-button_nowrap {
	font-size: 2.43em;
        line-height: 2.43em;
        max-height: 2.43em
 }
```

#### Section Header Relative Font Size

```css
.title-text {
font-size: 2.28em;
}
```
#### Specific Section Header Relative Font Size
In order for this CSS to work, you need to replace the randomid with the randomid that corresponds to the section that you intend to adjust. disco__RandomId__c can be found on the Section record in Salesforce.
```css
[data-randomid="27d6b101"].form-section .title-form-section .title-text {
	font-size: 2.28em;
}
```

#### Checkbox/Radio Button Option Label Text Size

```css
.slds-form-element__label.slds-radio__label.slds-radio__label_target, .slds-form-element__label {
font-size: 1.5em !important;
}
```
<br/>


## Button and Icon Adjustments
<br/>
This CSS Snippet section will allow you to customize various button and icon sizes on Youreka Forms.

#### Header Buttons Size (Desktop Only)

```css
.slds-scope .buttons-fixed button {line-height: 3.5em;} 
```     
   

#### Next Page Arrow Icon Size 

```css
/* Next Page Arrow Icon */
.nextBtn .slds-button__icon {
width: 2.15em !important;height: 2.44em !important;
}
/* Previous Page Arrow Icon */
.prevBtn .slds-button__icon {
width: 2.15em !important;height: 2.44em !important;
}
```  

#### Button Border Radius & Color - Desktop


```css
.slds-scope .slds-button_inverse,
.slds-scope .slds-button_inverse:link,
.slds-scope .slds-button_inverse:visited,
.slds-scope .slds-button-group .slds-button_icon-inverse,
.slds-scope .slds-button-group .slds-button_icon-inverse:link,
.slds-scope .slds-button-group .slds-button_icon-inverse:visited {
 border-radius: 15px;
 background: #ff9900;
 color: #fff;
 border: 0;
}
.slds-scope .slds-button_inverse:hover,
.slds-scope .slds-button_inverse:focus {
 color: #fff;
 background: #ff6600;
 border: 0;
}
```  
#### Button Border Radius & Color - Mobile

```css
.slds-button.slds-button_neutral.js-mobile-save.slds-m-top_x-large {
border-radius: 15px;
background: #ff9900;
color: #fff;border: 0;
}
``` 
#### Button Icon Adjustments (Calender Icon, Geolocation Icon, Upload Files Icon)

```css
.slds-scope .slds-button__icon_left, .slds-button__icon_large, .input-calendar {
height: 1.5em !important;
width: 1.5em !important;
}
```  
#### Hamburger Menu Adjustments - Hide Save/Submit Buttons (Blue App)

```css
/*hide Submit*/
.side-menu-list ion-item:nth-child(1) {
    display: none;
}

/*hide save and close button*/
.side-menu-list ion-item:nth-child(2) {
    display: none;
}

/*hide quick save button*/
.side-menu-list ion-item:nth-child(3) {
    display: none;
}
```  

#### Hamburger Menu Adjustments - Hide Save/Submit Buttons (White App)

```css
/* hides: submit in menu*/
.complete-form-menu-list ion-menu-toggle:nth-of-type(1)  {
  display: none !important;
}

/* hides: save and close in menu*/
.complete-form-menu-list ion-menu-toggle:nth-of-type(2)  {
  display: none !important;
}

/* hides: quick save in menu*/
.complete-form-menu-list ion-menu-toggle:nth-of-type(3)  {
  display: none !important;
}
``` 




#### Attachment Upload Button Size (Desktop Only)

```css
.slds-scope .slds-file-selector_files .slds-file-selector__button {
    max-height: 2.625rem;
    line-height: 2.625rem;
}
```

#### Checkbox/Radio Button Size

```css
/* Adjust Radio Button Outer Size */
.slds-scope .slds-form-element__control .slds-radio .slds-radio_icon {
height: 60px !important;
width: 60px !important;
}
/* Adjust Radio Button Inner Icon Size */
.slds-scope .slds-icon_small {
width: 3.3rem !important;
height: 3.3rem !important;
margin: 0px !important;
}
/* Adjust Checkbox Size */
.slds-scope .slds-form-element__control .slds-checkbox .slds-checkbox_faux {
width: 3.3em;
height: 3.3em;
}
/* Adjust Checkmark Size */
.slds-scope .slds-checkbox [type="checkbox"]:checked + .slds-checkbox__label .slds-checkbox_faux::after {
height: 1rem !important;
width: .5rem !important;
transform: translate3d(-50%,-50%,0) rotate(45deg) scaleX(-1) !important;
}
```

#### Radio Button Color

```css

/* Adjust Radio Button Color */

#complete-form .slds-radio.radio-list input[type="radio"][checked="checked"]:disabled + .slds-radio__label svg {
fill: #05395a !important;
}
```

#### Date Input Selector Icon Size

```css
.slds-button__icon.input-calendar {
        padding-top: 0.3em;
}
```
<br/>

    
## Form Design
<br/>
This CSS Snippet section will allow you to customize the color of text, backgrounds, and borders of various elements on Youreka Forms.

#### Save Buttons Bar/ Header Color

```css
.slds-scope .buttons-fixed {
    background-color: #009ACD;
}
```

#### Reduce White Space Between Questions Vertically

```css
/******************* Less Whitespace Vertically *******************/
.form-section .control-group {
line-height: 6px; /* increase/decrease pixels to adjust vertical space between questions*/
}
```
#### Make entire form read-only

```css
/******************* Less Whitespace Vertically *******************/
/* hides: text, text area, multiselect picklist, single-select picklist
e-sig container, phone, date, date-time, number */
input:not([type="button"]),
select,
textarea,
.sig-answer-container,
.selectable-multiselect {
  background-color: #dbdada !important;
  pointer-events: none !important;
  user-select: none !important;
}


/* disables: camera */
.js-att-photo button.question-camera_toucharea  {
  background-color: #dbdada !important;
  pointer-events: none !important;
  user-select: none !important;
}

/* disables: submit in form*/
.save-button-container button.js-mobile-save  {
  background-color: #dbdada !important;
  pointer-events: none !important;
  user-select: none !important;
}

/* hides: submit in menu*/
.complete-form-menu-list ion-menu-toggle.md:nth-of-type(1)  {
  display: none !important;
}

/* hides: save and close in menu*/
.complete-form-menu-list ion-menu-toggle.md:nth-of-type(2)  {
  display: none !important;
}

/* hides: quick save in menu*/
.complete-form-menu-list ion-menu-toggle.md:nth-of-type(3)  {
  display: none !important;
}

/* hides: checkbox, radio buttons, geo-location (button) file upload */
.slds-checkbox,
.table-radio,
.js-geolocation,
.slds-file-selector__dropzone {
  pointer-events: none !important;
  user-select: none !important;
}

/* hides: add link section button, save & close, submit, nav-bar */
.add-linked-section,
#quickSaver,
#normalSaver,
.js-toggle-button {
  visibility: hidden !important;
}

/*positions cancel button to center of app header*/
#cancelBtn {
  position: relative;
  left: 105px;
  top: 2px;
}
/* Indicates Form is Read Only */
.form-number:after {
  content: " - Read Only" !important;
  font-size: 1rem !important;
  color: red !important;
  font-weight: bold !important;
}
```


#### Remove Gear Icon and Menu from View Form page (Dekstop Only)

```css
#mainForm #moreActionsBtn {
    display: none;
}
```


#### Prevent Users from Removing Linked Sections from Records

```css
.remove-linked-section-container {
display: none!important;
}
```


#### Remove "Refresh" Icon from Formula Fields - Desktop


```css
.slds-scope .slds-button.js-refresh-formula {
display: none;
}
.slds-scope .control-group .controls .slds-form-element__control.formula-field input.slds-input {
width: 100%;
}
```
#### Remove "Refresh" Icon from Formula Fields - Mobile

```css
.js-refresh-formula {
display: none !important;pointer-events: none;
}
```
#### Prevent Users from Inserting New Records

The following snippet allows you to hide the Add button while using Linked Sections with Compact Cards.

```css
#formContent .ls-card-add-container {
display: none;
}
```

To hide the Add button of a specific linked section with Compact cards, Inspect the element for its data-randomid and use in the following:

```css
#formContent .ls-card-add-container[data-randomid="insert data-randomid here"] { 
display: none; 
}
```

The following snippet allows you to hide the Add button while using Linked Sections WITHOUT Compact Cards

```css
#formContent .add-linked-section {
display: none;
}
```

#### Prevent Users from Inserting more than one New Record
Replace "woli" with the section name.

```css
div[data-section-name="woli"] div:nth-of-type(2) button:nth-child(2){
display: none;
}
```



#### Highlight Required Fields by Adding Red Borders

```css
.control-group [required]{
border-color: red;border-width: 2px;
}
```


#### Change The Appearence of Formula Refresh Buttons - Desktop

```css
#formContent .slds-button.slds-button_icon.js-refresh-formula.slds-button_icon-border.input-btn {
	width: 40px;
	height: 40px;
	right: -30px
}#formContent .slds-button.slds-button_icon.js-refresh-formula.slds-button_icon-border.input-btn::before {
	content: "Refresh";
	position: relative;
	top: 24px;
	font-size: 0.8em;
}#formContent .slds-button.slds-button_icon.js-refresh-formula.slds-button_icon-border.input-btn .js-formula-icon {
	fill: #c9c7c5;
  background-color: #c9c7c5;
	stroke: #c9c7c5;
	border-radius: 0.5em;
	position: relative;
	top: -0.8em;
}
```

#### Change The Appearence of Formula Refresh Buttons - Mobile
```css
.js-refresh-formula.slds-button_icon-border.input-btn {
width: 49px;height: 37px;
right: -49px;
}
.js-refresh-formula.slds-button_icon-border.input-btn::before {
content: "Refresh";
position: relative;
top: 24px;
font-size: 0.8em;
}
.js-refresh-formula.slds-button_icon-border.input-btn .js-formula-icon {
fill: #c9c7c5;
background-color: #c9c7c5;
stroke: #c9c7c5;
border-radius: 0.5em;
position: relative;
top: -0.8em;
}
```


#### Adjust The Size of Long Text Question Boxes

```css
/*******************
* Larger Long Text *
*******************/
#formContent .form-section .controls:not(.controls-table) .slds-form-element.long-text-container {
width: calc(100% - 1em); /* change the number in the 1em to make the Long Text wider or narrower*/
max-width: calc(100% - 1em); /* change the number in the 1em to make the Long Text wider or narrower*/
height: 12em; /* change the number here to make the Long Text taller or shorter*/
}

.form-section .control-group .controls:not(.controls-table) .slds-form-element.long-text-container .slds-form-element__control,
.form-section .control-group .controls:not(.controls-table) .slds-form-element.long-text-container .slds-form-element__control textarea {
height: 100%;
}
```

#### Adjust The Size of Picklist Questions

```css
/*******************
* Wider Picklists *
*******************/
.slds-scope .form-horizontal .slds-form-element__control .slds-select_container {
  max-width: 500px;
  width: 500px;
}
.slds-scope .slds-select_container .slds-select {
  max-width: 500px;
  width: 500px;
}
```


#### Form Template Name Color

```css
.template-name-width {color: #A95014;}
```


#### Form Background Color - Desktop


```css
body#complete-form main {
background-color: #94E9E8;
}
```
#### Form Background Color - Mobile
```css
div#formContent {
background-color: #94E9E8
}
```

#### Form Background Image - Desktop


```css
body#complete-form main{
background: url('https://images.pexels.com/photos/235985/pexels-photo-235985.jpeg') no-repeat top left;
background-size: cover;
background-attachment: fixed;
}
```
#### Form Background Image - Mobile
```css
div#formContent {
background: url('https://images.pexels.com/photos/235985/pexels-photo-235985.jpeg') no-repeat top left;
background-size: cover;
background-attachment: fixed;}
```

#### Form Logo (png/jpg image size 50 X 46) - Desktop


```css
@media screen and (min-width: 400px) {
 .buttons-fixed:before {
 /* Replace the URL between the '' a a URL to your own image. */
 content: url('https://cdn2.hubspot.net/hubfs/2381843/Youreka/yWhiteLogo-711341-edited.png');
 
 /* If your image doesn't have a background color, you can set it here. */
 background: #913A93;
 
 display: block;
 width: 66px;
 height: 62px;
 top: 0;
 right: 0;
 position: absolute;
 padding-top: 10px;
 padding-left: 20px;
 }
}
```
#### Form Logo (png/jpg image size 50 X 46) - Mobile
```css
@media screen and (min-width: 400px) {.formName:before 
{/* Replace the URL between the '' a a URL to your own image. */
content: url('https://cdn2.hubspot.net/hubfs/2381843/Youreka/yWhiteLogo-711341-edited.png');
/* If your image doesn't have a background color, you can set it here. */
background: #913A93;
display: block;
width: 66px;
height: 62px;
top: 0;
right: 0;
position: absolute;
padding-top: 10px;
padding-left: 3px;}}
```

#### Form Width - Desktop


```css
.containerBox {
 width: 750px;
}
```
#### Form Width - Mobile

```css
.containerBox {width: 750px !important;margin-left: 3% ;}
```

#### Section Header Font Color

```css
span.title-text { 
    color: #4578c4;  
}
```


#### Section Header and Footer Background Color & Border Color

```css
/* Header Background Color */
.slds-scope .slds-card__header.OR-card__header {
    background-color: lightsalmon;
    border-color: lightsalmon;
    margin-bottom: 4px;
}

/* Header Background Color */
.slds-scope #formContent .slds-card.form-section {
    background-color: lightsalmon;
}

/* Footer Background Color */
.slds-card__footer.OR-card__footer {
    background-color: lightsalmon;
    border-color: lightsalmon;
}
```


#### Section Body Background, Border, and Text Color

```css
.slds-card__body.OR-card__body.slds-p-horizontal_xx-small {
    background-color: lightblue;
    border-color: darkblue;
    color: red; 
}
```


#### Checkbox and Radio Button Label Colors

```css
.slds-form-element__label, .slds-form-element__label {
color: #FFA500 !important;
}
```

#### Add More than Two Columns to a Standard Section
See https://support.youreka.io/hc/en-us/articles/11073754516759 for more information.
```css 
 .form-section .slds-card__body {
    column-count: 3;
    column-gap: 0px;
    padding-top: 30px !important;
  } 

  .date {
      width: 100%;
  }

  .right-addon {
      width: 100%;
  }

  .slds-card__body > div:nth-child(1) {
      height: 1530px;
  }

   .control-group {
    page-break-inside: avoid;
    }

  @media only screen and (min-width: 300px) and (max-width: 1370px) and (orientation: portrait) {
      .form-section .slds-card__body {
            column-count: 3;
            column-gap: 18px;
            padding: 8px 4px 0px;
      }

      .control-group {
          width: 102%;
          page-break-inside: avoid;
      }

      .date, .right-addon  {
          width: 100%;
      }

      .form-section div.control-group:first-child {
        margin-top: -6px !important;
      }     
  }

  @media only screen and (min-width: 934px) and (max-width: 1370px) and (orientation: landscape) {

      .form-section .slds-card__body {
            column-count: 3;
                column-gap: 150px;
          }

          .control-group {
              width: 102%;
              page-break-inside: avoid;
          }

          .date, .right-addon {
              width: 100%;
          }

          .form-section div.control-group:first-child {
            margin-top: -6px !important;
          }
  } 
```

#### Linked Section Table View
See https://support.youreka.io/hc/en-us/articles/11078711682455 for more information.
```css
 .form-section .slds-card__body .label-width {
   display: none;
 }

 p {
   text-align: center;
   color: rgb(57, 89, 125);
   font-family: "Salesforce Sans", Arial, sans-serif;
   padding-top: 1px !important;
 }

 .form-section[data-section-index="0"] .slds-card__body .label-width {
   display: initial !important;
 }

 div.form-section:nth-child(4)>div:nth-child(3)>div:nth-child(1) {
   margin-left: 121px;
   page-break-inside: avoid;
 }

 .slds-card__body[data-placeholdersection="true"] {
   justify-content: center;
   display: flex;
 }

 div.form-section:nth-child(3)>div:nth-child(3) {
   justify-content: center;
   display: flex;
 }

 div[data-question-text="Rich-Free-Text"] {
   width: 160% !important;
   display: table;
 }

 .slds-scope .slds-card__body.OR-card__body {
   background-color: #fff;
   border-top: 2px solid rgb(216, 221, 230);
   border-bottom: 2px solid rgb(216, 221, 230);
   padding-top: 6px;
   padding-bottom: -9px !important;
   margin-bottom: -15px !important;
   width: 100%;
 }

 .slds-scope .slds-input {
   background-color: #fff;
   border: 1px solid #dddbda;
   border-radius: .25rem;
   width: 180% !important;
   transition: border .1s linear, background-color .1s linear;
   display: inline-block;
   padding: 0rem 1rem 0 .75rem;
   line-height: 1.875rem;
   min-height: calc(1.875rem + (1px * 2));
   margin-left: 9px;
   margin-right: 9px;
   text-align: center;
 }

 .slds-scope .slds-card__body.OR-card__body {
   background-color: #fff;
   border-top: 2px solid rgb(216, 221, 230);
   border-bottom: 2px solid rgb(216, 221, 230);
   width: 100%;
   height: 5.3rem !important;
   padding-top: 18px;
 }

 .slds-scope .slds-card__footer.OR-card__footer {
   border-top: none;
   margin-top: 0;
   background-color: rgb(244, 246, 249);
   margin-bottom: -60px
 }

 .form-horizontal .controls {
   margin-top: 0px !important;
   text-align: left;
 }

 div.form-section:nth-child(4)>div:nth-child(3) {
   height: 75px !important;
 }
 
 /* Set Column Count and Column Gap Here */
 .form-section .slds-card__body {
  column-count: 6;
  column-gap: 0px;
}

 .add-linked-section {
   margin-left: 36px !important;
 }

 .slds-scope .slds-m-bottom_small {
   margin-bottom: 1.8em !important;
 }

 #formContent>div:first-of-type .title-text {
   display: block !important;
 }

 #formContent>div:first-of-type .slds-card__footer {
   margin-bottom: 3px;
 }

 .title-text {
   display: none;
 }

 .slds-scope .slds-card__header.OR-card__header {
   margin-bottom: 9px !important;
 }
```
