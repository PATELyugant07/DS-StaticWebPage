# Treap (Tree + Heap) - Interactive Static Webpage

<p align="center">
  <img src="https://img.shields.io/badge/Treap-Tree%20%2B%20Heap-blue?style=for-the-badge" alt="Treap Badge">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License">
  <img src="https://img.shields.io/badge/Static%20Webpage-HTML%2FCSS%2FJS-orange?style=for-the-badge" alt="Static Webpage">
</p>

---

## 🌟 Overview

Welcome to the **Treap (Tree + Heap)** interactive visualization project! This static webpage provides an engaging and interactive way to learn and understand the Treap data structure through stunning animations and step-by-step explanations.

### What is a Treap?

A **Treap** is a binary search tree (BST) that is also a heap. It combines the properties of both:
- **Binary Search Tree (BST)**: Left child < Root < Right child (by key)
- **Heap**: Parent has higher priority than children (by priority)

This elegant data structure provides **O(log n)** expected time complexity for search, insert, and delete operations while maintaining balance through randomization.

---

## 🎬 Animations

This project includes interactive animations to visualize Treap operations:

### 1. **Insert Animation**
- Shows new node falling into position
- Demonstrates heap property restoration through rotations
- Highlights priority comparisons

### 2. **Delete Animation**
- Visualizes node removal process
- Shows merge/bubble-down operations
- Demonstrates heap property maintenance

### 3. **Search Animation**
- Path highlighting during search
- Node comparison visualization
- Success/failure indicators

### 4. **Split & Merge Animations**
- Tree splitting at key boundaries
- Merging two treaps
- Priority-based node movement

---

## 🛠️ Technology Stack

| Technology | Purpose |
|------------|---------|
| HTML5 | Structure |
| CSS3 | Styling & Animations |
| JavaScript | Interactivity & Logic |
| Canvas/SVG | Animation Rendering |

---

## 📁 Project Structure

```
DS-StaticWebPage/
├── index.html          # Main HTML file
├── css/
│   └── styles.css     # Styling and animations
├── js/
│   ├── treap.js       # Treap implementation
│   └── animation.js   # Animation logic
├── assets/
│   └── images/        # Static images
└── README.md          # This file
```

---

## 🚀 Features

### Interactive Visualizations
- ✨ **Real-time animation** of all operations
- ✨ **Step-by-step** execution mode
- ✨ **Speed control** for animations
- ✨ **Node highlighting** during operations

### Educational Content
- 📚 **Detailed explanations** of Treap properties
- 📊 **Time complexity** analysis
- 💡 **Use cases** and applications
- 🔄 **Comparison** with other data structures

### User Experience
- 🎨 **Modern, clean UI** design
- 📱 **Responsive** layout
- 🌈 **Color-coded** nodes (by priority)
- 🎯 **Intuitive controls**

---

## 📊 Treap Properties

### Node Structure
```
TreapNode {
    key: number        // BST key value
    priority: number   // Heap priority (random)
    left: TreapNode   // Left child
    right: TreapNode  // Right child
}
```

### Operations Complexity

| Operation | Average | Worst Case |
|-----------|---------|------------|
| Search    | O(log n) | O(n) |
| Insert    | O(log n) | O(n) |
| Delete    | O(log n) | O(n) |

---

## 🎨 Color Legend

| Color | Meaning |
|-------|---------|
| 🔴 Red | High priority node |
| 🟡 Yellow | Medium priority |
| 🟢 Green | Low priority |
| 🔵 Blue | Current operation |
| ⚪ White | Inactive/Default |

---

## 💻 How to Use

1. **Open** `index.html` in your browser
2. **Select** an operation (Insert, Delete, Search)
3. **Enter** a key value
4. **Watch** the animation play
5. **Adjust** speed using controls

---

## 🔬 Mathematical Background

### Treap Invariants

1. **BST Property**: For any node `x`:
   - All keys in left subtree < `x.key`
   - All keys in right subtree > `x.key`

2. **Heap Property**: For any node `x`:
   - `x.priority` ≥ priorities of all children

### Expected Height

The expected height of a treap with n nodes is **O(log n)**, which provides excellent practical performance.

---

## 📚 Learning Resources

### Why Treap?

- ✅ **Simplicity**: Easier to implement than balanced BSTs
- ✅ **Efficiency**: O(log n) expected operations
- ✅ **Randomization**: No complex rebalancing code
- ✅ **Versatility**: Supports split and merge operations

### Applications

- 📊 **Priority queues** with fast search
- 🔍 **Ordered sets** and maps
- 🎮 **Randomized algorithms**
- 📝 **Data structures** for competitive programming

---

## 🎯 Animation Specifications

### Insert Animation Sequence
```
1. Create new node with random priority
2. Navigate to correct BST position (visualize comparisons)
3. Insert node as leaf
4. Check heap property with parent
5. If violated: perform rotation
6. Repeat until heap property satisfied
7. Highlight final tree state
```

### Delete Animation Sequence
```
1. Navigate to target node (show search path)
2. Rotate node down until it becomes leaf
3. Remove leaf node
4. Restore heap property (show rotations)
5. Highlight final tree state
```

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

## 📝 License

This project is open source and available under the MIT License.

---

<p align="center">
  Made with ❤️ for learning Treap
</p>
