# PRad-II Logbook Entry Generator

A self-contained HTML tool for generating PRad-II shift log entries at Jefferson Lab.

## Features

- **Self-Contained**: Single HTML file with no external dependencies (except logo hosted on jlab.org)
- **Auto-Save**: Automatically saves your work to browser localStorage
- **Session Management**: Import previous entries or start fresh
- **PRad-Themed**: Dark theme using colors from the PRad logo
- **Comprehensive Fields**: 19-column run summary table with PRad-specific parameters

## Usage

1. Open `logbook_generator.html` in any modern web browser
2. Fill in the summary, shift log entries, and run data
3. Click "Generate HTML" to create formatted output
4. Copy the generated HTML and paste into the logbook

## Run Summary Fields

The run table includes the following 19 columns:
- Run Number, Start Time, Stop Time, Length
- Type, Target, Target Pressure, Target Cell Temp (336D)
- Target Chamber Pressure
- Collimator 1 Position, Collimator 2 Position, Veto Position
- Beam Current, Vacuum Tank (Torr), HyCal Temp
- Event Rate (kHz), Live Time
- DAQ Config, Comments

## Contact

Questions? Email [acschick@jlab.org](mailto:acschick@jlab.org)

## License

Created for the PRad-II experiment at Jefferson Lab.
