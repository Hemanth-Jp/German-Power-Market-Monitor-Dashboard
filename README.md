# German Power Market Monitor Dashboard

## Project Overview
This interactive dashboard visualizes German energy market data, providing insights into actual power generation and day-ahead electricity prices. The dashboard features two main components:
1. Energy Generation Visualization: Shows actual generation data across different power sources
2. Day-ahead Price Analysis: Displays electricity prices for Germany and neighboring countries

### Key Features
- Interactive date range selection
- Real-time data filtering
- Multi-source energy generation tracking
- Cross-border price comparison
- Summary statistics and analysis
- Responsive design

## Prerequisites
- Python 3.8 or higher
- Jupyter Notebook
- Web browser (Chrome, Firefox, or Safari recommended)
- Basic understanding of Python and data analysis

## Installation

### Setting up the Environment
1. Open your terminal or command prompt
2. Create and activate a new virtual environment (recommended):
```bash
# Using venv
python -m venv energy_dashboard_env
source energy_dashboard_env/bin/activate  # On Windows use: energy_dashboard_env\Scripts\activate
```

### Installing Required Packages
Run the following command to install all necessary packages:
```bash
pip install dash pandas plotly numpy jupyter notebook
```

## Project Structure
```
project_root/
│
├── data/
│   ├── Actual_generation_202411010000_202412010000_Day.csv
│   └── Day-ahead_prices_202411010000_202412010000_Day.csv
│
├── notebooks/
│   └── energy_dashboard.ipynb
│
└── README.md
```

## Getting Started

### Running the Dashboard from Jupyter Notebook

1. Launch Jupyter Notebook:
```bash
jupyter notebook
```

2. Navigate to the notebook directory and open `energy_dashboard.ipynb`

3. Ensure your data files are in the correct location relative to the notebook

4. Execute all cells in the notebook:
   - Use Shift + Enter to run cells individually
   - Or use the "Run All" button from the Cell menu

5. The dashboard will launch automatically and can be accessed via your web browser

### Accessing the Dashboard

Once running, the dashboard can be accessed in two ways:

1. Local Access:
   - Open your web browser
   - Navigate to: `http://127.0.0.1:8050`

2. Network Access (within your local network):
   - Find your computer's IP address
     - Windows: Use `ipconfig` in command prompt
     - Mac/Linux: Use `ifconfig` in terminal
   - Access via: `http://[your-ip-address]:8050`

## Using the Dashboard

### Navigation
- The dashboard consists of two main tabs:
  1. **Actual Energy Generation**
  2. **Day-ahead Energy Prices**

### Energy Generation Tab

#### Features:
- Date range selector
- Energy source selection via checkboxes
- Stacked area chart visualization
- Generation summary statistics

#### How to Use:
1. Select your desired date range
2. Choose energy sources to display
3. Hover over the chart for detailed values
4. View summary statistics below the chart

### Price Analysis Tab

#### Features:
- Date range selector
- Country/region selector (multi-select)
- Step-line chart visualization
- Price statistics and comparisons

#### How to Use:
1. Select your desired date range
2. Choose countries/regions to compare
3. Hover over the chart for exact prices
4. View price statistics below the chart

## Data Description

### Generation Data File
- Format: CSV with semicolon (;) separator
- Time resolution: Daily
- Energy sources included:
  - Biomass
  - Hydropower
  - Wind (offshore/onshore)
  - Photovoltaics
  - Nuclear
  - Conventional sources (coal, gas, etc.)
- Units: MWh (Megawatt hours)

### Price Data File
- Format: CSV with semicolon (;) separator
- Time resolution: Daily
- Coverage: Germany and neighboring countries
- Units: €/MWh (Euros per Megawatt hour)

## Troubleshooting

### Common Issues and Solutions

1. **Dashboard Not Loading**
   - Check if all required packages are installed
   - Verify the correct port (8050) is available
   - Ensure no other Dash applications are running

2. **Data Not Displaying**
   - Verify data file locations
   - Check file permissions
   - Ensure correct file format and encoding

3. **Browser Connection Issues**
   - Try a different browser
   - Check network connection
   - Verify firewall settings

## Additional Information

### Performance Optimization
- The dashboard is optimized for datasets up to 1 year
- For larger datasets, consider implementing data aggregation
- Browser caching is enabled for better performance

### Browser Compatibility
- Fully tested on:
  - Chrome (recommended)
  - Firefox
  - Safari
- May have limited functionality on IE/Edge

### Best Practices
- Regular data updates for accurate analysis
- Clear browser cache if visualizations appear incorrect
- Use date filters to focus on specific time periods

## Support and Contact
For technical support or questions, please contact:
[hemanth.jadiswami.prabhakaran@stud.hs-emden-leer.de / manoj.kumar.prabhakaran@stud.hs-emden-leer.de]

## Version History
- v1.0 (29 Jan 2024): Initial release
  - Basic visualization features
  - Data import functionality
  - Interactive filtering


