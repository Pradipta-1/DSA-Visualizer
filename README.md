# DSA Visualizer

> **See algorithms. Understand algorithms. Master DSA.**

DSA Visualizer is a browser-based, interactive learning tool for understanding Data Structures and Algorithms through animation, step-by-step execution, code tracing, theory, and complexity analysis.

The project is designed to make DSA easier to learn by showing **what an algorithm is doing at each step**, not just displaying the final answer.

---

## ✨ Features

### 🧠 Interactive Algorithm Visualizations

The visualizer uses a step-based execution model so operations can be observed one step at a time.

Currently implemented interactive areas include:

- Linear Search
- Binary Search
- Bubble Sort
- Selection Sort
- Insertion Sort
- Merge Sort
- Quick Sort
- Singly Linked List
- Doubly Linked List
- Circular Linked List
- Stack using Array
- Stack using Linked List
- Simple Queue
- Circular Queue
- Queue using Linked List
- Deque
- Priority Queue
- Recursion visualizations:
  - Factorial
  - Fibonacci
  - Tower of Hanoi
  - Recursion Tree
- Tree visualizations:
  - Binary Tree
  - Binary Search Tree
  - Inorder Traversal
  - Preorder Traversal
  - Postorder Traversal
  - Recursive Traversal
  - Iterative Traversal

The roadmap also includes advanced data structures, graph algorithms, problem-solving techniques, and challenge mode.

---

## 🌳 Tree Module

The tree section is one of the major interactive parts of the project.

### Tree Theory

The learning section covers:

- Tree Terminology
- Binary Tree
- Full Binary Tree
- Complete Binary Tree
- Perfect Binary Tree
- Balanced Tree
- Binary Search Tree

The theory pages combine definitions, explanations, visual diagrams, examples, and complexity information.

### Binary Tree

The Binary Tree visualizer supports:

- Search
- Insertion
- Deletion
- Random tree generation
- Sample tree reset
- Step-by-step operation playback
- Visual highlighting of the current/visited node

For the plain Binary Tree, insertion follows a level-order strategy and deletion uses the deepest-node replacement approach to preserve the tree's compact structure.

### Binary Search Tree

The BST visualizer supports:

- Search
- Insertion
- Deletion
- Random tree generation
- Sample tree reset
- Step-by-step search paths
- Duplicate handling
- Deletion of:
  - Leaf nodes
  - Nodes with one child
  - Nodes with two children

BST deletion demonstrates the standard replacement process for a node with two children using the inorder successor.

### Tree Traversals

The traversal visualizer supports:

- Inorder
- Preorder
- Postorder
- Recursive traversal
- Iterative traversal

Traversal controls allow the learner to select:

- Tree type: Binary Tree or BST
- Traversal order
- Execution mode: Recursive or Iterative

The visualizer shows the traversal sequence and, for iterative traversal, the explicit stack used to keep track of pending nodes.

---

## 🎬 Playback Controls

Interactive visualizations provide controls such as:

- **Restart** — reset the visualization
- **Previous** — move one step backward
- **Play / Pause** — automatically run the visualization
- **Next** — advance one step
- **Randomize** — generate new input/tree data
- **Speed controls** — 0.25×, 0.5×, 1×, 2×, and 4×
- **Progress bar** — jump to a particular step

The step engine keeps the visualization, explanation, and code highlighting synchronized.

---

## 📖 Explanation, Code, Input & Info

The workspace contains four main learning tabs:

### Explanation

Shows what is happening during the current execution step and explains why the step matters.

### Code

Displays the relevant implementation and highlights the logic being executed.

### Input

Allows the learner to change the data used by supported visualizations.

### Info

Provides theory, concepts, complexity, terminology, applications, and other important facts related to the selected data structure or algorithm.

For the tree module, the Info section includes material for Binary Trees, BSTs, searching, insertion, deletion, traversal methods, recursive traversal, and iterative traversal.

---

## 🎨 Theme Support

The visualizer supports:

- Dark theme
- Light theme

The theme preference is stored in the browser using `localStorage`.

The sidebar, roadmap cards, workspace panels, buttons, borders, and other interface elements adapt to the selected theme.

---

## 🔎 DSA Topic Search

