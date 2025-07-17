# 📱 Social Media Simulator (C++ Data Structures Project)

A console-based application demonstrating core social media features using efficient data structures.

[![C++](https://img.shields.io/badge/C++-17-blue?logo=c%2B%2B)](https://en.cppreference.com/)
[![Data Structures](https://img.shields.io/badge/Data_Structures-Linked%20Lists%20%2F%20Queues%20%2F%20Vectors-orange)]()

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

