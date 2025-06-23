# ev-dashboard
Data Visualization Dashboard
This project is a frontend data visualization platform built with React, Redux Toolkit, and Tailwind CSS. It provides a user interface for analyzing electric vehicle (EV) data such as charging stations, fleet sizing, and parking distribution. The goal was to build a clean, responsive, and interactive user experience with minimal dependencies and modern UI practices.

Features Implemented
Three main screens for Charging Stations, Fleet Sizing, and Parking

A responsive top navigation bar with a search input

A sidebar menu with icon-based navigation

KPI cards with hover effects and dynamic content

Expandable "Best Scenario Results" section with animated transitions

A variable editing panel with search, autofill, and reset functionality

A context-aware help window that appears with a hover delay

Custom line chart with tooltips, active points, and vertical reference lines

Global state management using Redux Toolkit

Reusable and modular components with Tailwind-based styling

Technical Decisions and Trade-offs
Tailwind CSS was used for styling to ensure speed, consistency, and responsiveness across screen sizes. Redux Toolkit was selected for state management due to its simplicity and scalability. Chart rendering was handled by Recharts because of its tight integration with React and the ability to customize tooltips and visuals easily.

Authentication was not implemented, as the focus of the project was primarily on UI behavior and state interaction. Data is currently mocked locally; no backend or API integration was included to keep the project frontend-focused for the purposes of the assessment.

Known Limitations
This project does not include backend integration or persistent data. Variable selection logic is simple and does not validate logical dependencies between variables. Accessibility features such as keyboard navigation and ARIA roles are minimal. Authentication, data validation, and internationalization are not included.

Time Spent
The project took approximately two full days. Around 6–8 hours were spent on component layout and styling, 2-3 hours on implementing the chart, another 6–8 hours on interactive UI features such as the variable panel and scenario section, and the rest of the time was spent on cleanup, animations, and testing.

Local Development Instructions
Clone the repository:

git clone https://github.com/Sainazardosht/ev-dashboard
cd ev-dashboard
Install dependencies:
npm install

Start the development server:
npm run dev
The application will be available at http://localhost:5173 by default.

Setup Instructions
The project uses Vite as the build tool and dev server. All configuration is located in the vite.config.js file. Entry point is main.jsx. The App.jsx file sets up the routing and layout structure. All Redux slices are located under src/features. UI components are under src/components.

To modify or add more charts, update or extend the LineChartBox component using Recharts. For new screens or layout changes, refer to the SimulationResults and VariablesPanel components as structural references.
