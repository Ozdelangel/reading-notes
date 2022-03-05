HTML Forms - is a group or widget on a web page which can be used to collect information from users submissions to a server

Working with forms can be complicated. Developers need to write HTML for the form, validate and properly sanitize entered data on the server

A form is defined as a collection of elements inside the `<form>` tags and has at least one `input` element of `type=submit` 

The submit input will be displayed as a button by default that can be pressed by the user to upload the data in all the other input elements.

Actions: the resource/URL where data is to be sent for processing when the form is submitted

Method: the http method used to send the data post or get

The role of the server is to first render the initial state of the form either blank or pre-populated with values

Display all defaults first time it is requested by the server
Receive data from a submit request and bind it to the form
Clean and validate the data
If any data is invalid, re-display the form, this time with any user populated values
If all data is valid, perform required actions, send and email, return the results of the search, upload a file
Once all actions are complete, redirect the user to another page
Django provides a lot of tools to get these done. The most fundamental is the form class.
