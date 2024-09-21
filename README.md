# Let's create the README.md file for the user

readme_content = """
# QuickSell Assignment Priyam Rai NITJ

[View the live project here](https://quick-sell-assignment-priyam-rai.vercel.app/)

This project is a Kanban board built using ReactJS. It interacts with an external API and allows users to group and sort tickets by different criteria such as status, assigned user, or priority. It is designed to match the provided design, using only pure CSS.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Grouping and Sorting](#grouping-and-sorting)
- [API](#api)
- [Folder Structure](#folder-structure)
- [Technologies](#technologies)
- [Screenshots](#screenshots)
- [License](#license)

## Features
- **Grouping**: Users can group tickets by Status, User, or Priority.
- **Sorting**: Tickets can be sorted by Priority (descending) or Title (ascending).
- **Responsive Design**: The application is responsive and adjusts for different screen sizes.
- **State Persistence**: The application saves the user's last view state (grouping and sorting preferences) even after the page is reloaded.
- **Pure CSS**: The UI matches the provided design using only pure CSS, no external libraries like Bootstrap or Tailwind.

## Installation

### Prerequisites
- [Node.js](https://nodejs.org/) (v14 or higher)
- npm or yarn

### Steps
1. Clone the repository:
    \`\`\`bash
    git clone https://github.com/your-username/kanban-board.git
    cd kanban-board
    \`\`\`
2. Install the required dependencies:
    \`\`\`bash
    npm install
    \`\`\`
3. Start the development server:
    \`\`\`bash
    npm start
    \`\`\`
4. Open your browser and navigate to \`http://localhost:3000\` to view the app.

## Usage
Once the application is loaded:
- Click on the "Display" button to select how you want to group the tickets (Status, User, Priority).
- You can also select how to sort the tickets by priority or title.
- The board will update dynamically based on your selection.

## Grouping and Sorting
- **Grouping**: 
  - By Status: Organizes tickets by their current status (e.g., "To Do", "In Progress", "Done").
  - By User: Organizes tickets by the user assigned to them.
  - By Priority: Organizes tickets based on their priority level (Urgent, High, Medium, Low, No Priority).
  
- **Sorting**:
  - By Priority: Sorts tickets by their priority, from highest (Urgent) to lowest (No Priority).
  - By Title: Sorts tickets alphabetically by their title.

## API
The app fetches ticket data from the following API endpoint:
- **API URL**: \`https://api.quicksell.co/v1/internal/frontend-assignment\`

The API returns ticket data in the following format:
\`\`\`json
[
  {
    "id": "1",
    "title": "Ticket Title",
    "status": "To Do",
    "user": "John Doe",
    "priority": 4 // Urgent
  },
  ...
]
\`\`\`

### Priority Levels
- **4** - Urgent
- **3** - High
- **2** - Medium
- **1** - Low
- **0** - No Priority

## Folder Structure
\`\`\`
/src
  /components         # Reusable components for the Kanban Board
    Board.js          # Displays the Kanban board
    Card.js           # Displays individual ticket cards
    Header.js         # Header with display options
    GroupOptions.js   # Component for choosing grouping and sorting options
  /styles
    Board.css         # CSS for Board component
    Card.css          # CSS for Card component
    Header.css        # CSS for Header component
    GroupOptions.css  # CSS for GroupOptions component
  App.js              # Main application file
  App.css             # Global styles
  index.js            # Entry point for React application
\`\`\`

## Technologies
- **ReactJS**: Frontend library used to build the UI.
- **Axios**: For making HTTP requests to the API.
- **Pure CSS**: No external CSS frameworks, only pure CSS for styling.

## Screenshots
Here’s a quick preview of the application:

- **Group by User**  
  ![Group by User](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/de6f9ade-433a-4185-a6df-4d396ea8be2d/Untitled.png)

- **Group by Priority**  
  ![Group by Priority](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2f8e52ba-2b96-40e8-be6a-34e25dd240eb/Untitled.png)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
