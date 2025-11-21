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


