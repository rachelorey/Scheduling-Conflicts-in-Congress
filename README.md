# Scheduling Conflicts in Congress

This repository contains code and data related to the Bipartisan Policy Center's research on scheduling conflicts within Congress. The project focuses on identifying conflicts in committee schedules for members of the U.S. House of Representatives.

## Project Structure

- **Scheduling - Conflicts Data Pull V2.ipynb**: Collects hearing data from `docs.house.gov` and committee assignments from `clerk.house.gov`. It then identifies scheduling conflicts.
- **Scheduling - Results Analysis.ipynb**: Analyzes the collected data to aggregate and present results.
- **Folder Structure**:
  - Each Congress (113th through 118th) is organized into its own folder, containing relevant data files and analysis specific to that Congress. Data has been collected through July 31, 2024, about halfway through the second session of the 118th Congress.
  - A separate folder is dedicated to cross-congress analysis, allowing for a broader examination of scheduling conflicts over multiple Congresses.

## Notes

Due to rate limiting on government websites, the data collection process may take several hours.

## Usage

To run the analysis quickly, pre-loaded CSV files from the initial data collection are used in the analysis notebook.

## Requirements

- Jupyter Notebook
- Python 3.x
- Required libraries (e.g., pandas, requests)

## Methodology

### Data Collection
The data for this project was collected from two primary sources:
- **Hearing Data**: Retrieved from `docs.house.gov`, which provides information on scheduled congressional hearings.
- **Committee Assignments**: Extracted from `clerk.house.gov`, detailing the committee assignments for each member of the U.S. House of Representatives.

### Identifying Conflicts
Scheduling conflicts were identified by cross-referencing the hearing schedules with the committee assignments. If a member was scheduled to attend two or more hearings simultaneously, a conflict was recorded.

### Analysis
The collected data was then processed to quantify the number of conflicts per member and committee, allowing for analysis of trends and patterns in scheduling conflicts within Congress.
