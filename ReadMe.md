# ✨ Neuro-Evolved Flappy Bird AI  

An AI-powered Flappy Bird agent built using **NEAT (NeuroEvolution of Augmenting Topologies)**. The project trains neural networks through evolutionary strategies to play Flappy Bird autonomously.  

This implementation is based on Tech With Tim’s tutorial series but includes **my own modifications**: graphical improvements, custom parameters, and adjustments to the neural network architecture for **better performance and more consistent results**.  

---

## 🚀 Features  

### 🧠 NEAT Algorithm  
- Dynamic neural network topologies (nodes + connections evolve over time)  
- Speciation, crossover, and mutation operations  
- Fitness function customized to balance **survival time** and **pipe-passing success**  

### 🎮 Flappy Bird Environment  
- Real-time simulation using **Pygame**  
- Pixel-perfect collision detection  
- Smooth graphics with **custom sprite modifications** and optimized rendering  

### 🔧 Training Enhancements  
- Additional configuration parameters in `config-feedforward.txt`  
- Neural network inputs expanded with **relative velocity** and **pipe gap distance**  
- Hidden layer adjustments for improved decision-making  
- Smarter fitness evaluation (rewards efficiency, penalizes stalling)  

### 📊 Visualization & Logging  
- Real-time on-screen visualization of evolving agents  
- Generation statistics: best fitness, average fitness, species diversity  
- Optional logging to CSV/JSON for deeper analysis  

---

## 🛠️ Technologies Used  

| Tech / Library   | Purpose |
|------------------|---------|
| Python 3.12+     | Core programming language |
| NEAT-Python      | Evolutionary algorithm framework |
| Pygame           | Game rendering and event handling |
---

## 🧑‍💻 Getting Started  

### 1. Clone the Repository  
```bash
git clone https://github.com/YOUR_USERNAME/flappy-neat-ai
cd flappy-neat-ai
```

### 2. Install Dependencies  
```bash
pip install -r requirements.txt
```

### 3. Run the Simulation  
```bash
python run.py
```

Agents will begin training and evolving in the Flappy Bird environment.  

### 4. Adjust Configuration  
Modify `config-feedforward.txt` to experiment with:  
- Population size (`pop_size`)  
- Mutation rates (`mutate_weight_rate`, `node_add_prob`)  
- Speciation thresholds (`compatibility_threshold`)  
- Elitism and stagnation limits  

---

## 📁 Project Structure  

```bash
.
├── config-feedforward.txt   # NEAT configuration
├── run.py                   # Main simulation loop
├── flappy.py                # Game environment
├── neat_ai.py               # AI evaluation & fitness logic
├── assets/                  # Sprites & graphical modifications
├── visualizer.py            # Optional matplotlib visualizer
├── logs/                    # Training logs
├── requirements.txt         # Dependencies
└── README.md
```

---

## 🧪 TODO / Future Improvements  

- Add checkpointing to save and resume training progress  
- Parallelize evaluations for faster training  
- Build a dashboard (e.g. Streamlit/Dash) for real-time monitoring  
- Apply the same NEAT logic to other environments (CartPole, LunarLander, etc.)  

---

## 📜 License  

This project is open-source and free to use under the MIT license.  

---

## 🧠 Credits  

Inspiration from Tech With Tim’s *AI Plays Flappy Bird (NEAT)* tutorial series, with **modifications by Ali Abdullah** including:  
- Custom graphical updates  
- Extra NEAT parameters  
- Modified neural network architecture for stronger performance  
