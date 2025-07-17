# 📱 Mini Instagram (C++ Data Structures Project)

A console-based application demonstrating core social media features using efficient data structures.

[![C++](https://img.shields.io/badge/C++-17-blue?logo=c%2B%2B)](https://en.cppreference.com/)
[![Data Structures](https://img.shields.io/badge/Data_Structures-Linked%20Lists%20%2F%20Queues%20%2F%20Vectors-orange)]()

## 🎥 Project Demo
<div align="center">
  <img src="./screenshots/1.jpg" width="30%" alt="Main Menu">
  <img src="./screenshots/2.jpg" width="30%" alt="User Registration"> 
  <img src="./screenshots/3.jpg" width="30%" alt="Post Creation"><br>
  <img src="./screenshots/4.jpg" width="30%" alt="Friend System">
  <img src="./screenshots/5.jpg" width="30%" alt="Messaging">
  <img src="./screenshots/6.jpg" width="30%" alt="Notifications">
</div>

## ✨ Core Features
### 🧑 User System
- Registration with username/password
- Profile management (city, friends list)
- Secure login authentication

### 📝 Content Management
- Post creation (Linked List implementation)
- Message system (Linked List)
- Friend request queue (FIFO processing)

### 🔔 Notification System
- Real-time activity alerts
- Queue-based notification delivery

## 🛠️ Implementation Highlights
```cpp
// Memory-efficient linked list for posts
struct Post {
    string content;
    Post* next;  // O(1) insertion
};

// Friend request queue
struct FriendRequest {
    string requester;
    FriendRequest* next;  // FIFO processing
};

// O(1) notification insertion
void addNotification(string msg) {
    Notification* newNotif = new Notification(msg, notificationQueue);
    notificationQueue = newNotif;
}

