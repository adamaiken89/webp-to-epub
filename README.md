# webp_to_epub

This project converts a folder of `.webp` images into an EPUB file using Python.

- [webp\_to\_epub](#webp_to_epub)
  - [Requirements](#requirements)
  - [Setup](#setup)
  - [Usage](#usage)
  - [Notes](#notes)
  - [Output](#output)

## Requirements

- Python 3.8+
- [Homebrew](https://brew.sh/) (for macOS, to install Tkinter if needed)

## Setup

1. **Clone or download this repository.**
2. **Open a terminal in the project directory.**
3. **Create a Python virtual environment:**

   ```sh
   python3 -m venv epubenv
   ```

4. **Activate the virtual environment:**

   ```sh
   source epubenv/bin/activate
   ```

5. **Upgrade pip and install dependencies:**

   ```sh
   python -m pip install --upgrade pip setuptools wheel
   pip install ebooklib pillow
   ```

6. **(macOS only, if you see Tkinter errors):**

   ```sh
   brew install python-tk
   ```

## Usage

1. **Activate the virtual environment (if not already active):**

   ```sh
   source epubenv/bin/activate
   ```

2. **Run the script:**

   ```sh
   python webp_to_epub.py
   ```

3. **A folder selection dialog will appear.**
   - Select the folder containing your `.webp` images.
   - The script will generate an EPUB file in the current directory, named after the selected folder.

## Notes

- The script requires a GUI for the folder selection dialog (Tkinter).
- If you want to run the script without a GUI, you can modify it to hardcode the image directory or accept a command-line argument.

## Output

- The generated EPUB file will be named `<selected_folder>.epub` and saved in the current directory.

---

If you encounter any issues, please ensure all dependencies are installed and your Python version is compatible.
