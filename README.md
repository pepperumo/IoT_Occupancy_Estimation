[![LinkedIn][linkedin-shield]][linkedin-url]

# IoT Occupancy Estimation

This repository contains the implementation of an IoT-based occupancy estimation system. Using advanced data preprocessing techniques and machine learning models, it aims to estimate occupancy in real-time based on environmental sensor data. The primary focus is to improve the accuracy and efficiency of predictions, making it suitable for smart building applications.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Repository Structure](#repository-structure)
- [Data](#data)
- [Modeling](#modeling)
- [Contributing](#contributing)
- [License](#license)

## Features

- Preprocessing of environmental sensor data (e.g., temperature, humidity, light).
- Implementation of advanced machine learning algorithms, including XGBoost.
- Tools for feature engineering and model evaluation.
- Real-time prediction capabilities.
- Modular and extensible codebase.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/pepperumo/IoT_Occupancy_Estimation.git
   ```

2. Navigate to the project directory:
   ```bash
   cd IoT_Occupancy_Estimation
   ```

3. Create a new conda environment:
   ```bash
   conda create --name iot_occupancy_env python=3.10
   conda activate iot_occupancy_env
   ```

4. Install the required dependencies:
   ```bash
   conda env update --file conda_environment_requirements.yml
   ```

## Usage

1. Prepare the dataset by placing it in the `data/` directory.

2. Open the Jupyter notebook for preprocessing and training:
   ```bash
   jupyter notebook notebooks/Preprocessing_and_XGBoost.ipynb
   ```

3. Follow the steps in the notebook to preprocess the data, train the model, and evaluate it.

4. The trained model is saved as `models/xgboost_model.pkl` and can be used for predictions.

## Repository Structure

```plaintext
IoT_Occupancy_Estimation/
├── data/
│   └── Occupancy_Estimation.csv    # Dataset used for training and evaluation
├── models/
│   └── xgboost_model.pkl           # Trained XGBoost model
├── notebooks/
│   └── Preprocessing_and_XGBoost.ipynb  # Jupyter notebook for preprocessing and modeling
├── conda_environment_requirements.yml   # Conda environment configuration file
├── requirements.txt               # Additional Python dependencies
├── README.md                      # Project documentation
└── LICENSE                        # License information
```

## Data

The dataset used for this project includes:
- Environmental features such as temperature, PIR, and light intensity.
- Occupancy labels indicating whether a room is occupied or not.

Ensure the dataset is properly formatted and placed in the `data/` directory.

## Modeling

The primary model used for occupancy estimation is **XGBoost**. The pipeline includes:

- Feature engineering
- Model training
- Hyperparameter optimization
- Evaluation metrics (accuracy, precision, recall, F1-score)

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push your changes:
   ```bash
   git push origin feature-name
   ```
5. Create a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

<!-- MARKDOWN LINKS & IMAGES -->
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/giuseppe-rumore-b2599961
