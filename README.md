# IranGard

**Collaborative trip-planning web app for travel in Iran.**
Team project for the *System Analysis and Design* course, K. N. Toosi University of Technology (Fall 2025). Originally developed on the university's GitLab; full commit history is preserved here.

**Stack:** FastAPI · SQLAlchemy · Alembic · PostgreSQL · Vite (vanilla JS) · Docker Compose · Nginx (HTTPS) · LLM integration (Groq)

## Team
| Member | Main contributions |
|---|---|
| **Ali Abbasi** ([@Abbasi8312](https://github.com/Abbasi8312)) | Backend lead (trips, trip plans, places, auth APIs; CRUD and schemas), LLM-based review summarization, Docker/Nginx deployment, branch integration |
| Yasamin Riahi ([@YasaminRiahi](https://github.com/YasaminRiahi)) | |
| Kimia Sadeghi ([@Kimiass](https://github.com/Kimiass)) | |
| Mohammadreza Abedin ([@MrAbedam](https://github.com/MrAbedam)) | |

## Running locally
```bash
cp .env.example .env   # fill in DB credentials and your own GROQ_API_KEY
docker compose up --build
```

---

**Project Description:**  
IranGard is a comprehensive web application designed to help users plan their trips around Iran. The platform provides social, interactive, and organized trip planning features, allowing users to explore, share, and manage travel experiences efficiently.

---

## Features

### **User Account and Registration**
- Users can **register and log in** to their account.
- During registration, users provide:
  - Name
  - Preferred categories of places (e.g., religious, nature, cultural)
  - Other optional information

### **Friend Requests**
- Users can send **friend requests** to others using their IDs.
- Each user has a **request section** showing:
  - Sent requests
  - Received requests
- Requests remain until accepted or rejected.
- Accepted requests add users as **friends**.

### **Trip Creation**
- Users can **create trips** and send invitations to friends.
- A **trip request system** handles invitations.
- Based on the selected city, a list of places is suggested:
  - Matching the user’s preferred categories
  - Including photos, location, reviews, and descriptions
- Users can select places and **vote** on them within the group.

### **Pre-made Travel Packages**
- Pre-assembled sets of places for specific trips are available.
- These packages can also be **voted on** by participants.

### **Expense Tracking**
- During trips, users can log expenses with details:
  - Category (food, tickets, etc.)
  - Who paid
  - Share per person

### **Reviews and Feedback**
- Users can leave **reviews and ratings** for places visited.
- Trips can be **marked as completed** when finished.

### **My Trips**
- Each user has a **My Trips** section:
  - Current trips
  - Past trips (stored for up to 1 year)

### **Wishlist**
- Users can maintain a **wishlist** of places they want to visit.

### **Social Interaction**
- Users can:
  - Like places
  - Comment on places
  - Vote on trip plans

---

## Future Enhancements
- Enhanced recommendation system based on travel patterns
- Integration with maps and navigation services
- Real-time chat for trip participants

---


This project aims to create a **fun, interactive, and organized travel experience** for users exploring Iran.
