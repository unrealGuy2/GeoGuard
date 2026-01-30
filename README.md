#  GeoGuard: Physics-Informed Coastal Erosion Prediction

![Status](https://img.shields.io/badge/Status-Prototype_Ready-success)
![Hackathon](https://img.shields.io/badge/Hackathon-OdiseIA4Good_2026-blue)
![Tech](https://img.shields.io/badge/AI-Physics_Informed_Neural_Networks-orange)

**GeoGuard** is an AI system designed to protect vulnerable coastal communities in Africa from the devastating effects of erosion. Unlike traditional models that rely solely on historical data, GeoGuard utilizes **Physics-Informed Neural Networks (PINNs)** to learn the underlying dynamics of the coastline and predict future erosion patterns with high accuracy.

---

##  The Problem
**Lagos, Nigeria** is sinking.
* Coastal erosion destroys homes, displaces communities, and threatens critical infrastructure like the Eko Atlantic.
* Traditional satellite monitoring only shows *past* damage. It cannot accurately predict *future* structural failure.

##  The Solution
GeoGuard bridges the gap between **Computer Vision** and **Geophysics**.
1.  **Satellite Input:** We fetch real-time Sentinel-2 satellite imagery via Google Earth Engine.
2.  **Physics Integration:** We solve the **Diffusion Equation** ($\frac{\partial u}{\partial t} = D \nabla^2 u$) using a Deep Neural Network.
3.  **Future Simulation:** The model predicts how the coastline will shift in 5 years, allowing governments to take proactive action.

---

##  Tech Stack
* **Core AI:** PyTorch (Deep Learning), PINNs (Physics-Informed Neural Networks).
* **Data Source:** Google Earth Engine (Sentinel-2 Satellite Data).
* **Language:** Python 3.10+.
* **Infrastructure:** Google Colab .

---

## Results (Proof of Concept)
* **Location:** Victoria Island / Eko Atlantic Coastline.
* **Accuracy:** The PINN successfully converged with a loss rate of `< 1e-4`, effectively learning the erosion dynamics from sparse satellite data.
* **Projection:** The model simulates a 5-year erosion timeline, highlighting areas of "Integrity Loss" (Risk Zones).

---

##  How to Run
This project is built as an interactive **Jupyter Notebook**.

1.  Open the file `GeoGuard_Prototype.ipynb` in this repository.
2.  Click the "Open in Colab" badge (if available) or download and run locally.
3.  **Authentication:** The script requires a Google Earth Engine account.
    * *Note: Project ID configuration is handled within the script.*

---

##  Team
**AbdulSalam Sulaiman**
* Lead Engineer & Researcher.

---
*Built for the OdiseIA4Good 2026 Hackathon (Climate Change Category).*
