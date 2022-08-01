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
/*Import the font into the CSS*/
@import url('https://fonts.googleapis.com/css?family=Indie+Flower');
/*Apply the font family to the document body*/
body {
 font-family: 'Indie Flower', cursive;
}
/* Apply the font family to the form container */
.slds-scope {
 font-family: 'Indie Flower', cursive;
}
/*Apply the font for the headings, table and titles */
.slds-scope h1,
.slds-scope h2,
.slds-scope h3,
.slds-scope h4,
.slds-scope h5,
.slds-scope h6,
.slds-scope th,
.slds-scope td {
 font-family: 'Indie Flower', cursive;
}
/*Apply the font family to the form fields*/
.containerBox input[type=text],
[type=number],
[type=date],
[type=datetime-local],
[type=url],
[type=phone],
[type=email] {
 font-family: 'Indie Flower', cursive;
}
```    


#### Font Color

```css
/*Apply the font color to the document body*/
body {
 color: #ff9900;
}
/* Apply the font color to the form container */
.slds-scope {
 color: #ff9900;
}
/*Apply the font color for the headings, table and titles */
.slds-scope h1,
.slds-scope h2,
.slds-scope h3,
.slds-scope h4,
.slds-scope h5,
.slds-scope h6,
.slds-scope th,
.slds-scope td {
 color: #ff9900;
}
/*Apply the font color to the form fields*/
.slds-scope .slds-input {
 color: #ff9900;
}
.containerBox input[type=text],
[type=number],
[type=date],
[type=datetime-local],
[type=url],
[type=phone],
[type=email] {
 color: #ff9900;
}
/*Apply the font color to the buttons*/
.slds-scope .slds-button_inverse,
.slds-scope .slds-button_inverse:link,
.slds-scope .slds-button_inverse:visited,
.slds-scope .slds-button-group .slds-button_icon-inverse,
.slds-scope .slds-button-group .slds-button_icon-inverse:link,
.slds-scope .slds-button-group .slds-button_icon-inverse:visited,
.slds-scope h2.title-form-section,
.slds-scope .slds-select_container select {
 color: #ff9900;
}
/*Apply the font color to the form labels*/
.form-horizontal .control-label {
 color: #ff9900!important;
}
.slds-scope .slds-form-element__label {
 color: #ff9900;
}
 
.slds-scope h2.title-form-section {
 color: #ff9900;
}
 
.slds-scope .save-button-container button {
 border-color: #ff9900;
}
 
/* Apply Font Color to Form Title and Sub Title */
h1.formName,
h3.form-number {
 color: #ff9900;
}
 
