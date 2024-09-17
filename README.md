# Caffeinated - Disk Analyzer

## Project Overview

**Caffeinated** is a disk analyzer tool built using the Rust programming language and the FLTK GUI library. The name "Caffeinated" is inspired by the countless hours and caffeine our team consumed during the final stages of this project. Just like caffeine helps us stay productive, this tool helps you analyze your disk space and keep your system efficient.

### Team Members:
- Nada Moursi - 900191127
- Shahd Elmahallawy - 900194441
- Mona Ahmad Kamel - 900191833

---

## Table of Contents

- [Description](#description)
- [Objectives](#objectives)
- [Features](#features)
- [Algorithms](#algorithms)
- [Challenges](#challenges)
- [Data Structures](#data-structures)
- [Manual Reference](#manual-reference)
- [Conclusion](#conclusion)

---

## Description

Caffeinated is a disk analyzer designed to display directory structures and file information using an intuitive graphical interface. Built with Rust and FLTK, this tool lets users visualize their file system structure through both a tree view and a pie chart representation of disk space usage.

## Objectives

This project was developed incrementally, starting with a backend implementation and gradually integrating a GUI to provide a complete disk analysis tool.

---

## Features

- **Directory Tree**: Displays unsorted and alphabetically sorted views of directories and their files.
- **Pie Chart Visualization**: Represents the disk usage of folders within a specific directory.
- **Terminal Interface**: Provides a command-line-like experience for users who prefer terminal-based navigation.
- **Advanced Search**: Allows users to search for files based on name, extension, and case sensitivity, with the option to limit search results.
- **File Management**: Enables users to create and delete files from within the application.

---

## Algorithms

1. **Directory Traversal**:
   - Utilizes the `WalkDir` package to traverse all directories and distinguish between folders and files.
   - The traversal result is stored in a vector, which is passed to the tree method for visual representation in the GUI.

2. **Pie Chart Integration**:
   - Calculates the percentage of space occupied by each folder in a directory.
   - The chart is updated dynamically as users navigate directories, ensuring real-time data is visualized.

---

## Challenges

We encountered multiple challenges throughout the project due to limited documentation and community support for the Rust language and its GUI libraries. Key issues included:

- **Library Selection**: We explored multiple GUI libraries (EGUI, Tauri, Angular Rust) before settling on FLTK due to its better integration with Rust. However, even FLTK had inadequate documentation, making development difficult.
- **Rust Data Types**: Rust's strict type system and string manipulation caused significant challenges, especially with data conversion between different types.
- **Lab Environment**: The lab PCs frequently crashed under the weight of our project, slowing down progress and debugging.

---

## Data Structures

- **Strings and Vectors**: The `String` and `Vec<String>` types were heavily used to manage file paths, directories, and user input.
- **Tabs and Groups**: These were used to create different views in the GUI, including the directory tree, pie chart, and terminal.
- **Pie Charts**: Utilized Rust's charting libraries to dynamically represent disk usage as a pie chart.

Key data structures include:
- `Vec<String>` for storing directory paths.
- `Group`, `Pack`, and `Tabs` to structure the application window.
- `Tree` and `PieChart` objects for visualizing directory structure and disk usage.

---

## Manual Reference

The Caffeinated application consists of six main tabs, each offering a different feature:

1. **Unsorted Directory Tree**: Displays directories in the original file system order starting from the home directory.
2. **Sorted Directory Tree**: Alphabetically sorts and displays directories.
3. **Pie Chart**: Visualizes the disk space used by folders in a given directory. Users can input a directory, and the chart will update accordingly.
4. **Terminal**: Provides a command-line interface for users who prefer a text-based navigation experience.
5. **Advanced Search**: Allows users to filter files by name, extension, and other criteria within selected directories.
6. **File Management**: Enables users to create or delete files directly from the application.

---

## Conclusion

The Caffeinated project provided us with valuable experience in both Rust and GUI development, while also highlighting the importance of well-documented programming languages. Despite the challenges we faced, we succeeded in building a fully functional disk analyzer that includes several key features for efficient disk management. However, for future projects, using a more mature and better-supported language might be a more suitable option.

---

## How to Run

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/caffeinated-disk-analyzer.git
   ```

2. Change into the project directory:
   ```
   cd caffeinated-disk-analyzer
   ```

3. Install the necessary dependencies:
   ```
   cargo build
   ```

4. Run the application:
   ```
   cargo run
   ```

Enjoy using **Caffeinated** to keep your disk in check, just like caffeine keeps you going!

--- 

**Thank you for using Caffeinated!**
