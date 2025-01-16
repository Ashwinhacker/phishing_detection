# phishing_detection

# Phishing URL Detection Tool**

## Abstract

Phishing attacks are a significant cybersecurity threat, targeting unsuspecting users by tricking them into visiting malicious websites. This project introduces a machine learning-based phishing URL detection tool designed to identify and classify URLs as phishing or legitimate. It employs a **Random Forest Classifier** for classification, providing a high accuracy rate in detecting phishing URLs. The tool is enhanced with a user-friendly **Graphical User Interface (GUI)** built using **Tkinter**, enabling real-time predictions.



## objectives**

1. **To develop an effective machine learning model**  capable of accurately distinguishing between phishing and legitimate URLs.
2. **To create a user-friendly GUI** that simplifies the phishing URL detection process for non-technical users.
3. **To integrate basic animations** in the GUI for an enhanced user experience.
4. **To provide a lightweight and portable solution** for phishing detection that can be easily deployed on various systems.



## System Architecture

1. Input : User provides a URL via the GUI.
2. Processing :
   - The input URL is preprocessed and converted into numerical features.
   - The **Random Forest Classifier** processes these features to classify the URL.
3. **Output**: The tool predicts and displays whether the URL is phishing or legitimate.



## Key Components**

### 1. Machine Learning Model
- Algorithm : Random Forest Classifier.
- Dataset : A curated dataset of phishing and legitimate URLs.
- Features : Extracted from URLs, including:
  - Presence of special characters (e.g., `@`, `//`).
  - URL length.
  - Domain name characteristics.
  - HTTPS usage.
  - Suspicious patterns (e.g., IP addresses instead of domain names).
-  Training :
  - Dataset split into training and testing sets.
  - Model trained using labeled data to identify patterns indicative of phishing.
  - Performance metrics: Accuracy, precision, recall, and F1-score.

###  2. GUI Interface
- Built using **Tkinter**, offering a simple text input field and a "Predict" button.
- Displays results in real-time, with animations for visual feedback.

### 3. Basic Animation
- Visual effects added to enhance user engagement during the prediction process.

---

##  Installation

###  Step 1: Clone the Repository
```bash
git clone https://github.com/PERARASU10/Brainwave_matrix_intern.git
cd phishing-url-detection
```

###  Step 2: Install Dependencies
Ensure Python 3.6+ is installed. Use the following command to install required packages:
```bash
pip install pandas scikit-learn tkinter
```

### Step 3: Prepare the Dataset
- Ensure the dataset (CSV format) is in the project directory.
- Update the `file_path` variable in the `scanner.py` script with the dataset's file path.

### Step 4: Run the Tool
Start the GUI with:
```bash
python scanner.py
```

---

## Features

- **Real-Time Predictions**: Users can instantly determine if a URL is phishing.
- **User-Friendly Interface**: Simple and intuitive GUI.
- **Lightweight**: Minimal dependencies, making it easy to install and run.
- **Customizable**: Dataset and model can be updated to improve accuracy and adapt to new phishing techniques.



## Screenshots

### Interface Overview**
1.  Input Screen : Text field for URL entry.
2.  Output Screen : Displays the prediction results (Phishing or Legitimate).


##  Evaluation Metrics 

-  Accuracy : Proportion of correctly classified URLs.
-  Precision : Percentage of phishing predictions that are true.
-  Recall : Proportion of phishing URLs correctly identified.
-  1-Score : Harmonic mean of precision and recall.


## Challenges and Solutions

### 1. Feature Extraction
-  Challenge : Identifying meaningful URL features.
-  Solution : Leveraged domain knowledge and existing research to extract robust features.

###  2. Dataset Quality
-  Challenge : Ensuring the dataset's quality and representativeness.
-  Solution : Used a dataset with diverse examples of phishing and legitimate URLs.

###  3. GUI Responsiveness 
-  Challenge : Ensuring the GUI remains responsive during prediction.
-  Solution : Optimized the model and GUI code for faster execution.


##Future Enhancements

1.  Integration with Web Browsers : Develop browser extensions for real-time detection.
2.  Improved Machine Learning Models**: Experiment with deep learning techniques.
3.  Cloud-Based Deployment : Offer the tool as a web service.
4.  Enhanced Visualization : Add charts and graphs to display prediction confidence.



## Conclusion

The Phishing URL Detection Tool is a practical solution to a critical cybersecurity issue. By combining machine learning with a user-friendly interface, it empowers users to protect themselves against phishing attacks. The tool's modular design and extensibility make it an ideal foundation for further research and development.

