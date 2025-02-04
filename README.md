# File Downloader

A simple Tkinter-based GUI application that allows users to download files from a provided URL. The app displays a progress bar for each file being downloaded, showing the download percentage and size. It supports both finite and infinite content sizes.

## Features

- Add a download URL to start the download process.
- Displays download progress with percentage and file size.
- Supports both finite and infinite file sizes.
- Easy-to-use graphical interface built with Tkinter.
- Uses a separate thread for downloading to keep the UI responsive.

## Prerequisites

- Python 3.x
- Required Python libraries: `requests`, `Pillow`, `tkinter`, `re`, `os`, `threading`

You can install the required libraries using:

```bash
pip install requests pillow
```

## Installation

1. Clone the repository to your local machine:

```bash
git clone <repository-url>
```

2. Install the required Python packages:

```bash
pip install requests pillow
```

3. Make sure you have a file_icon.png image in the same directory as the script (this is used as the icon for each download item).
4. Run the script:

```bash
python downloader.py
```

## How It Works

- The user is prompted to enter a URL for the file they wish to download.
- Once a valid URL is provided, the download starts in a new thread.
- The app shows the file name, download progress, percentage, and size in a neat interface.
- The progress bar and download info are updated in real-time as the file is downloaded.
- If the file size is unknown (i.e., the server doesn't provide a Content-Length), the progress bar will work in indeterminate mode.

## Customization

- You can change the image used for the download icon by replacing file_icon.png with your preferred icon.
- To customize the look and feel, modify the Tkinter widget properties in the script.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
