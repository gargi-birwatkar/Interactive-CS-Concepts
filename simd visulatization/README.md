# SIMD Parallelism & Image Processing Visualizer

## 💡 About This Simulation

This interactive tool visualizes the **SIMD (Single Instruction, Multiple Data)** architectural model, which is the cornerstone of modern parallel computing for repetitive tasks.

The simulation demonstrates the core concept: a single control unit executes one instruction simultaneously across multiple, independent processing units (PUs), each handling a separate data stream.

## 📸 Real-World Application: Image Editing

SIMD is vital for fast, efficient image processing. This simulation is modeled after the process of applying a simple filter (like increasing brightness or contrast) to an image.

### Serial vs. Parallel Processing

Imagine an image is made up of millions of pixels. To change the color of every pixel:

| Method | Description | Time Efficiency |
| :--- | :--- | :--- |
| **Serial** (Single CPU) | The CPU fetches the data for **Pixel 1**, processes it, writes it back. Then moves to **Pixel 2**, and so on. | **Slow.** The operation must be repeated sequentially for every single pixel. |
| **SIMD** (This Simulation) | The Control Unit issues the instruction ("Increase Brightness") once. Multiple Processing Units (**PU1, PU2, PU3...**) fetch the data for **Pixel 1, Pixel 2, Pixel 3...** and execute the instruction **at the same time**. | **Fast.** The entire batch of pixels is processed in the time it takes to process a single pixel batch. |

## ⚙️ How the SIMD Simulation Works

The visualization showcases a simplified SIMD architecture (Control Unit, Instruction Bus, multiple Processing Units, and multiple Memory Modules).

### The Four Stages of Parallel Execution

The simulation animates the following steps for a batch of pixels:

1.  **Instruction Fetch:** The Control Unit (CU) retrieves an instruction (e.g., `ADD 10`) from memory.
2.  **Instruction Broadcast:** The CU sends the single instruction across the **Instruction Bus** to **all** Processing Units (PUs) simultaneously.
3.  **Data Load & Execute:** Each PU loads a unique piece of data (a pixel's value) from its assigned Memory Module (MM). All PUs then execute the same instruction on their individual data in parallel.
4.  **Write Back:** All PUs write their updated data (the processed pixel value) back to their respective Memory Modules simultaneously.



## ▶️ Getting Started

You can run this simulation easily in any modern web browser.

1.  Navigate to the simulation folder.
2.  Open the file `simd-image_editing.html` in your web browser.
3.  Use the controls to start the animation and observe the cycle of parallel execution.

---

## 💻 Technical Details

* **Technology:** HTML, CSS, and JavaScript for interactive visualization.
* **Target Audience:** Students and educators studying Computer Architecture and Parallel Processing concepts.
