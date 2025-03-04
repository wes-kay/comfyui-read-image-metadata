# comfyui-read-image-metadata
Python script that extracts and displays metadata embedded in PNG files generated by ComfyUI. The script reads metadata stored in standard PNG text chunks (tEXt, zTXt, and iTXt) and prints it in a structured JSON format.


# Read ComfyUI Metadata

## Description

`main.py` is a Python script that extracts and displays metadata embedded in PNG files generated by ComfyUI. The script reads metadata stored in standard PNG text chunks (`tEXt`, `zTXt`, and `iTXt`) and prints it in a structured JSON format.

## Features

- Extracts metadata from ComfyUI-generated PNG files and prints to console
- Supports standard PNG text chunks (`tEXt`, `zTXt`, `iTXt`)
- Outputs metadata in readable JSON format
- Command-line interface using `argparse`

## Requirements

- Python 3.7+
- `pypng` library

Install dependencies using:

```sh
pip install pypng
```

or

```sh
pip install -r requirements.txt
```

## Usage

Run the script with the path to the PNG file:

```sh
python main.py path/to/image.png
```

## Example Output

```json
{
    "ComfyUI_Metadata": "{\"workflow\": \"example\", \"parameters\": {\"steps\": 50}}"
}
```