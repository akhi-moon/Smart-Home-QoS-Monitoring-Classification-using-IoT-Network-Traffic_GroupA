# Smart Home QoS Monitoring & Classification using IoT Network Traffic

This project integrates a **Smart Home Network Simulation** (built in OMNeT++) with a **Machine Learning QoS Classifier** (built in Python/Scikit-Learn). 

The goal is to simulate realistic IoT traffic patterns (latency, jitter, packet loss) and use AI to predict the Quality of Service (Good, Moderate, or Poor) based on **3GPP Standards**.

## 📂 Project Structure

1.  **`smarthomenetwork.zip`**: 
    *   Contains the complete OMNeT++ Project.
    *   Includes: `Network.ned` (Topology), `Logic.cc` (Physics Engine), `omnetpp.ini` (Configuration), `IoTPacket.msg` (Blueprint for the packets) and the simulation results (`.vec` file).
    
2.  **`Smart_Home_QoS_Analysis.ipynb`**: 
    *   The Google Colab Notebook. 
    *   It handles Data Preprocessing, Model Training (Random Forest), and generates the final Performance Reports (Confusion Matrix, Stacked Bar Charts).

3.  **Dataset (Required for Training)**:
    *   This project uses the **IoT Network Traffic Dataset**.
    *   **Source:** [Kaggle - IoT Network Traffic Dataset](https://www.kaggle.com/datasets/programmer3/iot-network-traffic-dataset)

## 🚀 How to Run

### Step 1: The Simulation
1.  Download and unzip `smarthomenetwork.zip`.
2.  Import the folder into **OMNeT++**.
3.  Build the project and run the simulation in **Express Mode** to generate the `General-#0.vec` file.

### Step 2: The Analysis
1.  Open `Smart_Home_QoS_Analysis.ipynb` in Google Colab.
2.  Download the **IoT_Network_Data.csv** from the Kaggle link above.
3.  Upload the CSV file to Colab to train the model.
4.  Upload the `General-#0.vec` file from OMNeT++ to test the simulation.
5.  Run all cells to generate the QoS Visualizations.

## 📊 Technologies Used
*   **Simulation:** OMNeT++ 6.0
*   **Language:** C++ (Simulation Logic), Python (Data Analysis)
*   **Libraries:** Pandas, NumPy, Scikit-Learn, Seaborn, Matplotlib

## 👤➕👤➕👤Team Members
1. Akhi Moon Jahan **C223202**
2. Fayeza Afrah Hissan **C223206**
3. Israth Jahan Worthy **C223229**
