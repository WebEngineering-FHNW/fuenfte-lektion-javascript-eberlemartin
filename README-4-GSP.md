# WebEngineering Module, Server Pages

## Goals

### Abilities
- Being able to use dynamic content in server pages
- Using pages, templates, taglibs, and layouts
- Testing appropriately

### Knowledge
- Understanding the request-response cycle
- Understanding the four ways of composing server pages plus when to use which
- Where and how to validate
- Optional: using Grails internationalized error messages for generic error display

## Demo/Code walkthrough 

We are using git to walk through the code of InPlaceCalculator
incl. model, view, controller, tests.

Use `git checkout <commit_number>` to see the respective state of development.

You can always go back to the youngest state with `git checkout master`.

### Start of work on InPlaceCalculator

	git checkout cb1fc35
	
Have a look at all artifacts in the commit.

### Intermediate step:more generic field error handling

	git checkout 929dfef	

### Use of _form_row.gsp template for smart, labeled fields	

	git checkout fe5690f
	
### Using a taglib for dynamic content

	git checkout be7b2ac

### Grails specific: fully generic error messages plus I18N

	git checkout 192322a
	
### Using a layout for the form

	git checkout c321126
	

## Practical work (may extend into homework)

Make a Fahrenheit to Celsius converter.

You best make a copy of each artifact that we used for the InPlaceCalculator
(model, view, controller, tests, form_row template).
Just copy the file into the same directory as the original and rename accordingly.

You can reuse the _form_ layout.

You can make use of the following conversion functions:

	double c2f(double c) { c * 1.8d + 32 }
	double f2c(double f) { (f-32) / 1.8d }

It is probably best to work with two input fields: one for fahrenheit, one for celsius,
and calculate a result for each of the inputs separately.

## Homework 

Watch http://guides.grails.org/grails-quickcasts-developing-grails-3-applications-with-intellij-idea/guide/index.html

It is a good 20 minutes introduction to Grails even when you do not use IDEA.
