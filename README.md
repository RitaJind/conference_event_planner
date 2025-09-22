# Conference Event Planner

A modern React-based web application for planning and managing conference events. This application provides an intuitive interface for selecting venues, calculating costs, and managing event logistics.

## 🚀 Features

- **Venue Selection**: Choose from multiple venue options including Auditorium Hall, Presentation Room, Large Meeting Room, and Small Meeting Room
- **Real-time Cost Calculation**: Dynamic cost updates as you modify your selections
- **Redux State Management**: Centralized state management for scalable application architecture
- **Responsive Design**: Mobile-first design that works on all device sizes
- **Interactive UI**: Smooth animations and transitions for enhanced user experience
- **Quantity Management**: Add/remove venue bookings with intelligent business rules

## 🛠️ Tech Stack

- **Frontend**: React 18, JSX
- **State Management**: Redux Toolkit
- **Build Tool**: Vite
- **Styling**: CSS3 with modern features (Grid, Flexbox, Custom Properties)
- **Package Manager**: npm

## 📦 Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/RitaJind/conference_event_planner.git
   cd conference_event_planner
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Start the development server**

   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173` (or the port shown in your terminal)

## 🏗️ Project Structure

```text
conference_event_planner/
├── public/
│   ├── AUdi.png
│   ├── bgevent.png
│   └── conference.png
├── src/
│   ├── assets/
│   │   └── react.svg
│   ├── App.jsx                 # Main application component
│   ├── App.css                 # Global styles
│   ├── main.jsx                # Application entry point
│   ├── index.css               # Base styles
│   ├── ConferenceEvent.jsx     # Main event planning component
│   ├── ConferenceEvent.css     # Event planner styles
│   ├── TotalCost.jsx           # Cost calculation component
│   ├── TotalCost.css           # Cost component styles
│   ├── AboutUs.jsx             # About page component
│   ├── store.js                # Redux store configuration
│   ├── venueSlice.js           # Venue state management
│   ├── mealsSlice.js           # Meals state management (placeholder)
│   └── avSlice.js              # AV equipment state management (placeholder)
├── index.html
├── package.json
├── vite.config.js
└── README.md
```

## 🎯 Usage

1. **Landing Page**: Start by clicking "Get Started" on the welcome screen
2. **Venue Selection**: Browse available venues and adjust quantities using +/- buttons
3. **Cost Tracking**: View real-time cost updates as you make selections
4. **Summary View**: Toggle between selection and cost summary views

### Business Rules

- **Auditorium Hall**: Maximum 3 bookings allowed
- **Other Venues**: Maximum 10 bookings per venue type
- **Cost Calculation**: Automatic total calculation based on venue selections

## 🚧 Development Status

### ✅ Completed Features

- Venue selection and management
- Redux store setup and venue slice
- Responsive UI design
- Basic navigation system

### 🔄 In Progress

- Meals selection functionality
- AV equipment management
- Complete cost breakdown display

### 📋 Planned Features

- Event scheduling
- Additional venue types
- Export/print functionality
- User authentication
- Event templates

## 🎨 Design Principles

- **Mobile-First**: Responsive design that prioritizes mobile experience
- **User-Centric**: Intuitive interface with clear visual feedback
- **Performance**: Optimized with Vite for fast development and builds
- **Scalability**: Modular Redux architecture for easy feature additions

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint (if configured)

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Author

**Rita Jindal** - [RitaJind](https://github.com/RitaJind)

## 🙏 Acknowledgments

- React team for the amazing framework
- Redux Toolkit for simplified state management
- Vite for the lightning-fast build tool

---

Built with ❤️ for efficient conference event planning
