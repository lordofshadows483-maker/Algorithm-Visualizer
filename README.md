# Algorithm-Visualizer
<img width="1246" height="994" alt="image" src="https://github.com/user-attachments/assets/1c244dca-5415-4bc7-b788-e774766d3840" />

An interactive web application that visualizes popular sorting algorithms in real-time. Watch how Bubble Sort, Selection Sort, Insertion Sort, and Quick Sort work step-by-step with dynamic visual feedback.

![Algorithm Visualizer](https://via.placeholder.com/800x400/8B5CF6/FFFFFF?text=Algorithm+Visualizer)

## ✨ Features

- **Multiple Algorithms** - Visualize 4 different sorting algorithms:
  - Bubble Sort
  - Selection Sort
  - Insertion Sort
  - Quick Sort
- **Speed Control** - Adjust animation speed from 1ms to 100ms
- **Array Size Control** - Test with arrays from 5 to 100 elements
- **Performance Metrics** - Track comparisons, array accesses, and execution time
- **Color-Coded Visualization** - Different colors for comparing, swapping, and sorted elements
- **Algorithm Information** - Learn about time complexity and how each algorithm works
- **Responsive Design** - Works on desktop, tablet, and mobile devices

## 🚀 Demo

[Live Demo](your-demo-link-here) • [Video Walkthrough](your-video-link-here)

## 🎯 Why This Project?

This project demonstrates:
- **Deep CS Knowledge** - Understanding of fundamental sorting algorithms
- **Visual Communication** - Ability to explain complex concepts visually
- **Performance Analysis** - Tracking algorithm efficiency metrics
- **User Experience** - Intuitive controls and real-time feedback
- **Clean Code** - Well-structured, maintainable JavaScript

## 💻 How to Use

### Local Setup
1. Download `algorithm-visualizer.html`
2. Double-click to open in any modern web browser
3. No installation or dependencies required!

### Using the Visualizer
1. **Select an Algorithm** - Choose from the dropdown menu
2. **Adjust Settings**:
   - Use the speed slider to control animation speed
   - Change array size for different test cases
3. **Generate Array** - Click "New Array" to create a random dataset
4. **Start Sorting** - Click "Sort" to watch the algorithm in action
5. **Observe** - Watch the color-coded visualization and metrics

### Color Guide
- 🟣 **Purple** - Unsorted elements
- 🔴 **Red** - Currently comparing
- 🟡 **Yellow** - Being accessed/evaluated
- 🟢 **Green** - Sorted and in final position

## 🧮 Algorithms Explained

### Bubble Sort
Repeatedly steps through the list, compares adjacent elements, and swaps them if they're in the wrong order. Simple but inefficient for large datasets.

**Time Complexity:** O(n²)  
**Space Complexity:** O(1)  
**Best Use Case:** Educational purposes, nearly sorted data

### Selection Sort
Divides input into sorted and unsorted regions. Repeatedly selects the smallest element from the unsorted region.

**Time Complexity:** O(n²)  
**Space Complexity:** O(1)  
**Best Use Case:** Small datasets, minimal memory usage

### Insertion Sort
Builds the final sorted array one item at a time, inserting each element into its correct position.

**Time Complexity:** O(n²) average, O(n) best case  
**Space Complexity:** O(1)  
**Best Use Case:** Small datasets, nearly sorted data

### Quick Sort
Uses divide-and-conquer by selecting a pivot and partitioning the array around it. Recursively sorts sub-arrays.

**Time Complexity:** O(n log n) average, O(n²) worst case  
**Space Complexity:** O(log n)  
**Best Use Case:** General-purpose sorting, large datasets

## 🛠️ Technical Stack

- **HTML5** - Semantic structure
- **CSS3** - Tailwind CSS via CDN for styling
- **JavaScript (ES6+)** - Algorithm implementation and DOM manipulation
- **No frameworks** - Pure vanilla JavaScript

## 📊 Performance Tracking

The visualizer tracks three key metrics:

1. **Comparisons** - Number of times two elements are compared
2. **Array Accesses** - Total read/write operations on the array
3. **Time** - Actual execution time in milliseconds

These metrics help understand the practical efficiency of each algorithm.

## 🎓 Educational Value

Perfect for:
- **Computer Science Students** - Visual learning of sorting algorithms
- **Interview Preparation** - Understanding algorithm complexity
- **Teaching** - Demonstrating concepts in classroom settings
- **Self-Learning** - Exploring how algorithms work internally

## 🔧 Customization

### Adding New Algorithms
1. Create your sorting function following the existing pattern
2. Add algorithm info to the `algoInfo` object
3. Add case in the `startSort()` switch statement

### Changing Colors
Modify the Tailwind color classes:
```javascript
// In renderArray function
let bgColor = 'bg-purple-500';  // Change base color
if (highlighting.includes(idx)) {
    bgColor = 'bg-red-500';     // Change comparison color
}
```

### Adjusting Animation
Change the speed calculation:
```javascript
const speed = 101 - parseInt(document.getElementById('speed').value);
```

## 📱 Browser Compatibility

- ✅ Chrome/Edge 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Opera 76+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🚧 Future Enhancements

Potential features to add:
- [ ] More algorithms (Merge Sort, Heap Sort, Radix Sort)
- [ ] Step-by-step mode with pause between operations
- [ ] Code display showing current line executing
- [ ] Comparison mode to run multiple algorithms side-by-side
- [ ] Sound effects for comparisons and swaps
- [ ] Export visualization as video/GIF
- [ ] Dark mode support

## 📈 Performance Considerations

- Optimized rendering using CSS transitions
- Efficient array manipulation
- Debounced updates for smooth animations
- Minimal DOM operations

## 🤝 Contributing

This is a portfolio project, but suggestions are welcome! Feel free to:
- Fork the repository
- Create issues for bugs or feature requests
- Submit pull requests with improvements

## 📄 License

This project is open source and available for educational and personal use.

## 👤 Author

Created to demonstrate front-end development skills and computer science knowledge.

## 🌟 Acknowledgments

- Inspired by VisuAlgo and other algorithm visualization tools
- Built with modern web standards and best practices

---

**Learn by Watching, Understand by Doing** 🎓

*This project showcases the ability to transform complex computer science concepts into accessible, interactive visualizations.*
