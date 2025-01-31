# Self-Driving Car Simulation with Neural Networks

A JavaScript implementation of a self-driving car simulation using Neural Networks, based on freeCodeCamp's Neural Networks and Machine Learning course.

## 🚀 Features

- **Neural Network Implementation**  
   Custom neural network from scratch with mutation capabilities
- **Sensor System**  
   Ray-casting collision detection with road borders and traffic
- **AI Training**  
   Genetic algorithm implementation with generational evolution
- **Visualization Tools**  
   Real-time network architecture visualization using HTML5 Canvas
- **Persistent Storage**  
   Save/load best performing brain models using localStorage

## 🛠 Technologies

- Vanilla JavaScript (ES6+)
- HTML5 Canvas for rendering
- Web Storage API for model persistence
- RequestAnimationFrame for smooth animations

## 📥 Installation

1. Clone repository:

```bash
git clone https://github.com/yourusername/Asphyxia
```

2. Navigate to project directory:

```bash
cd /e:/Download/Documents/Asphyxia/Coding/Artificial Intelligence/Self-Driving
```

3. Open index.html in your browser

## 🕹 Controls

| Key       | Action             |
| --------- | ------------------ |
| `↑` Arrow | Accelerate         |
| `↓` Arrow | Brake/Reverse      |
| `←` Arrow | Steer Left         |
| `→` Arrow | Steer Right        |
| `S`       | Save Best Model    |
| `D`       | Delete Saved Model |

## 🧠 AI Training

```javascript
// Initialize population
const N = 100;
const cars = generateCars(N);

// Load best model
if (localStorage.getItem("bestBrain")) {
  cars[0].brain = JSON.parse(localStorage.getItem("bestBrain"));
}

// Mutate other cars
NeuralNetwork.mutate(cars[i].brain, 0.1);
```

## 📁 File Structure

```
Artificial Intelligence/Self-Driving/
├── neural-network/
│   ├── network.js      # Neural network core
│   └── visualizer.js   # Neural Network Simulation
├── car-system/
│   ├── car.js          # Vehicle physics
│   ├── sensor.js       # Collision detection
│   └── controls.js     # Input handling
├── environment/
│   ├── road.js         # Track generation
└── utils/              # Math helpers
```

## 📜 License

MIT License - see [LICENSE](LICENSE) for details

## 🙏 Acknowledgments

- Inspired by freeCodeCamp's Machine Learning curriculum
- Vehicle physics model adapted from Realistic Car Driving simulators