The application includes a built-in DSA search interface.

You can search for topics such as:

- Binary Tree
- Binary Search Tree
- Stack
- Queue
- Searching
- Sorting
- Traversal
- Recursion

The search system searches the topics exposed in the roadmap/sidebar and opens the corresponding learning or visualization area.

A keyboard shortcut is also available:

```text
Ctrl + K
```

---

## 🧭 Roadmap

The sidebar organizes the learning material into a DSA roadmap.

The roadmap currently includes areas such as:

1. DSA Fundamentals
2. Arrays
3. Linked Lists
4. Stack
5. Queue
6. Hashing
7. Trees
8. Tree Traversals
9. Heap
10. Graphs
11. Searching
12. Sorting
13. Recursion
14. Advanced Linked List
15. AVL Tree
16. More Topics

All roadmap sections currently shown in the application have working interactive routes or educational demos.

The **Challenges** section is interactive and includes DSA questions with feedback and scoring.

---

## 🏗️ Architecture

The project follows a lightweight client-side architecture built around a reusable visualization engine.

Conceptually, the execution flow is:

```text
User Input
   ↓
Algorithm / Data Structure Engine
   ↓
Step Generator
   ↓
Step State
   ↓
Visualization Renderer
   ↓
Code + Explanation + Info Panel
```

### Step Generator

Each operation generates a sequence of structured steps.

A step can contain information such as:

- Operation type
- Current node/index
- Visited elements
- Highlighted elements
- Code line
- Explanation
- Reason / why the step matters
- Extra operation metadata

This makes the visualizer reusable across multiple algorithms.

### Renderer

The renderer consumes those steps and updates:

- The main visualization
- Current state
- Code highlighting
- Explanation panel
- Progress
- Traversal output
- Stack visualization where applicable

---

## 🧩 Visualization Technologies

The project is implemented as a client-side web application using:

- **HTML5**
- **CSS3**
- **Vanilla JavaScript**
- **SVG** for diagrams and tree visualizations
- **HTML Canvas** for the complexity explorer
- **CSS animations and transitions**
- **Local Storage** for theme preference

The interface also uses web fonts including:

- Space Grotesk
- Inter
- JetBrains Mono
- Bricolage Grotesque

No frontend framework is required.

---

## 📁 Project Structure

The current implementation is intentionally simple and portable.

```text
dsa-visualizer/
│
├── dsa_visualizer_tree_implemented.html
└── README.md
```

The main application is contained in a single HTML file, which includes:

- Page structure
- Styling
- Navigation
- Algorithm engines
- Data structures
- Visualization rendering
- Theory content
- Controls
- Theme logic

This makes the project easy to download and run locally.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

Replace the repository URL with your actual GitHub repository URL.

### 2. Open the project

Because the project is a client-side HTML application, no backend setup is required.

You can simply open:

```text
dsa_visualizer_tree_implemented.html
```

in a modern browser.

### 3. Recommended browsers

Use a recent version of:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox

---

## 💡 How to Use

### To visualize an algorithm

1. Open the application.
2. Select an algorithm from the sidebar or Algorithms section.
3. Enter or generate input where supported.
4. Press **Next** to study the algorithm step by step.
5. Press **Play** to watch the complete execution.
6. Use **Previous** or **Restart** to review the process.
7. Read the Explanation, Code, Input, and Info tabs.

### To study trees

1. Open **Trees** in the DSA Roadmap.
2. Select Binary Tree or Binary Search Tree.
3. Use Search, Insert, Delete, or Randomize.
4. Step through each operation.
5. Open the Info tab for the theory and complexity.
6. Open Tree Traversals to experiment with Inorder, Preorder, and Postorder.
7. Switch between Recursive and Iterative traversal modes.

---

## 📊 Complexity Explorer

The application includes an interactive complexity graph for comparing growth rates.

It supports visualizing common asymptotic classes such as:

```text
O(1)
O(log n)
O(n)
O(n log n)
O(n²)
O(2ⁿ)
```

The graph uses a logarithmic visual scale so rapidly growing functions remain readable alongside slower ones.

---

## 🎓 Learning Philosophy

The project is built around a simple idea:

> **Do not only learn the final output. Learn the process that creates it.**

