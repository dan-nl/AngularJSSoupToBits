# AngularJS Soup to Bits
Provides a vanilla and complete version of the application used in the [Angular Soup to Bits Screencast][1] at Code School.


## Objectives

1. **Create custom elements** for the different content areas of the application
	 1. review form
      1. form
      1. live-preview
      1. review-fields
	 1. book list
1. **Create the book list dynamically**
	 1. adjust the book rating so that it receives a class of goodRating when the rating is >= 3
	 1. adjust the genres so that they only appear when the genre’s value is true
1. **Show/Hide the review form**
   1. add toggle functionality to the “Create a Review” button so that it shows/hides the create a review form
   1. toggle the text of that button from “Create a Review” to “Cancel” as appropriate
   1. initialise the show state to false
1. **Bind a model to the form fields**
   1. decide on an object name to receive the form field data
   1. initialise that object in the form controller to an empty object
   1. add the appropriate data-binding to each form field for that object
   1. because genre is a set of checkboxes you’ll need to bind this a bit differently
      1. you add a nested object within the one you created in step 2 above
      1. and in the form you pass in the individual value for that checkbox as a property of that nested object
      1. that property will receive a true or false value depending on whether or not the checkbox is checked
1. **Bind the live preview to the form fields**
   1. set the binding to display a default value until a form value is typed in
   1. again, for genre you’ll need to bind a bit differently
      1. you create a repeat that uses (key, value)
      1. and add the key
      1. and display only when the key is true
1. **add a submit handler to the form**
   1. add the new book review to the book list
   1. re-initialise the data model for the form
   1. clear out the form


[1]:https://www.codeschool.com/screencasts/soup-to-bits-shaping-up-with-angular-js