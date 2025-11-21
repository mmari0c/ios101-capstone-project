# Daily Wins – iOS App

Daily Wins is a simple, uplifting iOS app designed to help users acknowledge small accomplishments throughout their day. Users can log a “win,” add optional notes or photos, track their weekly progress, and build positive habits over time.

---

## App Overview

### **Description**
Daily Wins gives users a dedicated space to celebrate small positive moments such as making their bed, going for a walk, or finishing an assignment. Each win is logged with a title, timestamp, optional notes, and optional image. Over time, users can review their wins, see summaries, and maintain streaks.

### **Evaluation**
Daily Wins is:
- **Mobile-first**: Designed for quick capture of accomplishments throughout the day.
- **Habit-forming**: Encourages consistent use through streaks and reminders.
- **Positive & simple**: Focuses on improving mental well-being and self-confidence.

---

## App Features

### **Required Features (MVP)**
- [x] User can **create a win** with:
  - Title (required)
  - Optional notes
  - Auto-generated timestamp
- [x] User can **view a list/feed** of all wins in reverse chronological order.
- [x] User can **view details** of a single win.
- [x] User can **edit an existing win**.
- [x] User can **delete a win**.
- [x] Data persists locally (Core Data or FileManager + JSON).
- [x] App UI built using SwiftUI navigation and components.
- [x] Clean, responsive layout with light/dark mode.

---

### **Optional Features**
- [ ] Add an **image** to each win using SwiftUI's PhotosPicker.
- [ ] **Streak counter** (days with logged wins).
- [ ] **Weekly summary view** showing number of wins per day.
- [ ] **Analytics tab** using Swift Charts:
  - Wins per week/month
  - Line or bar graph of activity
- [ ] **Categories/tags** for wins (e.g., “School,” “Health,” “Mindset”).
- [ ] **Local notifications** reminding users to log a win.
- [ ] **Shareable “win card”** image for social media.
- [ ] App themes or custom accent colors.
- [ ] Home screen widget to quickly add a win.
- [ ] FaceID/TouchID lock for privacy.

---

## App Screens

### **1. Home Feed Screen**
- Shows a scrollable list of all wins.
- Each card includes:
  - Title
  - Short description preview
  - Timestamp
  - Optional thumbnail image
- Floating “+” button to add a new win.

### **2. Add Win Screen**
- Input fields for:
  - Title
  - Notes (optional)
  - Photo picker (optional)
- “Save” button to persist the new win.

### **3. Win Detail Screen**
- Full view of a single win:
  - Title
  - Notes
  - Larger image (if provided)
  - Timestamp
- Buttons for:
  - Edit
  - Delete

### **4. Edit Win Screen**
- Same UI as Add Win screen, pre-filled with current data.
- “Update” button saves changes.

### **5. Analytics Screen (Optional)**
- Charts for:
  - Wins per day/week
  - Activity streak
- Motivational stats or emojis.

### **6. Settings Screen (Optional)**
- Notification toggle
- Theme/color selection
- Clear data option
- About page

---


Optional screens (Analytics, Settings) branch from a tab bar or menu depending on design.

---

## App Spec

### **User Features**
- Log a daily accomplishment (“win”).
- Add details or photos to personalize entries.
- View all logged wins in a simple feed.
- Tap on a win to view full details.
- Edit or delete existing wins.
- Maintain local history of wins.
- (Optional) Track streaks and weekly progress.
- (Optional) View charts of activity trends.
- (Optional) Receive daily reminders.

---

### **Screens & Functionality**

#### **Home Feed**
- Displays all wins
- Access to Add Win
- Navigation to Win Detail

#### **Add Win**
- Title, notes, optional image
- Save and return to feed

#### **Win Detail**
- Full view of a win
- Edit and delete buttons

#### **Edit Win**
- Update data of an existing win

#### **Analytics (Optional)**
- Charts and weekly stats
- Streak visualization

#### **Settings (Optional)**
- App preferences
- About section
- Notifications toggle