For each supported visualization, the goal is to connect four things:

```text
Theory
  ↓
Algorithm
  ↓
Code
  ↓
Visual Execution
```

For example, while learning BST search, the learner can see:

```text
Target
  ↓
Compare with current node
  ↓
Target < node → go left
Target > node → go right
  ↓
Repeat
  ↓
Found / Not Found
```

This approach makes it easier to connect textbook concepts with actual program execution.

---

## 🛠️ Extending the Project

The architecture is designed so new visualizations can be added without rebuilding the entire application.

A typical new module can be added by implementing:

1. Data structure / algorithm logic
2. Step generator
3. Visualization renderer
4. Controls
5. Code snippet
6. Explanation content
7. Info/theory content
8. Catalog/sidebar registration

For example, a future data structure can follow:

```javascript
function generateSteps(input) {
    const steps = [];

    // algorithm logic
    // push structured states into steps

    return { steps };
}
```

Then the renderer can consume each state and update the UI.

---

## 🧪 Current Roadmap

The project is being developed incrementally.

### Implemented

- Searching
- Sorting
- Linked Lists
- Stacks
- Queues
- Priority Queue
- Recursion
- Binary Tree
- Binary Search Tree
- Tree Traversals
- Theory pages
- Complexity Explorer
- Dark/Light theme
- Topic search
- Responsive interface

### Advanced / Implemented

The project now includes interactive educational modules for:

- Hash Tables and collision handling
- Heaps, Heapify, Extract Min/Max, Heap priority queues, and Heap Sort
- Trie
- AVL Trees and rotations
- Graph representations
- BFS and DFS
- Dijkstra and A*
- Prim and Kruskal
- Topological Sort
- Strongly Connected Components
- Bellman-Ford
- Floyd-Warshall
- Disjoint Set / Union-Find
- Segment Tree
- Fenwick Tree / BIT
- Backtracking
- N-Queens
- Sudoku
- Maze solving
- Subsets and permutations
- Dynamic Programming
- Greedy Algorithms
- Divide and Conquer
- Bit Manipulation
- String Algorithms / KMP
- Jump Search
- DSA Challenge mode

---

## 📱 Responsive Design

The UI is designed to work across:

- Desktop
- Laptop
- Tablet
- Mobile

The sidebar becomes a mobile navigation drawer on smaller screens, while visualization areas adapt to available width.

---

## 🔗 Shareable Visualizations

The application supports generating a shareable URL for the currently selected visualization.

When a supported visualizer is selected, the application can encode the selected visualization in the URL hash so it can be reopened directly.

---

## 🔐 Privacy

The application is designed as a client-side learning tool.

- Algorithms execute in the browser.
- No backend is required.
- User input remains in the browser during normal use.
- Theme preference is stored locally using browser storage.

---

## 🤝 Contributing

Contributions are welcome.

A useful contribution can be:

- Adding a new algorithm
- Improving an existing visualization
- Adding theory or examples
- Improving accessibility
- Fixing responsive UI issues
- Improving animation quality
- Adding test cases
- Improving documentation

Recommended workflow:

```bash
git checkout -b feature/your-feature
```

Make your changes, test them locally, then commit:

```bash
git add .
git commit -m "Add your feature"
git push origin feature/your-feature
```

Then open a pull request on GitHub.

---

## 🐛 Reporting Issues

When reporting a bug, include:

- Browser and version
- Device / operating system
- Algorithm or topic where the issue occurs
- Steps to reproduce
- Expected behavior
- Actual behavior
- Screenshot or screen recording, when useful

---

## 📜 License

The application's About section currently describes the project as **MIT licensed**.

If the repository does not yet contain a `LICENSE` file, add the MIT License file before treating the repository as formally licensed.

---

## ⭐ Acknowledgement

This project is intended as an educational DSA visualization tool for students, beginners, interview preparation, and anyone who wants to understand algorithms by seeing them execute.

---

## 👨‍💻 Author

**Pradipta Santra**

Computer Science Engineering student focused on Data Structures & Algorithms, web development, and software projects.

---

## ⭐ Star the Repository

If this project helps you understand DSA, consider giving the repository a ⭐ on GitHub.

```text
Learn → Visualize → Trace → Understand → Practice
```
