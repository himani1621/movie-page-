Movie Page Project

Overview

The Movie Page project is a web application that provides users with an interface to search for movies and view their details. Utilizing HTML, CSS, and JavaScript, this project also integrates an API for fetching movie data and uses local storage for saving user preferences and watchlists. Below is a detailed overview of the project's features, structure, and instructions for use.

Features

Search Functionality: Users can search for movies using a search bar.
API Integration: Fetches real-time movie data from an external API.
Local Storage: Saves user watchlist and search history in the browser's local storage.
Responsive Design: Ensures the page is accessible across different devices and screen sizes.
Stylish UI: Utilizes Font Awesome icons and custom CSS for an attractive layout.
Navigation Button: Includes a "Go Back" button (hidden by default) for potential navigation features.
Watchlist Button: Allows users to manage and view their watchlist.

Project Structure
index.html - The main HTML file that structures the content of the page.
style.css - The stylesheet that defines the appearance and layout of the webpage.
script.js - The JavaScript file that adds interactivity, integrates with the API, and manages local storage.

File Descriptions

1.index.html

This file contains the HTML structure of the movie page. It includes:

Header Section: Displays the page title, a search form, and buttons for navigation and watchlist.
Main Section: Serves as a container for the main content of the page.

2.style.css

This file contains the CSS rules that style the movie page. It includes:

General Styles: Defines the overall look and feel of the page, including font sizes, colors, and spacing.
Header Styles: Styles for the header section, including the layout of the search form and buttons.
Responsive Design: Media queries to ensure the page is responsive and works well on various screen sizes.

3.script.js

This file contains the JavaScript code that adds functionality to the page. It includes:

API Integration: Fetches movie data from an external API (e.g., OMDb API) based on user input.
Search Functionality: Handles user input in the search bar and fetches movie details from the API.
Local Storage: Manages the saving and retrieval of user watchlist and search history in the browser's local storage.
Button Interactions: Manages the visibility and functionality of the "Go Back" and "Watchlist" buttons.

API Integration
The project uses the TMDb API for retrieving movie information. You will need an API key to access the API. Here’s how you can integrate the API:

Obtain an API Key:

Sign up at TMDb API to get an API key.

API Endpoint:

The base URL for the API is http://www.tmdbapi.com/.
Use the following format to fetch movie data:
Copy code
http://www.tmdbapi.com/?apikey=YOUR_API_KEY&s=SEARCH_QUERY
Replace YOUR_API_KEY with your actual API key and SEARCH_QUERY with the movie title or keywords.
Usage in script.js:

Implement fetch requests to get data from the API and update the UI with movie information.
Local Storage
Local storage is used to save user preferences and watchlist items. Here’s how it’s utilized:

Save Watchlist:

When a user adds a movie to their watchlist, the movie details are saved in local storage using localStorage.setItem('watchlist', JSON.stringify(watchlist)).
Retrieve Watchlist:

On page load, the watchlist is retrieved from local storage using JSON.parse(localStorage.getItem('watchlist')).
Save Search History:

Save search queries in local storage to provide quick access to recent searches.

Usage in script.js:

Implement functions to add, remove, and retrieve items from local storage.
How to Use
Clone or Download the Repository:

Clone the repository using Git: git clone <repository-url>
Or download the ZIP file and extract it to your local machine.
Open the Project:

Navigate to the project directory.
Open index.html in a web browser to view the movie page.

Search for Movies:
Enter a movie name in the search bar and press Enter or click the search icon to fetch movie details.

Manage Watchlist:
Click the "Watchlist" button to view and manage your watchlist. Movies can be added or removed from the list, and changes will be saved in local storage.
Explore the Interface:

Use the "Go Back" button (if implemented) to navigate back to previous pages or states.

Technology Stack
HTML: For structuring the content of the page.
CSS: For styling and layout, including responsive design.
JavaScript: For adding interactivity, integrating with the API, and managing local storage.
Font Awesome: For icons used in the project.

Future Enhancements
Advanced Movie Data: Integrate more features from the API, such as movie trailers or reviews.
Enhanced Watchlist Management: Allow users to categorize or prioritize their watchlist items.
User Authentication: Implement user accounts to manage personal watchlists and preferences.


Acknowledgments
TMDb API: For providing movie data.
Font Awesome: For providing icons used in the project.
HTML, CSS, and JavaScript Communities: For the resources and tutorials that helped in building this project.

