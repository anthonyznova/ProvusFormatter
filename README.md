# Provus Formatter

This tool streamlines the process of preparing TEM/PEM data files for import to provus by automatically generating appropriate waveform and channel sampling scheme files, adding the appropriate flags to file header, updating project file. 


## Disclaimer

This tool is provided to assist with data formatting. Users are responsible for verifying the accuracy and appropriateness of the generated waveform and sampling files for their specific data and requirements. Always maintain backups of original data files.


## Installation

### Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

### Dependencies

The following packages will be automatically installed:

- PyQt5 >= 5.15.0
- PyQtChart >= 5.15.0
- numpy >= 1.19.0
- pandas >= 1.3.0

### Install from Source

1. Clone the repository:
    git clone https://github.com/anthonyznova/ProvusFormatter.git

    cd provus-formatter

2. Install in development mode:
    pip install -e .

## Usage

### Launch the Application

If you installed from source, run the formatter using:
    provus-formatter

Otherwise doubleclick the .exe

### Basic Workflow

1. **File Selection**
   - Drag and drop TEM/PEM files into the application
   - Set the root directory for output files

2. **Review waveform and sampling**
   - Review detected parameters in the analysis table
   - Modify waveform and sampling scheme assignments if needed
   - Preview and edit waveform shapes by double clicking anywhere in row
   - Select appropriate data styles for each file

3. **File Generation**
   - Click "Update Headers" to write waveform and sampling information to data files
   - Click "Update Project File" to create/update the Provus project file


## License

This project is licensed under the MIT License - see the LICENSE file for details.
