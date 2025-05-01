# Molecular Toxicity Predictor

## Mini Project

## Overview
**Molecular Toxicity Predictor** is a deep learning-based web application that predicts the toxicity of chemical compounds based on their SMILES representation.  
It offers features like:
- Toxicity prediction across 12 biological endpoints using a pretrained Graph Convolutional Neural Network (GCN).
- Molecular property calculation (Molecular Weight, LogP, Hydrogen Bond Donors/Acceptors, etc.).
- 3D molecular visualization.
- AI-driven interpretation of results using Gemini AI.
- Clean single-page React frontend for a smooth user experience.

![Molecular Toxicity Predictor - Interface](ss1.jpg)

![Molecular Properties](ss2.jpg)

![Plotted visulalisation of Prediction](ss3.jpg)

## Installation Instructions

### Backend Setup (Python - Flask)

1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```

2. Create a virtual environment (perform only once):
   ```bash
   python3.9 -m venv env39
   # or if above fails
   py -3.9 -m venv env39
   ```

3. Activate the virtual environment (every time you start):
   ```bash
   .\env39\Scripts\Activate.ps1  # On Windows PowerShell
   ```
   or
   ```bash
   source env39/bin/activate  # On Linux/macOS
   ```

4. Install backend dependencies:
   ```bash
   pip install -r requirements.txt
   ```

5. Run the backend server (every time):
   ```bash
   python app.py
   ```

---

### Frontend Setup (React)

1. Install frontend dependencies:
   ```bash
   npm install
   npm install styled-components
   npm install primereact
   npm install three @react-three/fiber @react-three/drei three-orbitcontrols
   ```

2. Start the frontend development server:
   ```bash
   npm start
   ```

---

## Technologies Used

- **Backend:** Python (Flask), RDKit, DeepChem
- **Frontend:** React.js, Three.js, PrimeReact, Styled-Components
- **Visualization:** Three.js + @react-three libraries
- **Deep Learning:** Graph Convolutional Network (via DeepChem)
- **AI Assistant:** Gemini API
- **Version Control:** Git & GitHub

---

## Features

- Predict toxicity across 12 biological endpoints from the Tox21 dataset.
- Calculate key molecular descriptors automatically.
- View 3D structure of input molecules interactively.
- Get AI-powered human-readable explanations for predictions.
- Intuitive, responsive single-page web interface.

---
