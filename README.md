# formValidator
Hand coded form validator using Plain Old Javascipt. No Frills. ES5 Standard Only.

API Documentation
- DOM.addClass: Adds a css class to a DOM Element.
- DOM.removeClass: Removes a css class from a DOM Element.
- DOM.form.smoker.currentAge: Returns an integer value with the current age of the member
- DOM.form.smoker.checkSmokerAge: Disables smoker checkbox for members under 18. Invokes alert when box is 
  checked if member is underage.
- DOM.form.buttons.disableButtons: Disables add/submit buttons when validation errors occur.
- DOM.form.buttons.enableButtons: Enables add/submit buttons when validation errors are cleared.
- DOM.form.setPristine: Similar to Angular setPristine() Method, clears form and all added dirty,touched
  classes.
- DOM.form.touchEl: Adds "touched" class to form elements that have/had focus.
- DOM.form.dirtyEl: Adds "dirty" class to form elements that have/had a value.
- DOM.form.reset: Clears all form values.
- DOM.form.requiredMembers.getMembers: Returns an array of elements with a 'required' property.
- DOM.form.requiredMembers.isRequiredAndValid: Triggered by validation; If all required members have a 
  value(e.g. 'dirty'), it is assumed that the values are valid, because validation can only be triggered if add/submit buttons are enabled.
- DOM.form.validation.validate: checks form elements for errors, creates error messages, adds 'invalid' css 
  class, enables/disables add/submit buttons.
- DOM.form.validation.checkValueOf: Checks form input for a valid value (e.g. Age not a string, etc..).
- DOM.form.validation.isInt: Because isNaN doesn't cover all cases when checking for valid integer values.
- DOM.form.validation.triggerValidate: Triggers validation process on add.
- DOM.form.validation.triggerValidate.underAgeRelationships: Ensures appropriate relationships when 
  relationship options are selected (e.g. No 13 y/o spouses, 5 y/o granparents, etc...).
- DOM.form.validation.enableOptions: Works as an enable/disable options method for the options dropdown. 
  Takes and array and a boolean. enableOptions(arr[,false]) is equivalent to disableOptions.
- create: Instantiates a new member object from the Member class.
- renderNewMember: Renders new Member card to the view.

This program uses: 
--Uses npm
--Uses lite-server

To run this program (make sure you're inside of teh hhbuilder folder:
--npm install
--npm start
