# AlgoViz — Interactive Algorithm Visualizer

**AlgoViz** is a browser-based interactive algorithm laboratory designed to make algorithms and data structures easier to understand through **visualization, step-by-step execution, live statistics, explanations, comparison, and quizzes**.

It is built as a **single standalone HTML file**, using HTML, CSS, and vanilla JavaScript — no framework, backend, build process, or external dependency is required.

---

## ✨ Features

### 🔢 Sorting Algorithms

Visualize sorting algorithms step by step:

- Bubble Sort
- Selection Sort
- Insertion Sort
- Merge Sort
- Quick Sort
- Heap Sort

Each visualization shows:

- Comparisons
- Swaps
- Array accesses
- Current operation
- Elapsed time
- Highlighted elements
- Live pseudocode
- Algorithm explanation
- Time and space complexity

---

### 🔍 Searching Algorithms

Explore searching algorithms interactively:

- Linear Search
- Binary Search

Binary Search automatically works with a sorted array and visually displays:

- `LOW`
- `MID`
- `HIGH`
- Eliminated search ranges
- Successful matches
- Failed searches

You can also enter a custom target value.

---

### 🧱 Data Structures

AlgoViz includes interactive demonstrations of:

- Stack
- Queue
- Linked List
- Binary Search Tree
- Heap
- BST Traversal

Operations can be performed directly through the interface.

Examples include:

**Stack**
- Push
- Pop
- Peek

**Queue**
- Enqueue
- Dequeue
- Peek

**Linked List**
- Insert
- Delete
- Search

**Binary Search Tree**
- Insert
- Search
- Delete
- Inorder traversal
- Preorder traversal
- Postorder traversal
- Level-order traversal

**Heap**
- Insert
- Remove minimum
- Heapify

---

### 🕸️ Graph Algorithms

Interactive graph visualizations are available for:

- Breadth-First Search (BFS)
- Depth-First Search (DFS)
- Dijkstra's Algorithm
- A* Pathfinding

The graph editor supports operations such as:

- Add nodes
- Connect nodes
- Delete nodes
- Set start node
- Set destination node
- Move nodes
- Visualize visited nodes
- Display shortest paths
- Display distances

A* also provides an interactive grid where walls can be added or removed.

---

### 🔁 Recursion Visualizer

The recursion visualizer demonstrates how recursive calls are placed on and removed from the call stack.

The included example visualizes:

```text
factorial(5)
```

You can observe:

- Recursive calls
- Stack frames
- Base case
- Return values
- Final result

---

## 🎮 Visualization Controls

The main visualizer provides:

- **Generate Array** — creates a new dataset
- **Randomize** — generates a new random array
- **Start** — automatically runs the visualization
- **Pause** — pauses an active animation
- **Step** — executes one algorithm operation
- **Reset** — resets the current run
- **Array Size** — controls the number of values
- **Animation Speed** — controls execution speed
- **Target Value** — used by searching algorithms

The application supports five animation speeds:

```text
Slow
Relaxed
Medium
Fast
Turbo
```

---

## 🧠 Learning Mode

AlgoViz includes a dedicated **Learning Mode**.

When enabled, the application provides additional explanations describing *why* an operation occurred.

For example, instead of only showing a swap, the application can explain the reason behind the swap and how that operation contributes to the algorithm.

There is also an:

> **Explain like I'm a beginner**

option for simpler explanations.

---

## 📊 Live Statistics

While an algorithm is running, AlgoViz tracks:

| Statistic | Description |
|---|---|
| Comparisons | Number of comparisons performed |
| Swaps | Number of swaps performed |
| Array accesses | Number of array accesses |
| Current step | Current visualization step |
| Elapsed | Time spent running |

A recent-activity panel also shows the latest algorithm operations.

---

## ⚖️ Algorithm Comparison

The comparison tool allows you to run **two sorting algorithms against the same dataset**.

The results include:

- Generated operations
- Comparisons
- Swaps
- Array accesses
- Trace-generation time
- Average time complexity

This makes it easier to understand how different sorting algorithms behave on identical input.

---

## 📝 Quiz Mode

AlgoViz includes a built-in quiz system for testing algorithm knowledge.

Current questions cover topics such as:

- FIFO data structures
- BFS
- Quick Sort complexity
- Insertion Sort
- Binary Search requirements

The application tracks:

```text
Correct answers
Total questions
Quiz score
```

Quiz progress is saved locally in the browser.

---

## 💻 Technology Stack

AlgoViz is intentionally lightweight.

### Frontend

- HTML5
- CSS3
- JavaScript
- SVG
- Browser Local Storage

### No dependencies

The project does **not** require:

- React
- Vue
- Angular
- Node.js
- npm
- Webpack
- Vite
- Backend server
- Database

Everything is contained inside the HTML file.

---

## 🚀 Getting Started

https://priyanshjain08.github.io/Algorithm-Visualizer/

---

## 📁 Project Structure

The project currently uses a single-file architecture:

```text
AlgorithmVisualiser.html
```

The file contains:

