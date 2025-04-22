# 🧑‍🤝‍🧑 **Crowd Density Classification** 📊

Welcome to the **Crowd Density Classification** project! This project detects people in images using **YOLOv5** and classifies the density of crowds into three categories: **Low**, **Medium**, and **High**. After detection, we generate various visualizations like graphs and charts to analyze the results.

## 📁 **Contents**

- **`crowd_density_report.xlsx`** 📑: Excel file containing image filenames, detected people, and density classification.
- **`graphs/`** 📈: Folder with generated graphs for visualization.
- **`script.py`** 🐍: Python script for running YOLOv5 detection and generating density classifications.
- **`README.md`** 📄: This file!

## ⚙️ **Prerequisites**

Before getting started, you'll need the following:

- **Python 3.x** 🐍
- **PyTorch** (CUDA support if using GPU) 🖥️
- **YOLOv5** for object detection 🏞️
- **OpenCV** 🖼️
- **Pandas** 📊
- **Matplotlib**/ **Seaborn** 📉 (for generating plots)

### 💻 **Installation Steps**

1. **Clone the repository**:
    ```bash
    git clone https://github.com/shailisahu283/crowd-density-classification.git
    cd crowd-density-classification
    ```

2. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Download YOLOv5** and install additional requirements:
    ```bash
    git clone https://github.com/ultralytics/yolov5.git
    cd yolov5
    pip install -U -r requirements.txt
    ```

## 🖼️ **Dataset**

This project uses a set of images containing crowds. The images are in `.npy` format and can be loaded with Python’s **NumPy** library. The detection process uses **YOLOv5** to count the people in each image.

## 🚀 **Running the Project**

### 1. **Loading and Processing Images**:

The images are loaded using NumPy, and the **YOLOv5 model** is used to detect the people in each image. The results are saved in an Excel file (`crowd_density_report.xlsx`), with columns for the **image file name**, **detected people**, and **density classification**.

### 2. **Density Classification**:

After detecting the people in each image, we classify the density:
- **Low**: 0–10 people
- **Medium**: 11–25 people
- **High**: 26+ people

### 3. **Running YOLOv5 Detection**:

The script uses YOLOv5 to detect the number of people in each image. The number of detected people is then classified into one of the three categories.

### 4. **Generating Graphs**:

Graphs are generated to visualize the distribution of people detected across images and the density classifications.

### 5. **Run the Script**:
    ```bash
    python script.py
    ```

This will generate the **Excel report** and save the generated **graphs** in the `graphs/` folder.

## 📊 **Results and Graphs**

The following graphs will be generated:

1. **Bar Graph** for Detected People in Each Image 📉
    ![Bar Graph](graphs/bar_graph.png)
    
2. **Pie Chart** for Density Classification Distribution 🍰
    ![Pie Chart](graphs/pie_chart.png)

3. **Line Chart** for Trend of Detected People 🖥️
    ![Line Chart](graphs/line_chart.png)

4. **Histogram** for Distribution of Detected People 📚
    ![Histogram](graphs/histogram.png)

5. **Boxplot** for Spread of Detected People 📏
    ![Boxplot](graphs/boxplot.png)


## 🌐 **Run on Google Colab**

For an interactive and easy-to-use version of this project, you can run it directly on **Google Colab**! Just follow the link below to start working with the notebook.

[👉 Open in Google Colab](https://colab.research.google.com/drive/163LtK0AaMhFB0ZEZ0zTiVj7OOxdMarJ5?usp=sharing)

## 📥 **License**

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 🙏 **Acknowledgements**

- **YOLOv5** for object detection 🧠
- **Pandas** for managing the dataset 📊
- **Matplotlib** and **Seaborn** for creating the visualizations 📈

---

### 🎯 **Contributions**

Feel free to contribute! Open an issue or create a pull request to improve this project. I'm happy to collaborate! 😄