/* Apply Font Color to Free Text Question Type */
.slds-scope div.control-group.slds-text-align_center span{
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
.slds {
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
.slds #formContent h3.slds-text-heading--small {
	font-size: 1.286em;
}
```

#### Attachment Upload Button Font Size

```css
.slds span.slds-button {
	line-height: 2.43em;
}
```

#### Section Header Relative Font Size

```css
.form-section.slds-card h2 {
	font-size: 1.28em;
}
```
#### Specific Section Header Relative Font Size
In order for this CSS to work, you need to replace the randomid with the randomid that corresponds to the section that you intend to adjust. disco__RandomId__c can be found on the Section record in Salesforce.
```css
[data-randomid="27d6b101"].form-section .title-form-section .title-text {
	font-size: 1.28em;
}
```

#### Checkbox/Radio Button Option Label Text Size

```css
.slds .slds-form-element__control .slds-radio .slds-form-element__label,
.slds .slds-form-element__control .slds-checkbox .slds-form-element__label {
	font-size: 1em;
}
```
<br/>


## Button and Icon Adjustments
<br/>
This CSS Snippet section will allow you to customize various button and icon sizes on Youreka Forms.

#### Save Buttons Size

```css
.slds .buttons-fixed button {
	line-height: 2.5em;
} 
```     


#### Go To Page Select Icon Size 

```css
.slds .buttons-fixed .slds-select.goToPage,
.slds .buttons-fixed .pagination-container .slds-select_container,
.slds .buttons-fixed .pagination-container .slds-select_container select {
	width: 7.15em;
	height: 2.44em;
}
```     

#### Select Arrows Size 

```css
.slds #mainForm .slds-select_container:before,
.slds #mainForm .slds-select_container:after {
  border-left-width: 0.214em;
  border-right-width: 0.214em;
}
.slds #mainForm .slds-select_container:before {
  border-bottom-width: 0.357em;
  top: calc((2.429em / 2) - 0.429em);
}
.slds #mainForm .slds-select_container:after {
  	border-top-width: 0.357em;
  	bottom: calc((2.429em / 2) - 0.429em);
}
```  

#### Button Border Radius

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
#### Button Icon Adjustments

```css
.slds svg.slds-button__icon {
	height: 1.143em;
	width: 1.143em;
}
```  



#### Attachment Upload Button

```css
.slds button.slds-button {
	line-height: 2.385em;
}
```

#### Checkbox/Radio Button Size

```css
.slds .slds-form-element__control .slds-radio .slds-radio--faux,
.slds .slds-form-element__control .slds-checkbox .slds-checkbox--faux {
	width: 1em;
	height: 1em;
}
```

#### Checkbox & Radio Button check size

```css
.slds .slds-form-element__control .slds-radio [type="radio"]:checked + .slds-radio--faux::after, 
.slds .slds-form-element__control .slds-radio [type="radio"]:checked ~ .slds-radio--faux::after
.slds .slds-form-element__control .slds-checkbox [type="checkbox"]:checked + .slds-checkbox--faux::after, 
.slds .slds-form-element__control .slds-checkbox [type="checkbox"]:checked ~ .slds-checkbox--faux::after {
	border-bottom-width: 0.143em;
  	border-left-width: 0.143em;
	height: 0.286em;
  	width: 0.59em;
}
```

#### Date Input Selector Icon

```css
.slds .slds-form-element .input-glyphicon-calendar {
  	padding-top: 0.5em;
}
```
<br/>

    
## Form Design
<br/>
This CSS Snippet section will allow you to customize the color of text, backgrounds, and borders of various elements on Youreka Forms.

#### Save Buttons Bar

```css
.slds .buttons-fixed {
    background-color: #009ACD;
}
```




#### Form Template Name

```css
h1.formName,
h3.slds-text-heading--small {
   color: #A95014; 
}
```


#### Form Background Color

```css
body#complete-form.slds {
    background-color: #94E9E8;
}
```

#### Form Background Image

```css
body#complete-form main{
 background: url('https://2j5zg2h1itk3tosw21k7acb1-wpengine.netdna-ssl.com/wp-content/uploads/2018/06/formBgImage.jpg') no-repeat top left;
 background-size: cover;
 background-attachment: fixed;
}
 
h1.formName {
 color: #fdfdfd;
 text-shadow: 2px 2px #d3d3d3;
}
```

#### Form Logo

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

#### Form Width

```css
.containerBox {
 width: 750px;
}
```


#### Section Header Font Color

```css
.slds .currentPageContainer { 
    color: #ecf2fb;  
}
```


#### Section Header and Footer Background Color & Border Color

```css
.slds .slds-card { /* ELEMENTS: Section Header and Footer */
    background-color: #418638;
    border-color: #94E9E8;
}
```


#### Section Body Background, Border, and Text Color

```css
.slds .slds-card__body.OR-card__body.slds-p-left--small { 
    background-color: #75A05F;
    border-color: #94E9E8;
    color: #fff;  
}
```

#### Attachments Count Badge, Attachments, Multi-select Picklist Options Text & Background Color

```css
.slds .controls .selected-files .file-preview, 
.slds .controls .slds-file-selector .slds-badge.slds-theme--info,
.ms-selectable .ui-widget-content.ui-selectee.ui-selected {
    color: #75A05F;  
    background-color: #fff;
}
```

#### Checkbox and Radio Button Label Colors

```css
.slds .slds-form-element__control .slds-form-element__label,
.slds .slds-card__body.OR-card__body.slds-p-left--small  .control-label { 
    color: #fff !important;  
} 
```
