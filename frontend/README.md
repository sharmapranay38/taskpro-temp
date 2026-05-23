# Task Pro - Team Task Manager

A modern, professional task management application built with React and Vite. Organize, prioritize, and execute tasks with a beautiful glass-morphism UI and powerful workflow features.

![Task Pro](https://img.shields.io/badge/version-1.0.0-blue.svg)
![React](https://img.shields.io/badge/React-19.0.0-61DAFB?logo=react)
![Vite](https://img.shields.io/badge/Vite-6.4.2-646CFF?logo=vite)

---

## ✨ Features

### Core Task Management
- **Create & Manage Tasks** - Add tasks with title, description, due date, and priority level
- **Priority System** - Organize tasks by High, Medium, and Low priority levels
- **Status Tracking** - Track task progress with Todo, In Progress, and Done statuses
- **Task Details** - View and edit comprehensive task information
- **Bulk Operations** - Create, update, and delete tasks efficiently

### Smart Filtering & Search
- **Priority Filter** - Filter tasks by High, Medium, or Low priority
- **Status Filter** - View tasks by their current status (Todo, In Progress, Done)
- **Search Capability** - Full-text search across all tasks
- **Pagination** - Navigate through tasks with efficient pagination (10 tasks per page)
- **Combined Filters** - Use multiple filters simultaneously for powerful task queries

### Analytics & Insights
- **Task Statistics** - Real-time dashboard with key metrics:
  - Total tasks overview
  - Priority distribution breakdown
  - Status distribution (Todo, In Progress, Done)
  - Overdue task alerts
- **Visual Analytics** - Display statistics in beautiful stat cards

### Workflow Intelligence
- **Overdue Tracking** - Automatic identification and visual highlighting of overdue tasks
- **Task State Management** - Enforce logical workflow transitions
- **Real-time Updates** - Dashboard updates instantly on task changes

### Authentication & Security
- **User Registration** - Create new user accounts
- **Secure Login** - JWT-based authentication
- **Session Management** - Persistent login with localStorage
- **Token-based API Security** - All API requests secured with Bearer tokens

### Admin Capabilities
- **Admin Dashboard** - Switch to admin view to manage all system tasks
- **User Management** - Admin can create new user accounts
- **System Overview** - View complete task ecosystem as an administrator
- **Admin Panel** - Dedicated interface for user creation and system management

### User Experience
- **Modern UI Design** - Glass-morphism effects with professional aesthetics
- **Responsive Layout** - Fully responsive design (mobile, tablet, desktop)
- **Smooth Animations** - Elegant transitions and hover effects
- **Color-coded UI** - Indigo/purple accent color system for visual hierarchy
- **Clean Dashboard** - Organized layout with intuitive navigation
- **Error Handling** - Clear error messages and user feedback

---

## 🚀 Getting Started

### Prerequisites
- **Node.js** (v14 or higher)
- **npm** or **yarn** package manager

### Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd Team-Task-Manager/frontend
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up environment variables** (optional):
   Create a `.env` file in the project root:
   ```
   VITE_API_URL=http://localhost:5000
   ```
   If not set, defaults to `http://localhost:5000`

4. **Start the development server:**
   ```bash
   npm run dev
   ```
   The app will be available at `http://localhost:5174/` (or the next available port)

---

## 📖 Usage Guide

### Authentication

**Register a New Account:**
1. Click the "Register" tab on the login page
2. Enter your name, email, and password
3. Click "Create account"
4. You'll be automatically logged in

**Login:**
1. Enter your email and password
2. Click "Sign in"
3. Your session will be saved in browser storage

**Logout:**
- Click the "Logout" button in the dashboard to end your session

### Managing Tasks

**Create a Task:**
1. In the dashboard, fill out the task form:
   - **Title** - Task name (required)
   - **Description** - Task details
   - **Due Date** - When the task is due
   - **Priority** - High, Medium, or Low
2. Click "Add task" button
3. Task appears in your task list

**Update a Task:**
1. Find the task in the list
2. Change the status or priority using dropdown menus
3. Click "Save" to confirm changes
4. Edits are saved immediately

**Delete a Task:**
1. Click the trash icon on any task
2. Task is removed from your list
3. Cannot be undone

**View Task Details:**
- Hover over any task card to see all information
- Check the due date and priority indicators
- Red left border indicates overdue tasks

### Using Filters & Search

**Filter by Priority:**
1. Use the Priority dropdown in the filter bar
2. Select: All, High, Medium, or Low
3. Task list updates instantly

**Filter by Status:**
1. Use the Status dropdown in the filter bar
2. Select: All, Todo, In Progress, or Done
3. View only tasks in that status

**Search Tasks:**
1. Type in the search box
2. Results filter in real-time
3. Search works across task titles and descriptions

**Combine Multiple Filters:**
- Use Priority + Status + Search together
- Reset filters by clicking "Reset filters" button
- Use pagination to navigate results

### Dashboard Analytics

**View Statistics:**
- **Top stat card** - Total number of tasks
- **Distribution cards** - Priority breakdown (High, Medium, Low)
- **Status cards** - How many tasks in each status
- **Overdue alert** - Number of tasks past their due date

**Use Analytics to:**
- Identify workload distribution
- Spot priority imbalances
- Track completion progress
- Catch overdue tasks

### Admin Features

**Switch to Admin View** (if you have admin role):
1. Dashboard has an "Admin" toggle button
2. Click to view all system tasks
3. See complete task overview across all users
4. Switch back to personal view anytime

**Create Admin Users** (admin only):
1. In admin panel, fill the "Create user" form
2. Enter: Name, Email, Password
3. Click "Create" to add new user account
4. New user can immediately login

---

## 🏗️ Tech Stack

**Frontend:**
- **React 19.0.0** - UI component framework
- **Vite 6.4.2** - Fast build tool and dev server
- **Vanilla CSS** - Modern CSS with variables and glass-morphism effects
- **Google Fonts** - Inter & Poppins typography

**Architecture:**
- Component-based React application
- State management with React hooks (useState, useEffect, useMemo)
- REST API integration via fetch
- Local storage for session persistence
- JWT authentication with Bearer tokens

**Design System:**
- CSS Variables for theming
- Glass-morphism UI patterns
- Responsive breakpoints (mobile: 640px, tablet: 960px, desktop: 1200px+)
- Smooth transitions (0.25s ease) and hover effects
- Indigo/Purple color palette (#6366f1 primary)

---

## 📁 Project Structure

```
frontend/
├── src/
│   ├── App.jsx           # Main application component
│   ├── api.js            # API integration layer
│   ├── main.jsx          # React entry point
│   └── styles.css        # Complete styling (glass-morphism)
├── index.html            # HTML entry point
├── package.json          # Project dependencies
├── vite.config.js        # Vite configuration
└── README.md            # This file
```

---

## 🎨 Design Features

- **Modern Glass-Morphism** - Frosted glass effect panels with blur backdrop filter
- **Responsive Grid Layout** - 2-column hero, adaptive dashboard cards
- **Smooth Interactions** - Card hover animations, button transforms
- **Color-Coded Priorities** - Visual indicators for task importance
- **Overdue Indicators** - Red left border on past-due tasks
- **Professional Typography** - Poppins for headings, Inter for body text
- **Gradient Text** - Hero headline with blue-to-purple gradient
- **Focus States** - Blue glow effect on form inputs when active

---

## 🔧 Development

**Available npm Scripts:**

```bash
# Start development server (hot reload enabled)
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

**Development Features:**
- Hot Module Replacement (HMR) - Changes reflect instantly
- Fast refresh - Component state preserved during edits
- Source maps for debugging
- PostCSS compilation for CSS compatibility

---

## 🌐 API Integration

The app connects to a backend API (default: `http://localhost:5000`). 

**API Endpoints:**
- `POST /auth/register` - User registration
- `POST /auth/login` - User login
- `POST /auth/admin-users` - Create admin user (admin only)
- `GET /tasks` - Fetch user's tasks with filters
- `GET /tasks/all` - Fetch all tasks (admin only)
- `POST /tasks` - Create new task
- `PUT /tasks/:id` - Update existing task
- `DELETE /tasks/:id` - Delete task
- `GET /stats` - Get user statistics

All requests include JWT token in Authorization header.

---

## 📝 Notes

- Tasks are stored on the backend server
- Sessions persist in browser localStorage (survives page refresh)
- Clearing browser data will require re-login
- Overdue tasks are determined by comparing due date to current date
- Admin view shows all system tasks regardless of owner
- Pagination shows 10 tasks per page

---

## 🐛 Troubleshooting

**App shows login screen after refresh:**
- Clear browser storage: Settings → Privacy & Security → Clear browsing data
- Or use console: `localStorage.clear(); location.reload();`

**Cannot connect to API:**
- Ensure backend server is running on `http://localhost:5000`
- Check VITE_API_URL environment variable

**Styles not updating:**
- Vite should auto-refresh, but hard refresh browser: Ctrl+Shift+R
- Or rebuild: `npm run dev`

---

## 📄 License

This project is part of the Team Task Manager application.

---

## 👨‍💻 Support

For issues or feature requests, please contact the development team.

---

**Built with ❤️ using React + Vite**
