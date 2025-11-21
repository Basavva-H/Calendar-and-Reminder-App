<div align="center">

# 📅 Calendar & Reminder Manager

### A Professional Desktop Application for Intelligent Task Management

![Version](https://img.shields.io/badge/Version-2.0.0-0066FF.svg)
![Python](https://img.shields.io/badge/Python-3.8%2B-0066FF.svg)
![License](https://img.shields.io/badge/License-MIT-0066FF.svg)
![Status](https://img.shields.io/badge/Status-Production%20Ready-10B981.svg)

[Features](#-key-features) • [Tech Stack](#-tech-stack) • [Installation](#-installation) • [Usage](#-usage) • [Screenshots](#-screenshots)

</div>

---

## 🎯 Overview

A modern, feature-rich desktop application built during my Python Development Internship at PinnacleLabs. Calendar & Reminder Manager combines elegant UI design with powerful reminder functionality to help users organize their daily tasks, manage events, and stay on top of their commitments.

The application features an intuitive calendar interface, intelligent notification system, and comprehensive task management capabilities with a professional, modern UI.

---

## ✨ Key Features

### 📅 Calendar Management
- **Interactive Monthly Calendar** with smooth navigation between months
- **Date Selection** - Click any date to view and manage reminders
- **Visual Indicators** - Today's date highlighted in yellow, selected dates in blue
- **Proper Grid Layout** - Professional calendar grid fitting with weekend highlighting

### ⏰ Smart Reminders
- **Complete CRUD Operations** - Create, Read, Update, Delete reminders with ease
- **Multiple Categories** - Work, Personal, Health, Shopping, General
- **Priority Levels** - Low, Normal, High, Urgent with color-coded indicators
- **Recurring Reminders** - Support for Daily, Weekly, and Monthly repetition
- **Time-Based Notifications** - Automatic alerts at scheduled reminder times

### 🔔 Intelligent Notifications
- **System Notifications** - Native OS notifications on Windows, macOS, Linux
- **Sound Alerts** - Customizable beep notifications when reminders trigger
- **Smart Scheduling** - Real-time reminder checking with configurable intervals
- **Background Monitoring** - Continuous reminder monitoring while app is running

### 🎨 Advanced Filtering & Search
- **Filter by Category** - Quickly view reminders by type
- **Filter by Priority** - See urgent tasks first
- **Search Functionality** - Find reminders by keywords
- **Date-Based Views** - Today's reminders, Overdue tasks, Upcoming events

### 📊 Dashboard & Analytics
- **Statistics Dashboard** - Real-time metrics on total, pending, completed, and overdue reminders
- **Today's View** - Quick access to today's scheduled tasks
- **Upcoming Reminders** - 7-day ahead planning view
- **Overdue Tracking** - Identify missed reminders at a glance

### 💾 Data Persistence
- **SQLite Database** - Reliable local data storage with automatic backups
- **Data Integrity** - Proper schema with timestamps and relationships
- **Efficient Queries** - Optimized database operations for fast access

### 🎭 Professional UI
- **Modern Design** - Clean, minimalist interface inspired by contemporary productivity apps
- **Tabbed Interface** - Dashboard, All Reminders, and Smart Filters tabs
- **Responsive Layout** - Sidebar calendar + content area with optimal spacing
- **Color-Coded** - Visual differentiation for categories and priorities
- **Smooth Interactions** - Intuitive controls with proper visual feedback

---

## 🛠️ Tech Stack

| Category | Technology |
|----------|-----------|
| **Language** | Python 3.8+ |
| **GUI Framework** | Tkinter |
| **Database** | SQLite |
| **Notifications** | System Native APIs |
| **Audio** | Windows winsound / OS Native |
| **Date/Time** | Python datetime, pytz |

---

## 📋 Requirements

\`\`\`
Python 3.8 or higher
Operating System: Windows, macOS, or Linux
RAM: 512 MB minimum
Disk Space: 50 MB
\`\`\`

---

## 🚀 Installation

### Step 1: Clone or Download the Project

\`\`\`bash
# Clone from GitHub
git clone https://github.com/yourusername/calendar-reminder-app.git
cd calendar-reminder-app

# Or extract the downloaded ZIP file
\`\`\`

### Step 2: Create Virtual Environment

\`\`\`bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
\`\`\`

### Step 3: Install Dependencies

\`\`\`bash
pip install -r requirements.txt
\`\`\`

### Step 4: Run Database Migration (First Time Only)

\`\`\`bash
python migrate_database.py
\`\`\`

Expected output:
\`\`\`
✓ Added 'is_recurring' column
✓ Added 'recurrence_type' column
✓ Database migration completed successfully!
\`\`\`

### Step 5: Launch the Application

\`\`\`bash
python main.py
\`\`\`

---

## 📖 Usage Guide

### Adding a Reminder

1. Click the **"+ Add Reminder"** button in the Reminders panel
2. Fill in the reminder details:
   - **Title** - Brief name for your reminder
   - **Description** - Detailed information
   - **Date** - Select reminder date (YYYY-MM-DD)
   - **Time** - Set reminder time (HH:MM)
   - **Category** - Choose from Work, Personal, Health, Shopping, General
   - **Priority** - Set importance level (Low, Normal, High, Urgent)
   - **Recurring** - Enable and select repetition pattern if needed
3. Click **"Save"** to add the reminder

### Selecting & Managing Reminders

1. **Select a Reminder** - Click on any reminder in the list (it will highlight)
2. **Edit** - Click the "Edit" button to modify details
3. **Delete** - Click "Delete" to remove the reminder (confirmation required)
4. **Mark Done** - Click "Mark Done" to complete a reminder

### Navigating the Calendar

- **Previous/Next Buttons** - Move between months
- **"Today" Button** - Jump to current month and date
- **Click Date** - Select a specific date to view its reminders
- **Color Indicators** - Yellow = today, Blue = selected date

### Using Filters

1. Go to the **"Smart Filters"** tab
2. **Quick Filters** - One-click access to predefined views:
   - Today's Reminders
   - Upcoming (7 days)
   - Overdue Tasks
3. **Advanced Filters** - Combine multiple criteria:
   - Category filter
   - Priority filter
   - Keyword search

### Dashboard Overview

The **Dashboard** tab shows:
- Today's scheduled reminders
- Reminders for the selected date
- Quick statistics (Total, Pending, Completed, Overdue)

---

## 🗂️ Project Structure

\`\`\`
calendar-reminder-app/
├── main.py                 # Application entry point
├── config.py               # Configuration & color palette
├── database.py             # Database operations & queries
├── gui.py                  # User interface (Tkinter)
├── reminders.py            # Reminder business logic
├── notifications.py        # Notification & alert system
├── migrate_database.py     # Database migration script
├── requirements.txt        # Python dependencies
├── README.md              # Project documentation
└── data/
    └── reminders.db       # SQLite database (auto-created)
\`\`\`

---

## 🎨 UI Design Features

### Color Palette
- **Primary**: #0066FF (Professional Blue)
- **Success**: #10B981 (Green)
- **Warning**: #F59E0B (Amber)
- **Danger**: #EF4444 (Red)
- **Background**: #FFFFFF (Clean White)

### Layout Highlights
- **Sidebar Calendar** - Quick date selection
- **Tabbed Content Area** - Organized information
- **Card-Based Components** - Modern visual hierarchy
- **Professional Typography** - Clear, readable fonts
- **Responsive Spacing** - Optimal padding and gaps

---

## 🔧 Advanced Features

### Recurring Reminders
- Set reminders to repeat daily, weekly, or monthly
- Automatic generation of future reminder instances
- Easy management of recurring series

### Notification System
- **Windows**: System notifications + winsound alerts
- **macOS**: Native notification center integration
- **Linux**: Notify-send integration
- **Custom Intervals**: Configurable checking frequency

### Database Operations
- Automatic PRAGMA optimizations
- Proper indexing on frequently queried columns
- Timestamp tracking (created_at, updated_at)
- Data integrity with proper constraints

### Statistics Tracking
- Real-time metrics updates
- Category-wise reminder count
- Priority-level distribution
- Completion rate monitoring

---

## 📸 Screenshots

### Main Dashboard
*Clean, organized interface with sidebar calendar and tabbed content*

### Reminder Management
*Easy-to-use dialog for creating and editing reminders*

### Smart Filters
*Advanced filtering and search capabilities*

### Calendar View
*Professional calendar grid with proper date highlighting*

---

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| **ModuleNotFoundError** | Run `pip install -r requirements.txt` |
| **Database Errors** | Delete `data/reminders.db` folder and restart app |
| **Notifications Not Working** | Check OS notification permissions in system settings |
| **UI Not Displaying** | Update tkinter: `pip install --upgrade tk` |
| **Date Issues** | Ensure date format is YYYY-MM-DD |

---

## 🚀 Future Enhancements

- [ ] Export reminders to CSV/PDF
- [ ] Cloud synchronization with Google Calendar
- [ ] Multiple user accounts with authentication
- [ ] Mobile app companion
- [ ] Email reminders
- [ ] Custom notification sounds
- [ ] Dark mode theme
- [ ] Reminder templates
- [ ] Integration with popular calendar apps
- [ ] Keyboard shortcuts

---

## 📝 Database Schema

### Reminders Table

\`\`\`sql
CREATE TABLE reminders (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    title TEXT NOT NULL,
    description TEXT,
    date TEXT NOT NULL,
    time TEXT NOT NULL,
    category TEXT DEFAULT 'General',
    priority TEXT DEFAULT 'Normal',
    is_completed INTEGER DEFAULT 0,
    is_recurring INTEGER DEFAULT 0,
    recurrence_type TEXT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
\`\`\`

---

## 💡 Learning Outcomes

This project demonstrates:
- **GUI Development** - Professional desktop application with Tkinter
- **Database Design** - SQLite schema design and optimization
- **User Experience** - Intuitive interface design principles
- **System Integration** - Working with OS notifications and alerts
- **Code Organization** - Modular, maintainable code structure
- **Error Handling** - Robust exception management
- **Software Architecture** - MVC-inspired separation of concerns

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

---

## 📄 License

This project is open source and available under the MIT License. See `LICENSE` file for details.

---

## 👨‍💼 Author

**Developed during Python Development Internship at PinnacleLabs**

---

## 🙏 Acknowledgments

Special thanks to:
- **PinnacleLabs** - For the internship opportunity and mentorship
- **Python Community** - For excellent documentation and resources
- **Tkinter Documentation** - For GUI framework reference
- **SQLite** - For reliable database solution

---

## 📞 Contact & Support

For questions, suggestions, or support:
- **LinkedIn**: [Your LinkedIn Profile]
- **Email**: [Your Email]
- **GitHub**: [Your GitHub Profile]

---

<div align="center">

**Made with ❤️ during my internship at PinnacleLabs**

⭐ If you found this project helpful, please consider giving it a star! ⭐

</div>
\`\`\`

Now create additional documentation files:
