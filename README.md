### DSAHelper- Data Structure & Algorithm Visualizer
A web-based tool for visualizing data structures and algorithms using Rust for computation (compiled to WebAssembly) and React for visualization.

## Project Overview
DSAHelper helps users understand algorithms and data structures through interactive visualizations. This project combines the performance of Rust with the visualization capabilities of React to create an educational tool that demonstrates how algorithms work.

## Setup Instructions
Prerequisites
"
Node.js (v14 or later)
Rust (latest stable)
wasm-pack
"

## Setting Up the Development Environment

Clone the repository
"
bashgit clone https://github.com/yourusername/algoviz.git
cd algoviz
" 

Set up the Rust/WebAssembly project
"
bash# Add WebAssembly target
rustup target add wasm32-unknown-unknown
"

Build the WebAssembly package
"
cd algoviz  # The Rust project directory
wasm-pack build --target web
"

Set up the React frontend
"
bashcd ../frontend  # Navigate to the React project directory
npm install
npm install ../algoviz/pkg  # Install the local WebAssembly package
"

Start the development server
"
bashnpm start
"

The application should now be running at http://localhost:3000

## Available Visualizations

Array operations
Sorting algorithms (Bubble Sort, Quick Sort, Merge Sort)
Binary Search Tree operations
Graph algorithms
More coming soon!

## Development Workflow

Implement algorithms in Rust (in algoviz/src/)
Build WebAssembly package with wasm-pack build --target web
Create visualization components in React (in frontend/src/components/)
Connect React components to WebAssembly functions
