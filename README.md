# 🧪 Surface Roughness Drag & Flight Consistency Simulator

An interactive simulation tool I built in Google Colab using **Gradio**, **NumPy**, and **Matplotlib** to model controlled surface roughness on an aerodynamic body/model and document how it changes drag force and flight consistency.

## ✨ Key Features
- **Controlled Roughness Levels:** Compare *Smooth Finish*, *Light Roughness*, *Moderate Roughness*, and *Heavy Roughness* via equivalent roughness height ($k_s$) and non-dimensional ratio ($k_s / L_{\text{ref}}$).
- **Drag vs. Airspeed Analysis:** Evaluates how higher surface roughness increases effective drag coefficient ($C_D$) and drag force ($F_D$) across airspeeds.
- **Flight Consistency Simulation:** Runs Monte Carlo trials to show how roughness-driven variability widens range spread (standard deviation) and affects consistency.
- **Documentation-Ready Summary:** Generates side-by-side plots and a structured markdown summary ready to copy into notes or reports.

## 🛠️ Tech Stack
- **Environment:** Google Colab (no surface prep hardware or desktop simulation software required)
- **Simulation & UI:** Python, Gradio, NumPy, Matplotlib

## ⚙️ How to Run the Project
1. **Open in Google Colab:**
   - Upload `surface-roughness-drag-consistency.ipynb` to Google Colab (`colab.research.google.com`).
2. **Run & Launch the App:**
   - Run the cell; Gradio will install `gradio`, `matplotlib`, and `numpy` and open the interactive dashboard directly below it (plus a temporary `gradio.live` link if needed).
3. **Test & Document:**
   - Select roughness levels, tune reference length, area, speed, or trial scatter, click **Run Roughness Study**, and use the generated summary to document your findings.

## 📌 Scope & Assumptions
- Designed for **conceptual aerodynamic trade-offs and structured documentation**, not high-resolution boundary-layer CFD or certified flight testing.
- Uses roughness-scaled drag increments and Gaussian trial perturbations to represent drag penalties and consistency loss.
