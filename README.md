# Orbit Web Portal

A modern, responsive web portal that serves as a centralized hub for accessing popular web services and search functionality.

## Project Overview

Orbit is a clean, visually appealing web portal designed to provide quick access to frequently used web services like YouTube, Facebook, Instagram, LinkedIn, ChatGPT, Google, Twitter, Google Classroom, Google Meet, and WhatsApp. The interface features a gradient-themed design with platform-specific colors and a Google search functionality.

## Features

- Responsive design that works on desktop, tablet, and mobile devices
- Platform-specific styling for each service button
- Integrated Google search with fallback to Bing
- Smooth hover animations and transitions
- Clean, modern UI with gradient effects

## Technologies Used

- HTML5
- CSS3 with CSS Variables for theming
- JavaScript (for search functionality)
- Font Awesome icons
- Google Fonts (Segoe UI)

## Setup Instructions


3. Open the `index.html` file in your web browser:

The project can be viewed directly in any modern web browser without any additional dependencies or build processes.

orbit-web-portal/
├── index.html
├── README.md
└── (optional assets folder for future enhancements)


## Customization

To add new services:
1. Add a new `<a>` element in the buttons container
2. Create a corresponding CSS class with the desired background color
3. Add the appropriate Font Awesome icon

## Challenges Faced

- Creating a consistent design language across all platform buttons
- Implementing responsive design for various screen sizes
- Ensuring the search functionality works correctly with proper fallback

## Future Enhancements

- Customizable button arrangement
- Ability to add custom links
- Dark/light mode toggle
- Local storage for user preferences

## Contributing

Feel free to fork this project and submit pull requests for any improvements.

HTML Code Improvements
I noticed a small issue in your JavaScript code. The search URLs in the performSearch() function are missing quotation marks. Here's the corrected version:

javascript
function performSearch() {
    const query = document.getElementById('search-input').value.trim();
    if (query) {
        // Try Google first, fallback to Bing if Google is blocked
        try {
            window.open(`https://www.google.com/search?q=${encodeURIComponent(query)}`, '_blank');
        } catch {
            window.open(`https://www.bing.com/search?q=${encodeURIComponent(query)}`, '_blank');
        }
    }
}

GitHub Repository Setup Instructions
Create a new repository on GitHub named "orbit-web-portal"

Set the repository to public

Upload your HTML file (renamed to index.html)

Create a README.md file using the template above

Customize the README with your specific information

Once you've set up your repository, please share the link (it will be in the format: https://github.com/your-username/orbit-web-portal), and I'll be happy to review it further.

