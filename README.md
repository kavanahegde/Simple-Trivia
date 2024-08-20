HTML Structure (index.html):

Title and Head Section:
The HTML file is titled "Vacationista Search," and a CSS file named style.css is linked for styling (though the CSS file is not provided here).
Body Content:
Heading: The page starts with a heading <h1> titled "Vacationista Search."
Message Paragraph: A <p> element with an id of "message" is used to display whether the property matches the user's requirements.
Listing Details: The first <ul> contains <li> elements that display details about a specific vacation property, such as the number of beds, review score, cost per night, pool availability, and location.
User Requirements: The second <ul> lists the user's requirements for a vacation property, such as minimum beds, minimum review score, maximum cost, pool requirement, and location preference.
JavaScript Link: The HTML file includes a link to the external script.js file, where the logic for property matching is implemented.
JavaScript Functionality (script.js):

Property Details and User Preferences:
Variables are defined at the beginning of the script to store the property details (e.g., beds, reviewScore, costPerNight, pool, country) and the user's requirements (e.g., minBeds, minReviewScore, maxCostPerNight, needPool, inCountry).
Matching Logic:
The match variable is initialized as true. Several if statements then evaluate whether the property meets the user's requirements.
If the property has fewer beds than required, a lower review score, is in the wrong country, lacks a pool (if needed), or is more expensive than the user's maximum budget, the match variable is set to false.
If the property’s cost is within the user’s budget, the script calculates the saving compared to the maximum cost.
Displaying the Match Result:
If the property meets all the user’s requirements (match === true), a message is constructed and displayed in the HTML element with the id "message". If the property is cheaper than the maximum budget, the saving amount is also displayed.
If the property does not meet the requirements, a message stating "Sorry, this property is not suitable." is displayed.
Updating the Listing Details:
The querySelectorAll method selects all <li> elements in the document, and the script updates these list items with the property details and user requirements dynamically.
Overall Functionality:
This code snippet allows users to compare a specific vacation property against their personal requirements. The script determines if the property is a suitable match based on factors such as the number of beds, review score, cost per night, pool availability, and location. The result of this comparison is then displayed to the user, offering feedback on whether the property is a match, along with potential savings. The property details and user preferences are dynamically updated in the HTML to reflect the comparison.






