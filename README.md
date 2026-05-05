# ⚡ Smart Grid Electricity Distribution System (Graph - C)

## 👥 Team Members
- Student 1 T.sandeep kumar
- Student 2 B.siva

---

## 📌 Problem Statement
The project aims to design a Smart Grid Electricity Distribution System using a graph data structure.  
It simulates how electricity flows from power stations to consumers through interconnected nodes and transmission lines.

---

## 🌍 Real-World Application
- Power grid management systems  
- Electricity distribution networks  
- Load balancing between substations  
- Infrastructure planning  

---

## 🧠 Data Structure Used
**Graph (Adjacency List - Dynamic Implementation)**

- **Nodes (Vertices):**
  - Power Stations
  - Substations
  - Consumers  

- **Edges:**
  - Transmission lines with capacity  

---

## ⚙️ Features (CRUD Operations)

### ✅ Create
- Add Node (Station/Consumer)
- Add Connection (Edge)

### 📖 Read
- Display entire grid
- Search node

### 🔄 Update
- Update node details
- Update connection capacity

### ❌ Delete
- Delete node
- Delete connection

---

## 🧮 Algorithm Overview

### Add Node
1. Take node ID and name  
2. Allocate memory using `malloc`  
3. Insert node into linked list  

### Add Edge
1. Find source and destination nodes  
2. Create edge  
3. Link edge to source node  

### Delete Node
1. Remove all edges of the node  
2. Remove edges pointing to the node  
3. Free memory  

---

## 🏗️ System Design

The system is modeled as a graph:

[Power Station] --->[Substation] ---> [Consumers]

Each node connects to others through edges representing transmission lines.

---

## 💻 Technologies Used
- Programming Language: **C**
- Concepts:
  - Structures (`struct`)
  - Dynamic Memory Allocation (`malloc`, `free`)
  - Linked Lists
  - Graphs

---

## ▶️ Compilation & Execution

```bash
gcc main.c -o grid
./grid

```
## 📊Sample Output

```bash

1.Add Node
2.Add Edge
3.Display
4.Search
5.Update Node
6.Update Edge
7.Delete Node
8.Delete Edge
9.Exit

Enter choice: 1
Enter Node ID: 1
Enter Node Name: PowerStation
Node added.

Enter choice: 2
Enter Source ID: 1
Enter Destination ID: 2
Enter Capacity: 100
Connection added.

Display:
1 (PowerStation) -> 2 (Substation) [Cap:100]

```
