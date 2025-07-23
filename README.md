# Ransomware Detection and Prevention System using AI and ML

![Modern University for Technology & Information Logo]([https://i.imgur.com/vHq4g7x.png](https://elearning.mti.edu.eg/assets/2.png))

A cutting-edge cybersecurity solution developed as a graduation project for the Faculty of Computers & Artificial Intelligence at Modern University for Technology & Information. This project presents an advanced Ransomware Detection and Prevention System (RDPS) that implements a comprehensive, two-pronged defense strategy using Artificial Intelligence (AI) and Machine Learning (ML) to identify and combat malicious activity across network and host levels.

## Table of Contents
- [Abstract](#abstract)
- [Key-Features](#key-features)
- [System-Architecture](#system-architecture)
- [How-To-Use](#how-to-use)
- [Technology-Stack](#technology-stack)
- [Evaluation-Highlights](#evaluation-highlights)
- [The-Team](#the-team)
- [Acknowledgments](#acknowledgments)

## Abstract

Ransomware has emerged as a critical cybersecurity threat, causing severe financial and data losses while rendering traditional signature-based security solutions increasingly ineffective against its rapidly evolving variants. This project introduces an advanced Ransomware Detection and Prevention System (RDPS) that leverages a comprehensive, two-pronged defense strategy. [1] It uses Artificial Intelligence (AI) to identify malicious activity at both the network and host levels. The system features an online, network-based model for real-time threat identification by analyzing network traffic, and an offline, host-based model that provides pre-execution analysis of suspicious executable files.

## Key Features

- **Multi-Layered Detection Architecture**: A comprehensive approach combining static analysis, dynamic analysis, and network traffic analysis for robust detection.
- **Machine Learning Integration**: Utilizes advanced ML algorithms like Random Forest, XGBoost, SVM, and KNN to identify ransomware patterns missed by traditional systems.
- **Deep Learning Enhancement**: Implements CNN and RNN to detect complex patterns in ransomware behavior and network traffic.
- **Real-Time Monitoring**: Provides continuous monitoring and real-time threat detection for immediate response to ransomware activities.
- **Adaptive Learning**: Incorporates continuous learning capabilities, allowing the system to adapt to new ransomware variants automatically.
- **User-Friendly Dashboard**: An intuitive, web-based dashboard built with HTML, CSS, and JavaScript, providing real-time threat monitoring, alert visualization, and system management.

## System Architecture

The RDPS operates on a hybrid, defense-in-depth security model that combines proactive network-level defense with robust host-level protection.

1.  **Online Model (Network-Based Detection)**: This component acts as the first line of defense, analyzing real-time network traffic to identify threats before they reach the host machine.
2.  **Offline Model (Host-Based Detection)**: Operating on the endpoint, this model provides a second layer of defense by continuously monitoring the file system and performing scans to detect malicious files that may have bypassed the online model.

![System Architecture Diagram](https://i.imgur.com/rN1fBft.png)

## How To Use

To get the RDPS up and running, follow these steps:

### Prerequisites

*   **Operating System**: Windows 10/11
*   **Python**: Version 3.9 or higher
*   **Web Browser**: A modern browser like Chrome, Firefox, or Edge.
*   **Core Python Libraries**: `Flask`, `scikit-learn`, `pandas`, `numpy`, `xgboost`, `joblib`, `pefile`, `psutil`. Install them using the `requirements.txt` file.
*   **Java Development Kit (JDK)**: Version 8 or higher.

### Installation & Setup

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/ransomware-detection-system.git
    cd ransomware-detection-system
    ```
2.  **Install dependencies:**
    ```sh
    pip install -r requirements.txt
    ```
3.  **Setup CICFlowMeter** for the online model by downloading it from its [official repository](https://github.com/ahlashkari/CICFlowMeter).
4.  **Run the application:**
    ```sh
    python backend.py
    ```
    *Note: To enable the firewall prevention feature, you must run the script with administrative privileges.*
5.  **Access the Dashboard** by navigating to `http://127.0.0.1:5000` in your web browser.

## Technology Stack

- **Backend**: Python, Flask
- **Machine Learning**: Scikit-learn, XGBoost
- **Deep Learning**: TensorFlow, Keras
- **Frontend**: HTML, CSS, JavaScript
- **Network Analysis**: CICFlowMeter
- **Real-time Monitoring**: Watchdog

## Evaluation Highlights

The system underwent rigorous testing using real-world ransomware datasets and specialized simulations, demonstrating high detection accuracy and low false-positive rates.

-   The **XGBoost** model was selected for the online detection system, achieving a **100% accuracy** and a **1.00 F1-Score** on the test dataset.
-   The offline model, utilizing a **Random Forest** classifier, effectively detected and neutralized simulated ransomware attacks from the **RanSim** tool in real-time.

![Dashboard During Live Analysis](https://i.imgur.com/cR7LKYc.png)

## The Team

This project was submitted by:
- Esraa Salah Hassan Ahmed Shalan
- Nour Mohamed Morshed El-Shafie Nasr
- Ahmed Abd El-Aziz Ali Abd El-Aziz El-Sadany
- Ahmed Bassam Refaat Gaafar Ali
- Ahmed Ibrahim El-Sayed Ahmed Abdullah
- Abdullah Alaa Moukhtar Mohamed
- Mohamed Ahmed Yousef Salama
- Abdullah Anas Abdullah El-Gamal

### Supervised by:
- Prof. Dr. Hafez Abd El-Wahab
- Dr. Tarek Soliman
- T.A Ghada Nady
- T.A. Gerges Mourad

## Acknowledgments

We extend our deepest gratitude to Modern University for Technology and Information (M.T.I.) for providing an excellent learning environment. A special thanks to our project supervisors for their invaluable guidance and support. We are also deeply grateful to the leadership and faculty of MTI for their dedication, and to our families for their unwavering encouragement.
