# 🎯 Conference Event Planner

A **React application** built with Redux Toolkit for comprehensive conference event planning and cost management.

![React](https://img.shields.io/badge/React-18+-blue.svg)
![Redux](https://img.shields.io/badge/Redux_Toolkit-Latest-purple.svg)
![Vite](https://img.shields.io/badge/Vite-4+-yellow.svg)

##  Overview

Web application for event planning with real-time cost calculation, venue management, and interactive user experience. Built with modern React patterns and Redux state management.

##  Features

###  **Venue Management**
- Multi-venue selection (Auditorium, Conference Rooms, Meeting Rooms)
- Smart quantity controls with business rules
- Real-time cost calculation
- Venue-specific booking limits (Auditorium: max 3, Others: max 10)

###  **Technical Features**
- Redux Toolkit state management
- Responsive mobile-first design
- Component-based architecture
- Hash-based navigation

##  Quick Start

```bash
# Clone and install
git clone https://github.com/RitaJind/conference_event_planner.git
cd conference_event_planner
npm install

# Start development
npm run dev
# Open http://localhost:5173
```

##  Tech Stack

- **Frontend**: React 18, Redux Toolkit
- **Build Tool**: Vite
- **Styling**: CSS3 with Grid/Flexbox
- **State Management**: Redux with createSlice pattern

##  Project Structure

```text
src/
├── App.jsx              # Root component
├── ConferenceEvent.jsx  # Main event interface
├── TotalCost.jsx        # Cost display
├── store.js             # Redux store
├── venueSlice.js        # Venue state management
├── mealsSlice.js        # Meals module (planned)
└── avSlice.js           # AV equipment (planned)
```

##  Development Status

### ✅ **Completed**
- Venue selection with quantity management
- Redux state architecture
- Responsive UI design
- Cost calculation engine

### 🔄 **Planned**
- Meals selection module
- AV equipment booking
- Enhanced cost breakdown
- Data persistence

---

##  About the Developer

**Rita Jindal** - Software Engieer  

*Passionate about building scalable, secure, and maintainable software solutions. Experienced in microservices architecture, cloud-native, and full-stack software development.*
