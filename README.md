# **Machine Learning Approach to Extracting Entity Values from Images**

## **Project Overview**

This project demonstrates the use of **Optical Character Recognition (OCR)** and pattern recognition techniques (**Regex**) to extract key product attributes (like **weight, dimensions, voltage, and wattage**) from images. It was built to solve the challenge of extracting product details from e-commerce images, where textual descriptions may be missing or incomplete.

## **Table of Contents**
- [**Introduction**](#introduction)
- [**Dataset**](#dataset)
- [**Approach**](#approach)
- [**Technologies Used**](#technologies-used)
- [**Experiments**](#experiments)
- [**Results**](#results)
- [**Conclusion**](#conclusion)
- [**How to Run**](#how-to-run)

## **Introduction**

In e-commerce, having accurate product details such as **weight, voltage**, and **dimensions** is critical for tasks like inventory management and product listing. This project tackles the problem by extracting these values directly from product images, using a combination of **OCR** to capture text and **regex** for pattern recognition.

## **Dataset**

The dataset consists of product images accessed via URLs, containing attributes such as:
- **Weight** (e.g., "22 lbs", "10 kg")
- **Dimensions** (e.g., "10x12 inches", "30x50 cm")
- **Voltage** (e.g., "120V")
- **Wattage** (e.g., "60W")

Each image is processed to extract these attributes using **OCR** and **regex patterns**, followed by unit standardization.

## **Approach**

The project follows these key steps:

1. **Data Preprocessing**: The images are processed to extract textual information using **Tesseract OCR**.
2. **Pattern Recognition**: **Regular expressions** are used to detect and extract specific attribute values such as **weight** and **dimensions**.
3. **Unit Conversion**: Once values are extracted, they are converted into standardized units for consistency.

### **Key Components**:
- **Optical Character Recognition (OCR)**: **Tesseract** is used to extract text from product images.
- **Regex for Feature Extraction**: Regular expressions are employed to identify numeric patterns associated with product attributes like **weight, dimensions,** and **voltage**.

## **Technologies Used**
- **Python**: Used for scripting, data manipulation, and regex.
- **Tesseract OCR**: An open-source OCR engine used to extract text from product images.
- **Regular Expressions (Regex)**: For pattern-based extraction of product attributes.
- **Pandas**: For data manipulation.
- **Matplotlib**: For data visualization.

## **Experiments**

### **Image Preprocessing**
To improve the accuracy of text extraction using **OCR**, different image preprocessing techniques like changing **brightness** and **contrast** were applied.

### **Regex Optimization**
**Regex patterns** were refined iteratively to accurately identify product attributes such as **weight** and **dimensions** across a wide range of formats (e.g., "10x12 in", "22 lbs"). Flexibility was added to handle variations and edge cases.

## **Results**

The solution achieved high accuracy in extracting relevant attributes such as **weight, voltage**, and **dimensions** from product images. The combination of **OCR** and **regex-based pattern recognition** was found to be effective for structured data extraction.

- **Accuracy**: Approximately **85% accuracy** was achieved for correctly extracting key attributes across diverse product images.
- **Performance**: The system performs efficiently even with large datasets, making it suitable for real-time applications.

## **Conclusion**

This project successfully demonstrated how **OCR** and **regex** can be applied to extract structured data from product images. The system efficiently extracts and standardizes values like **weight, voltage**, and **dimensions**, which are critical in e-commerce. The solution is robust and can be adapted for various product categories.

## **How to Run**

1. Clone the repository:
   ```bash
   git clone https://github.com/Mukunj-21/Image-Entity-Extractor.git
   cd Image-Entity-Extractor
2. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Image Entity Extractor.ipynb


