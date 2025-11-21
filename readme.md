# Daily Wins

## Table of Contents
- [Overview](#overview)
- [Product Spec](#product-spec)
- [Wireframes](#wireframes)
- [Schema](#schema)

---

# Overview

## Description
Daily Wins is a simple, positive iOS journaling app where users log a “win” for the day—such as making their bed, going for a walk, or finishing an assignment. Each win includes a title, optional notes, optional photo, and an automatic timestamp. The app helps users build self-confidence, mindfulness, and positive habits through reflection and streaks.

## App Evaluation

**Category:**  
Productivity / Wellness / Journaling  

**Mobile:**  
Mobile-first experience; users quickly capture wins on the go. Uses notifications, camera/photo picker, and a fast, lightweight interface ideal for short daily interactions.

**Story:**  
People often overlook small accomplishments. Daily Wins gives users a space to acknowledge and celebrate small moments of progress, helping build motivation and a healthier mindset.

**Market:**  
Students, young adults, working professionals, or anyone looking to build positive habits or improve mental well-being.

**Habit:**  
Users log wins daily, often multiple times a day. Optional streaks and reminders encourage consistent use and habit formation.

**Scope:**  
- **V1:** Add, view, delete, and edit wins; persistent storage.  
- **V2:** Optional photo support, categories, and basic streak tracking.  
- **V3:** Analytics with charts, weekly summaries, shareable cards.  
- **V4:** Themes, widgets, and advanced journaling features.

---

# Product Spec

## 1. User Stories (Required and Optional)

### **Required Must-have Stories**
- [x] User can **create a win** with a title and optional notes.
- [x] User can **view a list/feed** of all wins.
- [x] User can **tap on a win** to view detailed information.
- [x] User can **edit an existing win**.
- [x] User can **delete a win**.
- [x] App **persists data locally** (Core Data or FileManager).
- [x] Clean, responsive SwiftUI-based UI.

### **Optional Nice-to-have Stories**
- [ ] User can add a **photo** to a win.
- [ ] User can track **streaks** (days with wins).
- [ ] User can see **weekly analytics** (wins per day, bar chart).
- [ ] User receives **daily reminders** to log a win.
- [ ] User can assign **categories/tags** to each win.
- [ ] User can share a **visual card** of the win.
- [ ] User can choose custom **themes** or color accents.
- [ ] App has a **widget** for quick win logging.
- [ ] App is protected with **FaceID/TouchID**.

---

## 2. Screen Archetypes

### **Home Feed Screen**
- Required: User can view a list of wins.
- Required: User can tap a win to navigate to detail view.
- Required: User can start creating a new win.

### **Add Win Screen**
- Required: User can create a new win (title & notes).
- Optional: Add a photo.
- Required: Save win to persistent storage.

### **Win Detail Screen**
- Required: User can view full details of a win.
- Required: User can delete a win.
- Required: User can navigate to edit a win.

### **Edit Win Screen**
- Required: User can modify and update win content.
- Required: User can save changes to persistent data.

### **Analytics Screen (Optional)**
- Optional: User can view streaks and weekly summaries.
- Optional: User can view charts showing wins over time.

### **Settings Screen (Optional)**
- Optional: User can enable/disable reminders.
- Optional: User can change themes or clear data.

---

## 3. Navigation

### **Tab Navigation (Tab to Screen)**
*(If implementing a tab bar)*  
- Home → Home Feed  
- Add → Add Win  
- Analytics → Optional Analytics Screen  
- Settings → Optional Settings Screen  

### **Flow Navigation (Screen to Screen)**

**Home Feed Screen**
- → Add Win Screen  
- → Win Detail Screen  

**Add Win Screen**
- → Home Feed (after saving)  

**Win Detail Screen**
- → Edit Win Screen  
- → Delete Win (returns to feed)  

**Edit Win Screen**
- → Win Detail Screen (after saving)  

**Optional Screens**
- Settings → Notification settings, theme options  
- Analytics → Chart views, streak info  

---

# Wireframes

Figma Wireframe(https://www.figma.com/make/Y5IrtsBkgeMqCjkXyFGO3M/Daily-Wins-iOS-Wireframe?node-id=0-4&t=d9GyR748JJycyBDD-1)

# Schema

### **Model: Win**
| Property      | Type       | Description                           |
|---------------|------------|---------------------------------------|
| id            | UUID       | Unique identifier for each win        |
| title         | String     | Main text describing the win          |
| notes         | String?    | Optional additional text              |
| imageData     | Data?      | Optional photo attached to the win    |
| timestamp     | Date       | Automatically saved date/time         |
| category      | String?    | Optional win category/tag             |

