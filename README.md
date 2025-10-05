# Shark Predictor 🦈

### For Safe, Data-Driven Human-Marine Coexistence
*A project for the NASA International Space Apps Challenge 2025.*

---

## The Problem
Human-shark interactions are increasing, posing risks to both public safety and marine ecosystems. Coastal communities, scientists, and conservationists lack accessible, real-time tools to understand and predict where sharks are likely to be, making it difficult to implement proactive safety and conservation strategies.

## Our Solution
Shark Predictor is a data-driven application that uses a machine learning model to predict the probability of shark presence. Our model is built on a fundamental ecological premise: sharks, as apex predators, are found where their prey is abundant. Prey abundance is dictated by specific oceanographic conditions that we can measure from space, turning the ocean into an open book.

---

## The Science Behind Shark Predictor
Our model integrates three key pillars of NASA data to create a dynamic probability map.

### 🌿 Phytoplankton: The Ocean's Green Heart
**Why it Matters:** Phytoplankton forms the base of the entire marine food web. High concentrations attract zooplankton, which attract small fish, which in turn attract the larger predators—sharks. A map of phytoplankton is essentially a map of potential feeding grounds.
**NASA Data Used:** We use data from the MODIS sensor on NASA's Aqua and Terra satellites to measure Chlorophyll-a concentration, a direct indicator of phytoplankton presence.

### 🔥 Sea Surface Temperature (SST): The Predator's Comfort Zone
**Why it Matters:** Each shark species has an ideal temperature range. More importantly, thermal fronts—where cold and warm water masses meet—are highly productive hunting zones. These fronts act as natural barriers, concentrating nutrients and prey. As demonstrated by Queiroz et al. (2016) in PNAS, sharks actively select habitats characterized by strong thermal gradients.
**NASA Data Used:** Sensors like MODIS and VIIRS provide daily global SST maps, allowing our model to identify both thermal comfort zones and these critical thermal fronts.

### 💨 Ocean Dynamics: The Engine of Marine Life
**Why it Matters:** Winds, currents, and eddies determine where nutrients and plankton are transported. Wind is the primary driver of upwelling, a phenomenon where cold, nutrient-rich deep water rises to the surface, causing an explosion of phytoplankton and fueling the entire food chain.
**NASA Data Used:** We utilize datasets like the "MetOp-A ASCAT Level 2 Ocean Surface Wind Vectors" to get the speed and direction of ocean winds. Analyzing these vectors allows us to predict the occurrence of upwelling.

### 🔗 The Final Synthesis: Connecting the Dots
Our model integrates these pillars to understand the *why* behind a prediction:

    Winds (ASCAT) ➡️ predict Upwelling
    Upwelling ➡️ brings Nutrients to the surface
    Nutrients + Sunlight ➡️ trigger Phytoplankton blooms (Chlorophyll-a / MODIS)
    Phytoplankton ➡️ attracts the Food Chain (zooplankton, fish)
    Thermal Fronts (SST / MODIS & VIIRS) ➡️ concentrate the Prey
    Concentrated Prey + Thermal Comfort Zones ➡️ Attract Sharks 🦈🎯

---

### Key Technologies
- **Analysis & Modeling:** Python (Pandas, Matplotlib, NumPy, xarray)
- **Environment Management:** MiniConda
- **Prototyping:** Jupyter Notebook
- **AI Assistants:** Google Gemini, Manus AI, Claude AI, ChatGPT

### Data Sources
- **NASA Earthdata:** MODIS, VIIRS, ASCAT
- **Copernicus Marine Service:** (for parameters like depth/physics)
- **Hycom:** (for ocean current modeling)
- **CSIRO:** (for additional marine data)

### Next Steps & Future Improvements
The current prototype focuses its predictive power on marine environments. A key next step for development is implementing a land mask (geospatial filter) to automatically handle and reject terrestrial coordinates, further refining the user input process.

### Our Team
- Rafael Silva Nascimento
- Caio Artiaga Gondim
- Erick Henrique de Oliveira Medeiros
- Henrique Miranda Chaves
- Bruno Henrique Leão
- Eduardo Silva Oliveira
