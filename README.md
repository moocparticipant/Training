# Accessibility Issue List 

## Page Title 

Screen readers read the title as soon as the page is loaded. It is important to have a page title that reflects what is on the page. Here the page title is “Happy Holidays!” - this is not relevant. Notice on the tab you have opened the page it will show the page title. 

Automatic testing tools can capture if the page title is missing but if it is present but not relevant that may not get flagged. 

## Skip to main link 

If a keyboard user is navigating this page they have to go through all the navigation links to get to the main form. There should be a Skip to main link as the first tab stop of the page if the page contains repeated headers, navigation etc. 

## Focus order 

We expect the focus to move from left to right and top to bottom. But focus jumps to About skipping Home. Then it jumps back to Home. This is not the correct order. 

## Focus indicator contrast 

In the top navigation menu, one link has a lilac focus indicator. This against a white background is not very visible. All active UI components and focus indicators should have sufficient colour contrast to be accessible. This should be at a minimum 3:1 contrast. 

## Keyboard inaccessible content 

On the navigation list, contact link can be clicked by mouse. But for a keyboard user you can’t get to that link. It is not accessible. 

Hovering over the information icon gives information to the user. But this information is not available to screen reader users or keyboard users. 

## Content not marked up as heading 

“Demonstrating Bad Accessibility” is the main heading of this page. It is made to look like a heading, but it is not correctly marked up as a heading. For a screen reader user this will not show as a heading. 

## Hard to read font 

Some text on the page is using a font that is hard to read. A sans Serif font is recommended like Arial or Calibri that is easy to read. 

## Text alignment 

Centred text or justified text is hard to read. It is good practice to left align the text. 

## Non descriptive link text 

“Click here” does not give the user any indication where the link will take them to. 

## Use of colour 

“Click here” link is only differentiated from surrounding text by colour.  

## Fixed width 

This form is set for fixed width. This means if you open the form in a smaller screen you will have to scroll horizontally and vertically 

## Form layout 

The form field names are to the left of the form field. It is much easier for user on any device if the form field name is just above the form field. This is good design practice. 

## Required fields 

No indication of required fields. 

## Form labels 

Currently form labels for email, and date of birth for day is associated with the relevant form input field. You can click on the form label and if it is correctly associated with input field it should take you to the input field. However, this is not always a reliable test because there are different ways of associating form field name with the input. 

This issue can be a blocker for screen reader users as they may not understand what each input field is for. For example, in this page date of birth month and date of birth year are not associated with a label. 

## Visual labels for fields
For the field password there is no visual label.

## Interaction complexity 

The date of birth is split into three separate text fields, increasing interaction complexity. As an alternative you could offer a date input for date of birth which would then be one field. 

## No instructions 

The password field requires users to create a password, but there is no guidance on what an acceptable password should contain. 

## Form instructions as a placeholder 

When user types in the placeholder text disappear. If there are instructions provided for forms, these should not be in a placeholder text. 

## Insufficient colour contrast 

At the bottom of the page there is light purple text on lilac background. The text and background do not have sufficient colour contrast making it harder to read. For normal text to be accessible they require 4.5:1 colour contrast ratio. 

Automated accessibility checkers are generally good at identifying colour contrast issues. 

## On input focus change 

When inserting date of birth, as you type two digits for day the focus moves to month field. When you type two digits the focus moves to year field. For visual users this may be helpful. However, for users relying on screen readers this can be disorientating. The user did not move the focus but on input the form advanced them along to a different field. This is an accessibility failure. Inserting bank details (esp. Sort code) or any field with multiple parts of input is likely to be programmed in this way.  

## All capitals 

All capitals are hard to read due to lack of shape variation in text. For screen reader users CONTACT US may be read as Contact U.S. depending on settings. 

## Animation without option to pause 

Animations playing for longer than 5s need to have a way of pausing. 

## Zoom 

Enlarging the text by zooming does not make the page adapt. This leaves you with both horizontal and vertical scrolling.  

## Error Indication & Correction 

If the form was submitted with an empty field, the field is highlighted in red. However, person with colour vision deficiency or is blind/visually impaired may not be able to spot this difference in colour. Therefore, it is always good practice to indicate what fields need at and provide sufficient instruction for the user to correctly fill that field. 

## Dynamic Messages 

If the form is submitted with at least one empty field, the form generates an error message otherwise the form generates a message to say all form fields were filled. This message is dynamically displayed at the top of the form. However, this message is not accessible to assistive technology users. If you use a screen reader to navigate this form, the error message will not be conveyed. 

This is a technically advanced area of accessibility. You can ask the question to make sure developers take this into consideration in the implementation. 

## Language of page 

Language of a web page is defined so that the assistive tech can accurately interpret (e.g. screen reader can correctly pronounce) the content. This page’s language is not defined.  

Automatic testing can capture this issue.  

## Incorrect heading hierarchy 

The document contains H2 heading and then H4 heading. The heading hierarchy should be maintained H1, H2, H3, H4 and you can’t skip heading levels because for assistive tech users' headings create the document structure.  

Automatic testing can capture this issue. 

## Grouping form fields 

The two radio buttons are not correctly grouped. This can also cause problems for assistive technology users. This is an advanced issue, but where there are input groupings, you can ask the question whether they are correctly grouped. 

## Instructions not associated with input field 

Date of Birth format instructions are provided but this is not associated with the input field. This is an advanced issue to fix but where there are instructions provided, they should always be associated with the input field so that assistive tech users can also access that information. 

## Image without alternative text 

The information icon is missing alternative text. Images should be marked as decorative or given meaningful alternative text. Automated tools can detect missing alternative text but usually cannot judge whether existing text is appropriate for the context. 
