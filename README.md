# Magic a LoRA

Magic a LoRA is the evolution of LoRAHelpà, designed to manage and process files of various formats (text, PDF, Word, PPT, Excel, audio, video, etc.) and create subtitle (SRT) files from videos. It also supports customizable configuration and interface localization in multiple languages.

## Main Features

- Convert files of various formats (PDF, Word, PPT, etc.) to text.
- Extract and transcribe audio from videos.
- Create SRT files from videos.
- Customizable application configuration.
- Support for localization in multiple languages.
- Directory exploration and file management with various search options.

## Requirements

- Python 3.7 or higher
- The following Python libraries:
  - `os`
  - `json`
  - `logging`
  - `tkinter`
  - `datetime`
  - `threading`
  - `fitz` (PyMuPDF)
  - `pptx`
  - `moviepy.editor`
  - `speech_recognition`
  - `pydub`
  - `csv`
  - `ebooklib`
  - `bs4` (BeautifulSoup)
  - `xml.etree.ElementTree`
  - `zipfile`
  - `pandas`
  - `pytube`
  - `vlc`
  - `docx`
  - `re`
  - `difflib`
  - `tkinterdnd2`

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/magic-a-lora.git
    cd magic-a-lora
    ```

2. Create and activate a virtual environment:

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Start the application:

    ```bash
    python MagicALoRA.py
    ```

2. Use the graphical interface to interact with the application:
    - **Convert**: Convert files of various formats to text.
    - **Test SRT**: Test the creation of SRT files from videos.
    - **Create text file**: Create text files by exploring directories and processing found files.
    - **Create Json**: Create JSON files from processed text files using specified keywords.
    - **Setup**: Configure the application, set output directories, manage ignored directories, etc.

## Configuration

The application allows saving and loading configurations via JSON files. Use the "Setup" tab in the graphical interface to manage settings.

### Example Configuration File

    ```json
    {
        "directories": [
            "E:/AI/someDIRTOINCLUDE"
        ],
        "ignore_dirs": [
            "E:/AI/someDIRTOIGNORE"
        ],
        "output_path": "E:/LoRA/TXT",
        "json_output_path": "E:/LoRA/Json",
        "process_subfolders": true,
        "temp_dir": "E:/AI/pythonscript/temp",
        "limit_search": "No Limit",
        "keywords": [
            "Original file path",
            "File content",
            "Content \\d",
            "Article \\d"
        ],
        "widget_positions": {
            ".!notebook.!frame5.!listbox": {
                "x": 10,
                "y": 5
            },
            ".!notebook.!frame5.!button": {
                "x": 280,
                "y": 179
            },
            ".!notebook.!frame5.!button2": {
                "x": 269,
                "y": 215
            },
            ".!notebook.!frame5.!listbox2": {
                "x": 10,
                "y": 251
            },
            ".!notebook.!frame5.!button3": {
                "x": 261,
                "y": 425
            },
            ".!notebook.!frame5.!button4": {
                "x": 251,
                "y": 461
            },
            ".!notebook.!frame5.!label": {
                "x": 286,
                "y": 502
            },
            ".!notebook.!frame5.!button5": {
                "x": 275,
                "y": 538
            },
            ".!notebook.!frame5.!label2": {
                "x": 284,
                "y": 579
            },
            ".!notebook.!frame5.!button6": {
                "x": 272,
                "y": 615
            },
            ".!notebook.!frame5.!label3": {
                "x": 254,
                "y": 656
            },
            ".!notebook.!frame5.!button7": {
                "x": 266,
                "y": 692
            },
            ".!notebook.!frame5.!label4": {
                "x": 286,
                "y": 733
            },
            ".!notebook.!frame5.!combobox": {
                "x": 250,
                "y": 774
            },
            ".!notebook.!frame5.!checkbutton2": {
                "x": 258,
                "y": 810
            },
            ".!notebook.!frame5.!button8": {
                "x": 266,
                "y": 845
            },
            ".!notebook.!frame5.!button9": {
                "x": 265,
                "y": 881
            }
        }
    }
    ```


## Contributing

Contributions are welcome, including improvements to the code, bug fixes, and new features. To contribute, follow these steps:

1. Fork the project.
2. Create a branch for your feature (`git checkout -b feature/feature-name`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push the branch (`git push origin feature/feature-name`).
5. Open a pull request.

## License

This project is licensed under the GPL-3.0 License. See the `LICENSE` file for more details.
