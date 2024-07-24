Sure, here is a README for your GitHub repository:

---

# Data Recording and Plotting

This repository contains two Python scripts: one for recording data from a serial port and another for plotting the recorded data.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
  - [Recording Data](#recording-data)
  - [Plotting Data](#plotting-data)
- [License](#license)

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. Install the required Python packages:

   ```sh
   pip install -r requirements.txt
   ```

## Usage

### Recording Data

The script `record_data.py` is used to record data from a serial port and save it to an Excel file.

1. **Configure COM parameters:**  
   Open the `record_data.py` file and set the `serial_port` and `baud_rate` variables to match your serial port configuration.

   ```python
   serial_port = 'COM8'  # Replace with your serial port
   baud_rate = 115200    # Replace with your baud rate
   ```

2. **Input desired grip:**  
   Set the `grip` variable to your desired grip name.

   ```python
   grip = 'PointTripod'  # Replace with your desired grip
   ```

3. **Start the script:**  
   Run the script to start receiving and recording data.

   ```sh
   python record_data.py
   ```

4. **Save data:**  
   To save the recorded data, interrupt the script execution using `Ctrl + C`. The data will be saved to an Excel file named `<grip>_<timestamp>.xlsx`.

### Plotting Data

The `plot_data.py` script is used to plot the data recorded by `record_data.py`.

1. **Configure file path:**  
   Open the `plot_data.py` file and set the `file_path` variable to the path of the Excel file you want to plot.

   ```python
   file_path = 'PointTripod_07_23_12_34_56.xlsx'  # Replace with your file path
   ```

2. **Run the script:**  
   Run the script to generate the plot.

   ```sh
   python plot_data.py
   ```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to adjust any sections as needed!