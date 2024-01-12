

```bash
# Handwritten Recognition

## Note:
1. Run `app.py` to open the canvas, draw your image, download the drawn image, and then convert it to text by uploading the image and generating speech.
2. Run `app2.py` to generate speech directly from the drawn canvas without downloading the image.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/InnoTech-Titans/HandScribeVoice.git
   cd HandScribeVoice
   ```

2. Create a Virtual Environment:
   ```bash
   python -m venv your_env_name
   your_env_name/Scripts/activate
   pip install -r requirements.txt
   ```

3. Download the Tesseract Bin File from the following link:
   - [Tesseract Bin File](https://github.com/UB-Mannheim/tesseract/wiki)

   Remember the path when setting up the Tesseract application.

   Install the `pytesseract` library:
   ```bash
   pip install pytesseract
   ```

   Make sure to add the following command in your script:
   ```python
   pytesseract.pytesseract.tesseract_cmd = r'C:\Users\USER\AppData\Local\Tesseract-OCR\tesseract.exe'
   ```

   Note: Your path may vary; choose the correct path.

4. Run the command:
   ```bash
   streamlit run app.py  # or app2.py according to your needs
   ```
