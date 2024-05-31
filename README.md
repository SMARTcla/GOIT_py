# File Organizer

## Overview

This Python script organizes files in a specified directory into subdirectories by their file type. It handles images, documents, audio files, videos, and archives by moving them into respective folders. Additionally, it renames files to ensure compatibility across different file systems and removes empty directories.

## Features

- **File Sorting**: Automatically sorts files into `images`, `documents`, `audio`, `video`, and `archives` folders based on their extensions.
- **Renaming**: Converts filenames into a consistent format to avoid issues with different file systems, especially useful for non-Latin characters.
- **Cleanup**: Removes empty directories after sorting, except for specified categories.
- **Archive Handling**: Unpacks archive files and moves them to the `archives` folder.

## Prerequisites

Before running this script, ensure that you have Python installed on your system. Additionally, you will need to install the `transliterate` package if it's not already installed:

```bash
pip install transliterate
```

## Usage

Modify the path variable in the script to point to the directory you want to organize:
```bash
path = "C:\\path_to_your_directory"
```

## Directory Structure

After running the script, your files will be organized into the following directory structure based on their types:

- **Images**: path\images
- **Documents**: path\documents
- **Audio**: path\audio
- **Video**: path\video
- **Archives**: path\archives

Each folder will contain files sorted from the specified directory. Unsupported file types will be left in their original location.

Supported File Extensions

- **Images**: .jpeg, .png, .jpg, .svg
- **Videos**: .avi, .mp4, .mov, .mkv
- **Documents**: .doc, .docx, .pdf, .txt, .xlsx, .pptx
- **Audio**: .mp3, .ogg, .wav, .amr
- **Archives**: .zip, .gz, .tar
