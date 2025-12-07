# ASCII Art Video Player

This small Python script converts a video into ASCII art and plays it in the terminal.

**Repository path:** `assci-art`

## Prerequisites

- Python 3.8+ installed
- `pip` available
- A video file (for example `vid.mp4`) placed in the project folder or a path to any video file

## Install dependencies

From the project root (`assci-art`) install the required packages:

```powershell
python -m pip install -r requirements.txt
```

If you prefer to install manually:

```powershell
python -m pip install opencv-python
```

## Usage

Interactive mode:

```powershell
cd "C:\Users\h\Desktop\New folder\assci-art"
python index.py
# then when prompted enter the video path, terminal width (e.g. 80), and FPS (or 0 to use video FPS)
```

Non-interactive (pipe inputs) example (Windows PowerShell):

```powershell
# Provide the full video path, desired width, and fps (0 to use video FPS)
echo "C:\Users\h\Desktop\New folder\assci-art\vid.mp4`n80`n0" | python index.py
```

Notes:
- If you pass `0` for FPS the script will try to use the video's FPS. If the video FPS cannot be read, provide a positive integer.
- Use a smaller `width` for faster rendering or when your terminal is narrow.

## Troubleshooting

- ModuleNotFoundError: No module named 'cv2' — install dependencies (`pip install -r requirements.txt`).
- Can't open/read file — ensure the video path is correct and the file is accessible. Use an absolute path if needed.
- If the ASCII output looks squashed, try lowering the `width` value.

## Files

- `index.py`: main script to convert and play video as ASCII art
- `requirements.txt`: Python dependencies

## License

This repository does not include a license file by default. Add one if you plan to share or modify this project publicly.

---
Created README and instructions to run the ASCII-art video player.
# Arts
Ascii art
