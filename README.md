# Bug Tracker Application (Next.js)

## Overview
This is a simple Bug Tracker web application built using **Next.js** and **React.js**. It supports user authentication with two roles: Developer and Manager. Developers can create, edit, and track tasks/bugs, including starting and stopping time trackers on each task. Managers can view all tasks, approve or re-open bugs pending verification, and monitor developer activity.

-----------------------------------------------------------------------------------------

## Features
- **User Authentication (Mock):** Hardcoded users with Developer and Manager roles.
- **Role-Based Dashboard:**
  - Developers see their tasks and can manage them.
  - Managers see all tasks and can approve or re-open bugs.
- **Task Management:**
  - Create, edit, delete tasks.
  - Set task fields: Title, Description, Priority, Status, Assignee, Dates.
  - Filter and sort tasks by priority and status.
- **Task Status Workflow:**
  - Developers can close bugs, which then await manager approval.
  - Managers can approve closure or re-open bugs.
- **Time Tracking:**
  - Developers can start and stop timers per task.
  - Time spent is logged and displayed.
  - Managers can view aggregated time spent by all developers.
- **Responsive UI:** Works on desktop and mobile.
- **State Management:** React Context API used for tasks and timers.

-----------------------------------------------------------------------------------------

## Assumptions & Hardcoded Values
- **User Authentication:**
  - Mocked with hardcoded users inside the frontend (no backend authentication).
  - Example credentials:
    - Developer:  
      - Username: `dev1`  
      - Password: `devpass`  
    - Manager:  
      - Username: `manager1`  
      - Password: `managerpass`
- **Data Persistence:**
  - Data is stored in React state and context only; no database or backend persistence.
  - Refreshing the page resets all data.
- **Task IDs:**
  - Tasks are assigned incremental or UUIDs in the frontend for identification.
- **Time Tracking:**
  - Time logs are stored in memory and displayed; no detailed analytics or export.
- **Status Workflow:**
  - Task statuses include: Open, Pending Approval, Closed, etc.
- **UI/UX:**
  - Simple and clean UI using CSS modules or global CSS.
  - Basic responsiveness; no advanced animations or transitions.

-----------------------------------------------------------------------------------------

## Setup Instructions

### Prerequisites
- Node.js (v16 or higher recommended)
- npm (comes with Node.js) or yarn

### Installation Steps

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd bug_tracker_nextjs_full
   npm install/yarn install
   npm run dev

   Live URL: https://bug-tracker-seven-rho.vercel.app/
