# My Learning Journal 🥜

This GitHub repository serves as a collection of my daily learnings in technology. Here, you'll find notes, code snippets, and resources that reflect my progress and insights.

## 🛠️ CMake

CMake is an open-source, cross-platform tool designed to manage the build process of software using compiler-independent configuration files. It generates platform-specific build scripts, such as Makefiles for Linux or project files for IDEs like Visual Studio, from a single set of configuration files. I can learn from [here](https://cmake.org/getting-started/).

## 🧠 Keras

Keras is a high-level deep learning API that allows users to easily build, train, and deploy neural networks. It abstracts many low-level details of neural networks and provides a simple, user-friendly interface for complex tasks. [Explore](https://www.notion.so/Keras-e2587ac62cf14f1aa3bf410feaf480b4).

## 🔦 Lidar

Lidar is a method for determining ranges by targeting an object or a surface with a laser and measuring the time for the reflected light to return to the receiver. [Wiki](https://en.wikipedia.org/wiki/Lidar)

## 🛣️ Lin–Kernighan Algorithm

The [Lin–Kernighan algorithm](https://en.wikipedia.org/wiki/Lin%E2%80%93Kernighan_heuristic) is a powerful heuristic for solving the Traveling Salesman Problem (TSP), which is a classic NP-hard combinatorial optimization problem. This algorithm is designed to find a near-optimal solution through iterative local optimization techniques.

##  🕸️ Darknet
[Darknet](https://pjreddie.com/darknet/) is an open-source neural network framework written in C and CUDA, designed for both CPU and GPU computing. It’s widely known for powering the YOLO (You Only Look Once) object detection models, which are some of the fastest and most popular real-time object detectors.

## Transfer Learning 
need for OpenDub (automatic dialogue generator from subtitle) implementation.

## GraphQL 
need for bug-book (journal book of errors) why? see chatgpt.

## Hoisting 
[link](https://www.digitalocean.com/community/tutorials/understanding-hoisting-in-javascript)

[more](https://github.com/yangshun/top-javascript-interview-questions?trk=feed_main-feed-card_feed-article-content)

## Symlink
A symbolic link (or symlink) is a special type of file in Unix-like operating systems that serves as a reference or pointer to another file or directory. It acts like a shortcut, allowing you to access files or directories from multiple locations without duplicating the actual data. [Explore](https://en.wikipedia.org/wiki/Symbolic_link)

## Flyweight Pattern
[link](https://refactoring.guru/design-patterns/flyweight)

## Shadowing
Shadowing occurs when a variable in a certain scope (like inside a function) has the same name as a variable in an outer scope (like the global scope). When this happens, the inner variable "shadows" or "hides" the outer variable, meaning that within the inner scope, any reference to that variable name will refer to the inner variable rather than the outer one.
#### Example of Shadowing:

```python

x = 10  # Global variable

def example_function():
    x = 5  # Local variable, shadows the global variable
    print(f"Inside function: {x}")  # This prints 5

example_function()  # Call the function
print(f"Outside function: {x}")  # This prints 10
```

## TRAINEDDATA File

[A TRAINEDDATA file is an optical character recognition (OCR) model created by Tesseract.](https://fileinfo.com/extension/traineddata)

## LSTM
[link](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)

## Reverse Proxy

## VGSL
## Otsu algorithm
## Alpha Channel
[link](https://www.linearity.io/blog/alpha-channel/)
## DPI
DPI stands for Dots per Inch, referring to the number of ink droplets a printer will produce per inch while printing an image. The more dots of ink per inch the picture has, the more detail you will see when printed. [wiki](https://en.wikipedia.org/wiki/Dots_per_inch)
## Putty
[wiki](https://en.wikipedia.org/wiki/PuTTY)

## fzf

## Handling OpenCV Scripts

<details> <summary>more</summary>


#### Exiting OpenCV Programs
If your OpenCV script gets stuck because of `cv2.imshow` and `cv2.waitKey(0)`, you can use the following methods to exit:

1. **Use `Ctrl+C`:** This sends an interrupt signal to terminate the program.
2. **Use `Ctrl+Z`:** This suspends the process. To terminate it completely:
   - Run `jobs` to list suspended jobs.
   - Use `kill %<job-id>` to terminate it.
   - Alternatively, use `fg` to bring it to the foreground, then `Ctrl+C` to exit.

#### Preventing Blocking Behavior
To avoid this issue in the future:
1. Use `cv2.waitKey(<timeout>)` with a specific timeout (e.g., `cv2.waitKey(1000)` for 1 second).
2. Replace `cv2.imshow` calls with file-saving commands (e.g., `cv2.imwrite`).
3. If running in a headless environment, remove GUI-related calls or use virtual displays like `Xvfb`.
</details>

