#📄 PDF Print Enhancer
An open-source tool to automatically "scan" and enhance your PDF documents. It straightens pages, increases contrast, and cleans up backgrounds, making them perfect for printing or digital archiving.

**✨ Features**
Automatic Page Straightening: Detects the document within each page and corrects its perspective.

High-Contrast Output: Converts pages into a clean, black-and-white format, similar to a physical scanner.

User-Friendly Web Interface: Simple drag-and-drop UI powered by Gradio. No command-line skills needed.

Adjustable Quality: Control the output resolution (DPI) for a perfect balance between file size and quality.

In-Memory Processing: Fast and efficient, with no intermediate files saved to your disk.

**🚀 Getting Started**
Follow these steps to get the PDF Print Enhancer running on your local machine.

Prerequisites
You need to have Python 3.8 or newer installed on your system. You can download it from python.org.

1. Clone the Repository
   First, clone this repository to your local machine using Git:

git clone https://github.com/ItsSp00ky/pdf_enhancer.git
cd pdf-print-enhancer

(Replace your-username with your actual GitHub username.)

2. Create a Virtual Environment (Recommended)
   It's a good practice to create a virtual environment to keep dependencies isolated.

On macOS/Linux:

python3 -m venv venv
source venv/bin/activate

**On Windows:**

python -m venv venv
.\venv\Scripts\activate

3. Install Dependencies
   Install all the required Python libraries using the requirements.txt file.
```
pip install -r requirements.txt
```
### 💻 How to Use
Once the installation is complete, running the application is simple.

Run the pdf_enhancer.py script from your terminal:
```
python pdf_enhancer.py
```
Your terminal will display a local URL, usually ``` http://127.0.0.1:7860. ```

Open this URL in your web browser.

Drag and drop your PDF file into the upload box, adjust the DPI if needed, and click "Submit".

Once processing is complete, a download link for your enhanced PDF will appear.

**🤔 How It Works**
The tool follows a simple three-step process:

PDF to Images: The input PDF is converted into a series of high-resolution images, one for each page.

Image Processing: Each image is analyzed using OpenCV to find the four corners of the document. A perspective transform is applied to "straighten" the page. Finally, an adaptive threshold is used to create a clean, high-contrast binary image.

Images to PDF: The processed images are compiled back into a single, enhanced PDF file.

**🤝 Contributing**
This is an open-source project, and contributions of all kinds are welcome! Whether it's reporting a bug, suggesting a new feature, or submitting code, your help is greatly appreciated.

Feel free to check the issues page to see what needs attention or to open a new issue.

If you'd like to contribute code, please fork the repository and create a pull request:

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request

📜 License
Copyright 2025 Ahmed Gali

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
