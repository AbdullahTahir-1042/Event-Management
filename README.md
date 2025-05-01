# 📅 Event Scheduling System (C++)

A robust, console-based **Event Scheduling System** implemented in C++. This project utilizes a Binary Search Tree (BST) to efficiently manage events based on their start time and provides key scheduling features such as conflict detection and free slot calculation.

---

## 🚀 Features

- ✅ **Add Event** — Add a new event with ID, name, start time, and duration.
- ❌ **Delete Event** — Remove an event using its unique ID.
- 🔍 **Detect Overlaps** — Check if a given time window overlaps with any existing event.
- ⏰ **Calculate Free Time Slots** — Identify available time intervals for a specific day.
- 📋 **View Full Schedule** — Display all scheduled events in sorted (chronological) order.

---

## 🧠 Data Structure

Events are stored in a **Binary Search Tree (BST)** ordered by `startDateTime` (`YYYY-MM-DD HH:MM` format). This allows for efficient insertion, traversal, and conflict resolution.

### Event Node Structure:
    ```cpp
        struct Event {
              int id;
              string name;
              string startDateTime;
              int duration;
              Event *left;
              Event *right;
          };

# 🛠️ How to Compile and Run

* Prerequisites
    A C++ compiler like g++.
  
* Clone or download the repository.

* Use the following commands to compile and run it.
  
        g++ -o scheduler scheduler.cpp
        ./scheduler
  
