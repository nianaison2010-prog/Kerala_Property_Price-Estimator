# Kerala_Property_Price-Estimator
# 🏡 Kerala House Price Predictor

An end-to-end multi-variable machine learning web application built to predict house prices across premium residential markets in Kerala, India. This project features a **Linear Regression** backend engine paired with a self-contained **Flask web interface** optimized to run entirely in a single file on mobile environments like **Pydroid 3**.

---

## 🚀 Features

*   **Regional Pricing Multipliers**: Tracks localized market fluctuations for top Kerala real estate nodes: **Kochi**, **Thiruvananthapuram**, **Kozhikode**, **Thrissur**, and **Kottayam**.
*   **Property Type Variations**: Dynamically scales valuations for different structural blueprints including **Apartments / Flats**, **Independent Villas**, and **Traditional Kerala Houses**.
*   **Structural Input Parameters**: Processes exact metrics including **Built-up Area (Sq. Ft.)**, layout scales (**BHK / Bedrooms**), and total **Bathrooms**.
*   **Automated Categorical Data Pipelines**: Implements native **One-Hot Encoding** (`pd.get_dummies`) to translate string names into numerical vectors readable by the machine learning algorithm.
*   **Localized Formatting Engine**: Formats the predicted values dynamically using the **Indian Currency System (Lakhs and Crores)** alongside the **₹** symbol.
*   **Pydroid 3 Optimized**: Built to run out-of-the-box on Android devices with dynamically self-generating synthetic market distributions.

---

## 🛠️ Tech Stack & Prerequisites

*   **Language**: Python 3
*   **Framework**: Flask
*   **Machine Learning**: Scikit-Learn (Linear Regression model)
*   **Data Processing**: Pandas, NumPy

---

## 📦 Installation & Setup (Pydroid 3)

1. Open the sidebar navigation menu inside **Pydroid 3** on your Android device.
2. Select **Pip** -> **Quick Install** and ensure you install the following modules:
   * `flask`
   * `pandas`
   * `scikit-learn`
   * `numpy`
3. Create a new file named `app.py`, paste the source script into the editor, and tap the yellow **Play/Run** button.
4. Open your phone's web browser (e.g., Google Chrome) and go to:
   ```text
   http://127.0.0.1:5000
   ```

---

## 📊 Core Data Architecture & Logic

The engine establishes a baseline structure calculating real estate asset values through structural coefficients modified by combined locational and construction premiums:

$$\text{Structural Value} = \text{Base Price} + (\text{Sq.Ft.} \times 3500) + (\text{BHK} \times 200,000) + (\text{Bathrooms} \times 100,000)$$

$$\text{Final Prediction} = \text{Structural Value} \times \text{City Multiplier} \times \text{Property Type Multiplier}$$

---

## 📄 License

Licensed under the **Apache License, Version 2.0** (the "License"); you may not use this project except in compliance with the License. You may obtain a copy of the License at [Apache License 2.0](http://apache.org "Apache License 2.0").

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