```text
AlgorithmVisualiser.html
│
├── HTML
│   ├── Sidebar navigation
│   ├── Visualizer controls
│   ├── Visualization area
│   ├── Algorithm information
│   ├── Statistics
│   ├── Live pseudocode
│   ├── Explanations
│   ├── Comparison tool
│   └── Quiz mode
│
├── CSS
│   ├── Dark UI theme
│   ├── Responsive layout
│   ├── Visualization styles
│   ├── Animations
│   └── Mobile styles
│
└── JavaScript
    ├── Algorithm definitions
    ├── State management
    ├── Sorting traces
    ├── Searching traces
    ├── Data structures
    ├── Graph algorithms
    ├── A* pathfinding
    ├── Recursion visualization
    ├── Comparison engine
    ├── Quiz engine
    └── Local persistence
```

---

## 🧩 Supported Algorithms

### Sorting

| Algorithm | Best | Average | Worst | Space |
|---|---:|---:|---:|---:|
| Bubble Sort | O(n) | O(n²) | O(n²) | O(1) |
| Selection Sort | O(n²) | O(n²) | O(n²) | O(1) |
| Insertion Sort | O(n) | O(n²) | O(n²) | O(1) |
| Merge Sort | O(n log n) | O(n log n) | O(n log n) | O(n) |
| Quick Sort | O(n log n) | O(n log n) | O(n²) | O(log n) |
| Heap Sort | O(n log n) | O(n log n) | O(n log n) | O(1) |

### Searching

| Algorithm | Best | Average | Worst |
|---|---:|---:|---:|
| Linear Search | O(1) | O(n) | O(n) |
| Binary Search | O(1) | O(log n) | O(log n) |

### Graph Algorithms

| Algorithm | Complexity |
|---|---:|
| BFS | O(V + E) |
| DFS | O(V + E) |
| Dijkstra | O((V + E) log V) |
| A* | O(E) |

---

## 💾 Data Persistence

AlgoViz uses the browser's **Local Storage** to remember selected user preferences and quiz progress.

The application stores data under:

```text
algoviz.state.v1
```

Stored information includes items such as:

- Selected algorithm
- Array size
- Animation speed
- Learning-mode preference
- Quiz score
- Recent activity

No external database is required.

---

## 📱 Responsive Design

The interface is designed to work across:

- Desktop
- Laptop
- Tablet
- Mobile screens

On smaller screens, the sidebar navigation changes to a compact algorithm selector.

The application also includes support for users who prefer reduced motion through the browser's `prefers-reduced-motion` setting.

---

## 🎨 UI Design

AlgoViz uses a dark, modern interface featuring:

- Glass-style panels
- Gradient backgrounds
- Animated visualization elements
- Responsive cards
- Color-coded algorithm states
- Accessible focus states
- SVG-based trees and graphs

Visualization colors communicate different states such as:

- Comparing
- Swapping
- Sorted
- Current
- Pivot
- Visited
- Path
- Start
- Destination

---

## 🧠 How the Visualizer Works

Instead of simply animating decorative UI elements, the application generates a sequence of **algorithm trace events**.

Each event can contain information such as:

```text
Operation
Pseudocode line
Explanation
Why the operation happened
Array state
Highlighted elements
Statistics changes
Graph state
Recursion state
```

The visualization engine then applies these events one at a time.

This allows the same execution engine to power both:

```text
▶ Start
⏸ Pause
⏭ Step
```

and makes the visualization useful for learning how the underlying algorithm actually operates.

---

## 🔧 Customization

Algorithms are defined inside the `ALGORITHMS` configuration object.

A new algorithm can be added by defining information such as:

```javascript
{
    name: "My Algorithm",
    category: "Sorting",
    kind: "sort",
    desc: "Description of the algorithm",
    best: "O(...)",
    avg: "O(...)",
    worst: "O(...)",
    space: "O(...)",
    stable: "Yes",
    inPlace: "Yes",
    code: [
        "step 1",
        "step 2",
        "step 3"
    ]
}
```

The corresponding trace-generation logic can then be added to the visualization engine.

---

## 🔐 Privacy

AlgoViz is a client-side application.

It does not require a backend or external database. User preferences and quiz progress are stored in the browser using Local Storage.

Because the project is a standalone HTML application, it can also be used offline after the file has been obtained.

---

## ⚠️ Limitations

This project is primarily an **educational visualization tool** rather than a production-grade algorithm benchmarking suite.

In particular:

- Visualization overhead affects measured JavaScript execution time.
- Trace-generation time should not be interpreted as real-world algorithm runtime.
- The visualized dataset sizes are intentionally limited for usability.
- Complexity values describe the implemented algorithms rather than guaranteeing performance for every possible implementation.
- Browser Local Storage is device/browser-specific.

---

## 🔮 Future Improvements

Possible future enhancements include:

- More sorting algorithms
- More graph algorithms
- Dynamic algorithm code highlighting
- Custom user-defined datasets
- Side-by-side visualization mode
- More quiz questions
- Progress tracking
- Exportable learning reports
- Algorithm animation recording
- Light theme
- Keyboard shortcuts
- More advanced graph editing
- Interactive complexity charts

---


## 👨‍💻 Project

**AlgoViz — Interactive Algorithm Visualizer**

A lightweight educational tool for learning algorithms and data structures through interactive visualization.

Built with:

```text
HTML + CSS + Vanilla JavaScript
```

**No framework. No backend. No build step.**

---

## ⭐ Why AlgoViz?

Traditional algorithm explanations often rely on static diagrams or blocks of code.

AlgoViz turns those concepts into an interactive experience where you can:

**Select → Generate → Run → Pause → Step → Understand → Compare → Test Yourself**

The goal is simple:

> **Don't just read the algorithm. Watch it happen.**
