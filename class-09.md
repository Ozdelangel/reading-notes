## Events
1. select the element you want the script to respond to
2. indicate which event the selected node will trigger the response
3. state the code you want to run when the event occors

- those are the basic steps on how to deal with events
### Event Bubbling
- the event starts at the most specific node and flows outwars to the least specific one
- this will be the default event flow
### Event Capturing 
- the event starts at the least specific nodw and flows inwards

the flow of events only really matters when your code has Event Handlers on an element and one of its ancestors or decendant elements

# Forms
- A user fills in a form and then presses a button to submit
- the name of each formcontrol is sent to the server along with the value
-the server processes the infor using the language
-the server creates a new page to send back to the browser based on the info received