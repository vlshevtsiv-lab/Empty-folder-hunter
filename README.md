# Empty-folder-hunter

<img width="742" height="557" alt="Screenshot 2026-03-10 193814" src="https://github.com/user-attachments/assets/b57f7943-63d6-495a-a3ba-2789504b3c31" />

# Simple Empty Folder Hunter

Simple Empty Folder Hunter is a lightweight Python desktop application that scans a selected directory and finds all empty folders inside it. It provides an easy-to-use graphical interface that allows users to quickly identify and optionally delete empty directories.

The program is built with **Tkinter** and **CustomTkinter**, giving it a modern dark-themed UI while keeping the application simple and fast.

## Features

* 🔍 Scan any folder to detect empty subfolders
* 🧾 Display a list of all empty folders found
* 🗑️ Delete all detected empty folders with one click
* ⚠️ Confirmation prompt before deleting folders
* 🚫 Automatically ignores system folders such as:

  * `$RECYCLE.BIN`
  * `System Volume Information`
* 🌙 Modern dark-mode interface using CustomTkinter

## How It Works

1. The user selects a folder using the **Select Folder** button.
2. The application recursively scans the directory using `os.walk`.
3. Any folders that contain **no files and no subfolders** are considered empty.
4. The results are displayed in the main results panel.
5. The user can choose to remove all empty folders using the **clean all** button.

## Requirements

Python 3.8 or newer.

Install the required library:

```
pip install customtkinter
```

## How to Run

1. Download or clone the project.
2. Install dependencies.
3. Run the script:

```
python main.py
```

The application window will open, allowing you to select a folder and scan for empty directories.

## Project Structure

```
project-folder
│
├── main.py        # Main application script
└── README.md      # Project documentation
```

## Warning

Deleting folders is permanent. Always review the results before cleaning empty folders to avoid removing directories you might still need.

## License

This project is open-source and free to use.
