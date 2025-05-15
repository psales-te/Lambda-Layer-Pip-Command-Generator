# Lambda Layer Pip Command Generator

This is a lightweight tool that can help you generate `pip install` commands compatible with AWS Lambda Layer deployment. It allows you to customize the Python version, target folder, and packages, with optional support for generating individual pip commands per package.

The generated `pip install` command contains the basic options to generate the Lambda Layer. Feel free to add more options to this output!

## Features

- 🎯 Select Python version (from 3.9 to 3.13)
- 📦 Add multiple packages (comma-separated)
- 📁 Customize the pip `--target` installation folder
- 🔀 Toggle to generate a separate pip command per package
- 📋 Copy the generated pip command to your clipboard
- 🧼 Simple, responsive interface powered by Bootstrap

## How to Use

1. Open the `index.html` file in any modern browser (or just use the [Github Page](https://psales-te.github.io/pip-command-generator-python-lambda-layer/)).
2. Choose your desired **Python version**.
3. Enter one or more **package names** (comma-separated).
4. Set a **target folder** or use the provided default buttons.
5. (Optional) Check the box to generate individual pip commands for each package.
6. Click **Generate** to produce your pip install command.
7. Click **Copy to Clipboard** to use it in your terminal or deployment script.

## Example Output

```bash
pip install openpyxl pandas --platform manylinux2014_x86_64 --target=lambda-layer/python/lib/python3.10/site-packages --python-version 3.10 --only-binary=:all:
