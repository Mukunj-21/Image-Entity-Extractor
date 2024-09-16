Machine Learning Approach to Extracting Entity Values from Images

Project Overview
This project demonstrates the extraction of key product attributes (such as weight, dimensions, voltage, and wattage) from images using Optical Character Recognition (OCR) and pattern recognition. This task is essential for e-commerce, where extracting accurate product information from images can be crucial for inventory management, quality control, and product listings.

Introduction
In e-commerce platforms, products often lack detailed textual descriptions, making it difficult to obtain crucial information like product dimensions or power ratings. This project aims to solve that problem by leveraging machine learning techniques, particularly OCR, to extract and structure information from product images.

Dataset
The dataset consists of product images sourced via URLs. The images typically contain product labels with attributes such as:
Weight (e.g., "22 lbs")
Dimensions (e.g., "15x10x5 inches")
Voltage (e.g., "120V")
Wattage (e.g., "60W")
Approach
The project follows these key steps:

Data Preprocessing: Extract text from images using OCR.
Pattern Recognition: Use regular expressions (regex) to identify relevant patterns for different attributes.
Standardization: Convert extracted values to a standardized format (e.g., converting lbs to kilograms).
Key Components:
Optical Character Recognition (OCR): We utilized Tesseract to extract text from images.
Regex for Feature Extraction: Regular expressions were used to identify and capture numeric values associated with product attributes such as weight and dimensions.
Technologies Used
Python: Programming language.
Tesseract OCR: To extract text from images.
Regular Expressions (Regex): For pattern matching and value extraction.
Pandas: Data manipulation and analysis.
Matplotlib: For visualization.
Experiments
We tested several image preprocessing techniques to improve OCR accuracy, including contrast and brightness adjustments. Regular expressions were fine-tuned through multiple iterations to handle diverse patterns and reduce errors introduced by OCR.

Challenges
OCR Errors: Inaccuracies caused by poor image quality or complex product labels.
Unit Inconsistencies: Handling different unit formats (e.g., pounds, kilograms) and converting them to a standard unit.
Handling Edge Cases: Some images lacked relevant information, or OCR failed to capture the text properly.
Future Improvements
Potential enhancements include:

Using deep learning models to improve OCR accuracy on complex and noisy images.
Implementing natural language processing (NLP) models to further refine extracted text.
Expanding the system to support a wider range of product attributes.
Conclusion
This project demonstrates the successful use of OCR and regex to extract entity values from product images. This approach is efficient for cases where textual descriptions are missing or incomplete. The system can be expanded to various applications such as automated product listing generation, inventory management, and quality control.

How to Run
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Run the Jupyter Notebook to execute the code:

bash
Copy code
jupyter notebook Amazon_ML_Challenge.ipynb
Follow the steps outlined in the notebook to preprocess the images, run OCR, and extract the values using regex.
