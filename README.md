# JavaScript Project 1: MLB Game and Highlights Viewer

## Description
This project retrieves and displays Major League Baseball (MLB) game data for a specified past date. The project is inspired by an MLB Demo example and leverages JavaScript to fetch data in JSON format from the MLB website. Users can view the home and away team names for games played on a selected day, browse through game highlights, and even play highlight videos in a new browser tab.

## Objectives
1. Retrieve baseball game schedule data for an entered past date.
2. Allow the user to display team names (home and away) for the games played on the selected day using "Next" and "Previous" buttons.
3. Enable the user to browse through game highlight headlines using another set of "Next" and "Previous" buttons.
4. Allow the user to play a highlight video within a new browser tab.

## Requirements
- A web browser supporting JavaScript and HTML5.
- Internet connection to retrieve data from the MLB API.

## Setup
1. Clone the repository.
2. Open the `index.html` file in a web browser.
3. Ensure that the browser has internet access to fetch data from the MLB website.

## Usage
1. Open the `index.html` file in your web browser.
2. Enter a past date in the date input field.
3. Click the "Retrieve MLB Data for this Date" button to fetch the game data for the selected date.
4. Use the "Next Game for this Date" and "Previous Game for this Date" buttons to navigate through the games.
5. View the game highlights by clicking on the "Next Highlight for this Date" and "Previous Highlight for this Date" buttons.
6. To play a highlight video, click on the "Run Playback for this Highlight" button, which will open the video in a new tab.

## Code Explanation

### HTML Structure
The HTML file contains a form for inputting a date and buttons for retrieving and navigating through the MLB game data. The page layout is styled using CSS flexbox for a responsive design.

### JavaScript Functions
- **`retrieveJSON(url)`**: Fetches JSON data from the specified URL using a synchronous AJAX request.
- **`retrieveMLB(givenData)`**: Parses the retrieved JSON data to extract game information, including game IDs, home team names, and away team names, storing them in arrays.
- **`nextGame()` & `previousGame()`**: Functions to navigate through the list of games.
- **`getHighlights()`**: Retrieves and displays the first highlight headline for the selected game.
- **`getFrontHighlights()` & `getBackHighlights()`**: Functions to navigate through the highlight headlines for the selected game.
- **`playHighlight()`**: Opens the video playback for the selected highlight in a new tab.

### CSS Styling
The CSS styles define the layout and appearance of the elements on the page, including the buttons and input fields, using flexbox for alignment and responsive design.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## References
- MLB API Documentation: [MLB API](https://statsapi.mlb.com)
- [W3Schools](https://www.w3schools.com)
- [Stack Overflow](https://stackoverflow.com)
