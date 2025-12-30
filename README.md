# React Admin Dashboard

A fully-featured, professional admin dashboard built with React and Material-UI, showcasing enterprise-level packages and best practices for production applications.

![Dashboard Preview](https://claude.ai/chat/public/assets/dashboard-preview.png)

## 🌟 Features

### Core Functionality

- **Light/Dark Mode Toggle** - Seamless theme switching with persistent preferences
- **Responsive Sidebar** - Collapsible navigation with icons and clean organization
- **Interactive Data Tables** - Advanced Material-UI DataGrid with filtering, sorting, and export capabilities
- **Form Management** - Full validation using Formik and Yup
- **Calendar Integration** - Full-featured calendar with event management using FullCalendar
- **Data Visualization** - Multiple chart types (Bar, Line, Pie, Geography) using Nivo Charts

### Pages Included

1. **Dashboard** - Overview with revenue stats, transactions, and multiple chart widgets
2. **Team Management** - Data grid displaying team members with role-based access levels
3. **Contacts** - Contact list with toolbar for filtering and exporting
4. **Invoices** - Invoice tracking with checkbox selection
5. **Profile Form** - User creation form with comprehensive validation
6. **Calendar** - Interactive calendar for event scheduling
7. **FAQ Page** - Accordion-based frequently asked questions
8. **Charts** - Dedicated pages for Bar, Pie, Line, and Geography charts

## 🛠️ Tech Stack

### Core Technologies

- **React** - Frontend framework
- **Material-UI (MUI)** - Component library and design system
- **React Router DOM** - Client-side routing

### Data & Forms

- **Formik** - Form state management
- **Yup** - Schema validation
- **Material-UI DataGrid** - Advanced data tables

### Visualization

- **Nivo Charts** - Data visualization library
    - Bar charts
    - Pie charts
    - Line charts
    - Geography/Choropleth maps
- **FullCalendar** - Calendar and event management

### UI Components

- **React Pro Sidebar** - Professional sidebar navigation
- **Material-UI Icons** - Icon library

## 📦 Installation

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Setup Instructions

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/react-admin-dashboard.git
cd react-admin-dashboard
```

2. **Install dependencies**

```bash
npm install
```

3. **Required packages** (if installing manually):

```bash
# Core MUI packages
npm install @mui/material @emotion/react @emotion/styled

# Data Grid
npm install @mui/x-data-grid

# Icons
npm install @mui/icons-material

# Routing
npm install react-router-dom@6

# Sidebar
npm install react-pro-sidebar

# Forms and Validation
npm install formik yup

# Calendar
npm install @fullcalendar/core @fullcalendar/daygrid @fullcalendar/timegrid @fullcalendar/list @fullcalendar/interaction

# Charts
npm install @nivo/core @nivo/pie @nivo/line @nivo/bar @nivo/geo
```

4. **Start the development server**

```bash
npm start
```

The application will open at `http://localhost:3000`

## 📁 Project Structure

```
react-admin-dashboard/
├── public/
│   └── assets/
│       └── user.png
├── src/
│   ├── components/
│   │   ├── BarChart.jsx
│   │   ├── LineChart.jsx
│   │   ├── PieChart.jsx
│   │   ├── GeographyChart.jsx
│   │   ├── Header.jsx
│   │   ├── ProgressCircle.jsx
│   │   └── StatBox.jsx
│   ├── scenes/
│   │   ├── global/
│   │   │   ├── Sidebar.jsx
│   │   │   └── Topbar.jsx
│   │   ├── dashboard/
│   │   │   └── index.jsx
│   │   ├── team/
│   │   │   └── index.jsx
│   │   ├── contacts/
│   │   │   └── index.jsx
│   │   ├── invoices/
│   │   │   └── index.jsx
│   │   ├── form/
│   │   │   └── index.jsx
│   │   ├── calendar/
│   │   │   └── index.jsx
│   │   ├── faq/
│   │   │   └── index.jsx
│   │   ├── bar/
│   │   │   └── index.jsx
│   │   ├── pie/
│   │   │   └── index.jsx
│   │   ├── line/
│   │   │   └── index.jsx
│   │   └── geography/
│   │       └── index.jsx
│   ├── data/
│   │   ├── mockData.js
│   │   └── mockGeoFeatures.js
│   ├── theme.js
│   ├── App.js
│   └── index.js
├── package.json
└── README.md
```

## 🎨 Theming

The application uses a custom theme configuration with support for both light and dark modes:

- **Color Tokens** - Organized color palette with multiple shades
- **Context API** - React Context for global theme state
- **Material-UI Theme Provider** - Integrated with MUI's theming system
- **Custom Scrollbar** - Styled scrollbar matching the theme

### Color Scheme

- **Primary** - Dark blue (#141b2d in dark mode)
- **Secondary** - Green accent (#4cceac)
- **Additional Accents** - Red and blue accents for various UI elements

## 🔧 Key Features Explained

### Data Grid Tables

Three different implementations showcasing:

- Custom cell rendering
- Column customization
- Checkbox selection
- Export functionality
- Filtering and sorting
- Custom styling

### Form Validation

Formik and Yup integration featuring:

- Real-time validation
- Custom error messages
- Email format validation
- Phone number regex validation
- Touch-based error display

### Calendar System

FullCalendar implementation with:

- Multiple view modes (Month, Week, Day, List)
- Event creation via click
- Drag-and-drop event management
- Event deletion
- Custom styling

### Charts

Nivo charts with:

- Custom themes matching the app design
- Responsive layouts
- Interactive tooltips
- Dashboard and full-page versions

## 🚀 Usage

### Navigating the Dashboard

- Use the sidebar to navigate between different pages
- Click the hamburger menu to collapse/expand the sidebar
- Toggle between light and dark mode using the sun/moon icon in the top bar

### Managing Data

- **Tables**: Click column headers to sort, use the toolbar for filtering
- **Forms**: Fill out the profile form with validation feedback
- **Calendar**: Click dates to add events, click events to delete them

### Viewing Analytics

- Navigate to individual chart pages for detailed views
- Dashboard provides an overview with multiple widgets

## 🎓 Learning Outcomes

This project demonstrates:

- **Component Architecture** - Proper file/folder organization using the "Ducks pattern"
- **State Management** - React Context for global state
- **Routing** - React Router for navigation
- **Form Handling** - Best practices with Formik and Yup
- **Data Visualization** - Integration of chart libraries
- **Theming** - Custom theme implementation with light/dark mode
- **Material-UI Mastery** - Advanced usage of MUI components
- **CSS Grid & Flexbox** - Responsive layouts
- **Best Practices** - Clean code, reusable components, and proper imports

## 📝 Customization

### Adding New Pages

1. Create a new folder in `src/scenes/`
2. Add an `index.jsx` file with your component
3. Register the route in `App.js`
4. Add a navigation item in `Sidebar.jsx`

### Modifying Colors

Edit the color tokens in `src/theme.js` to customize the color scheme for both light and dark modes.

### Updating Mock Data

Modify files in `src/data/` to change the sample data displayed in tables and charts.

## 🐛 Known Issues

- The application is optimized for desktop viewing
- Mobile responsiveness could be improved
- Some features (search, notifications, settings) are UI-only without backend integration

## 🔮 Future Enhancements

- [ ] Full responsive design for mobile devices
- [ ] Backend API integration
- [ ] User authentication and authorization
- [ ] Real-time data updates
- [ ] Additional chart types
- [ ] Export functionality for all data views
- [ ] Advanced filtering options
- [ ] User profile management

## 📄 License

This project is open source and available under the [MIT License](https://claude.ai/chat/LICENSE).

## 🙏 Acknowledgments

- Material-UI for the component library
- Nivo for beautiful chart components
- FullCalendar for calendar functionality
- EdRoh for the tutorial inspiration

---

**Built with ❤️ using React and Material-UI**
