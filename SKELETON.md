<div align="center">

# Roadmap

</div>

<br/>

## User inputs vacation information in a form

### Add dropdown calendar for user to select start and end date (all information required)

- Prevent user from adding dates that have already passed
- Prevent user from adding an end date prior to the start date

### User adds location information (all information required) 🗺️

- Text input for starting city
- Dropdown menu for starting state
  - Have "Other" section that when selected adds another text box -> useful for international locations
- Text input for destination city
- Dropdown menu for destination state
  - Have "Other" section that when selected adds another text box -> useful for international locations

<br />

---

<br />

## User receives information based on input

- Submit button
- Loading screen
  - Add an animation
  - Add a random message ("Don't forget your iphone charger" etc.)
- Calculate time between current date and vacation start date
  - Start countdown to vacation ✈️
- Calculate time between start date and end date
  - Send API call to get weather information based on the vacation dates
  - Output weather data as _dynamically created_ accordions
- Send API call to get image of destination city
  - Output image at top of results page
- User has option to save trip
  - Use local storage

## User options regarding results

- Save trip
  - Save trip in local storage
  - Use destination city as saved trip name
  - _if_ destination city button already exists, name it "city 2" and order it based on start date
  - Pop up saying trip has been saved
- Edit trip
  - User is returned to the input page with all of the information already populated
- Start over
  - Refreshed the page

## User interaction with saved trips

- Saved trips on bottom of page with countdown clock
- User clicks on button to see results
- Option to edit or delete trip  
   _if edit:_ User goes back to the main page with the information already populated, then they receive the option to save information. 🛑 Make sure a new saved trip is not created, but that the current trip is updated.  
   _if delete:_ Prompt asks user if they are sure they want to delete. If they select delete, then they receive an alert that trip was deleted. Remove the trip button from the main page.
