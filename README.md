# 🎯 Conference Event Planner

A **production-ready React application** built with modern web technologies for comprehensive conference event planning and management. This application demonstrates enterprise-grade frontend architecture, state management patterns, and responsive design principles.

![React](https://img.shields.io/badge/React-18+-blue.svg)
![Redux](https://img.shields.io/badge/Redux_Toolkit-Latest-purple.svg)
![Vite](https://img.shields.io/badge/Vite-4+-yellow.svg)
![CSS3](https://img.shields.io/badge/CSS3-Modern-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## 🚀 Project Overview

This web application implements a **comprehensive event planning system** with real-time cost calculation, venue management, and interactive user experience. Built following **React best practices** and **modern frontend architecture patterns**, it's designed for scalable event management workflows.

### 🏗️ **Architecture Highlights**

- **Component-Based Architecture** - Modular, reusable React components
- **State Management Excellence** - Redux Toolkit with optimized slice patterns
- **Modern Build System** - Vite for lightning-fast development and builds
- **Responsive Design** - Mobile-first CSS with Grid and Flexbox layouts
- **Business Logic Integration** - Smart quantity limits and cost calculations
- **Performance Optimized** - Code splitting and efficient re-renders

## 📋 Features

### 🏢 **Venue Management**

- ✅ **Multi-Venue Selection** - Auditorium Hall, Presentation Room, Meeting Rooms
- ✅ **Smart Quantity Control** - Intelligent booking limits per venue type
- ✅ **Real-time Cost Calculation** - Dynamic pricing updates with user interactions
- ✅ **Business Rules Enforcement** - Auditorium Hall (max 3), Others (max 10)
- ✅ **Visual Feedback** - Interactive +/- controls with immediate UI updates

### 🛠️ **Technical Features**

- ✅ **Redux State Management** - Centralized store with slice-based architecture
- ✅ **Responsive UI/UX** - Mobile-first design with smooth animations
- ✅ **Component Modularity** - Reusable components with clear separation of concerns
- ✅ **Navigation System** - Hash-based routing with smooth scrolling
- ✅ **Future-Ready Architecture** - Extensible structure for meals and AV equipment
- ✅ **Modern CSS** - Custom properties, Grid, Flexbox, and media queries

## 🏃‍♂️ Quick Start

### **Prerequisites**

- Node.js 18+
- npm or yarn package manager
- Modern web browser

### **Option 1: Local Development**

```bash
# Clone the repository
git clone https://github.com/RitaJind/conference_event_planner.git
cd conference_event_planner

# Install dependencies
npm install

# Start development server
npm run dev

# Open browser
# Navigate to http://localhost:5173
```

## 🎯 Application Workflow

### **User Journey**

1. **Landing Page** - Welcome screen with professional event planning introduction
2. **Venue Selection** - Interactive venue cards with quantity controls
3. **Cost Calculation** - Real-time pricing updates with business rule validation
4. **Summary View** - Toggle between selection interface and cost breakdown
5. **Future Extensions** - Meals and AV equipment modules (in development)

### **Business Logic**

- **Auditorium Hall**: Premium venue, maximum 3 bookings per event
- **Meeting Rooms**: Standard venues, maximum 10 bookings per type
- **Cost Engine**: Dynamic calculation with immediate UI feedback
- **State Persistence**: Redux store maintains selections across views

## 🏗️ Architecture & Design Patterns

### **Project Structure**

```text
src/
├── main.jsx              # Application entry point & React DOM rendering
├── App.jsx               # Root component with landing page logic
├── App.css               # Global application styles
├── index.css             # Base CSS reset and typography
├── store.js              # Redux store configuration
├── components/           # Feature components
│   ├── ConferenceEvent.jsx    # Main event planning interface
│   ├── ConferenceEvent.css    # Event planner styling
│   ├── TotalCost.jsx          # Cost calculation display
│   ├── TotalCost.css          # Cost component styling
│   └── AboutUs.jsx            # About page component
├── store/                # Redux state management
│   ├── venueSlice.js          # Venue selection logic
│   ├── mealsSlice.js          # Meals management (future)
│   └── avSlice.js             # AV equipment (future)
└── assets/               # Static resources
    └── react.svg
```

### **State Management Architecture**

```javascript
// Redux Toolkit Slice Pattern
const venueSlice = createSlice({
  name: 'venue',
  initialState: venueData,
  reducers: {
    incrementQuantity: (state, action) => {
      // Immutable state updates with Immer
      const venue = state[action.payload];
      if (venue.name === "Auditorium Hall" && venue.quantity < 3) {
        venue.quantity += 1;
      } else if (venue.name !== "Auditorium Hall" && venue.quantity < 10) {
        venue.quantity += 1;
      }
    }
  }
});
```

## 🚧 Development Status & Roadmap

### **✅ Completed Features**

- **Core Venue Management** - Full CRUD operations with Redux integration
- **Responsive UI Framework** - Mobile-first design with CSS Grid/Flexbox
- **State Architecture** - Redux Toolkit store with optimized slice patterns
- **Business Logic Engine** - Quantity limits and cost calculation algorithms
- **Component Library** - Reusable UI components with consistent styling

### **🔄 In Progress**

- **Meals Management Module** - Food service selection with dietary preferences
- **AV Equipment System** - Audio/visual equipment booking and management
- **Enhanced Cost Display** - Detailed breakdown with tax calculations
- **Data Persistence** - Local storage integration for session management

### **📋 Planned Features**

- **Event Scheduling** - Calendar integration with time slot management
- **User Authentication** - Multi-user support with role-based access
- **Export Functionality** - PDF generation and email notifications
- **Payment Integration** - Stripe/PayPal integration for booking confirmation
- **Admin Dashboard** - Analytics and venue utilization reporting
- **Mobile App** - React Native companion application

---

## 👨‍💻 About the Senior Software Engineer

**Rita Jindal** - Full Stack Developer  

*Passionate about building scalable, secure, and maintainable software solutions. Experienced in microservices architecture, cloud-native development, and full-stack web applications.*
