# Shark Predictor 🦈

### A Data-Driven Analysis of Shark Habitats using Simulated Oceanographic Data
*A project for the NASA International Space Apps Challenge 2025.*

---

## Our Solution
Shark Predictor is a Python-based analytical tool, presented in a Jupyter Notebook, that models and predicts the probability of shark presence. Our model is built on a fundamental ecological premise: sharks, as apex predators, are found where their prey is abundant. This project simulates key oceanographic conditions based on real-world principles to test and validate this prediction logic.

## How to Use This Project
This project is designed to be run cell by cell within a Jupyter Notebook environment.

1.  **Clone the Repository:** Get a local copy of this project.
2.  **Install Dependencies:** Run `pip install -r requirements.txt` in your terminal.
3.  **Open the Notebook:** Launch Jupyter and open the `shark-notebook-fixed.ipynb` file.
4.  **Configure Locations:** In the second code cell, you can modify the `locations_to_analyze` list to test any coordinates you wish.
5.  **Run the Analysis:** Execute the cells sequentially to see the data simulation and validity checks for your chosen locations.

---

## The Science Behind Shark Predictor
Our model integrates key pillars of oceanographic data to create a dynamic probability map.

- **Phytoplankton & Chlorophyll:** We simulate chlorophyll-a concentration (the base of the marine food web) using data from NASA's MODIS sensor as a scientific basis. High chlorophyll suggests abundant food sources.
- **Sea Surface Temperature (SST):** Sharks prefer specific temperature ranges. Our model is based on data from sensors like MODIS and VIIRS, identifying thermal comfort zones and critical thermal fronts where prey congregates.
- **Ocean Dynamics:** Using principles from datasets like ASCAT Wind Vectors, our simulation accounts for ocean currents and their strength, which are crucial for nutrient transport and prey movement.

---

### Technology Stack
- **Analysis & Modeling:** Python (Pandas, Matplotlib, NumPy)
- **Environment Management:** MiniConda / venv
- **Prototyping:** Jupyter Notebook
- **AI Assistants:** Google Gemini, Manus AI, Claude AI, ChatGPT

### Next Steps & Future Improvements
This notebook serves as the foundational logic for the Shark Predictor system. The current version uses a sophisticated simulation of ocean data. The next steps are:
- **Integrate Live APIs:** Replace the simulation functions with real-time API calls to NASA Earthdata and Copernicus to fetch live oceanographic data.
- **Implement the Full ML Model:** Add the complete machine learning predictor class to translate the simulated data into a final probability score.

### Our Team
- Rafael Silva Nascimento
- Caio Artiaga Gondim
- Erick Henrique de Oliveira Medeiros
- Henrique Miranda Chaves
- Bruno Henrique Leão
- Eduardo Silva Oliveira
