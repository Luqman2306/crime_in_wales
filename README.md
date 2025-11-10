README – Crime in Wales Analysis Project


Overview


This project explores recorded crime data across the four Welsh police forces — South Wales, North Wales, Gwent, and Dyfed-Powys — over a 24-month period. 
The objective is to identify spatial, temporal, and categorical patterns in crime that can support data-driven decision-making for housing sales prioritisation, community safety planning, and local policy guidance.
The analysis was completed using Python in Jupyter Notebooks, executed within Visual Studio Code (VS Code). The project includes both data preprocessing and exploratory data analysis (EDA), with detailed written interpretation documented separately.


Project Structure


C:\
│
├── Police forces\
│   ├── Dyfed-Powys\
│   ├── Gwent\
│   ├── North Wales\
│   └── South Wales\
│       └── (Contains raw monthly and yearly CSV files)
│
└── Police forces preprocessing\
    ├── 01_data_preprocessing_police_forces.ipynb
    └── eda.ipynb






File Descriptions


File / Folder	Description


C:\Police forces	Folder containing all raw police force data (CSV files). Each subfolder corresponds to a specific police force and includes data across multiple months and years. This folder must remain in the same directory structure for the notebooks to locate the data.
01_data_preprocessing_police_forces.ipynb	Jupyter Notebook for data preprocessing — merges raw CSVs, cleans and formats data, removes duplicates, handles missing values, and outputs a structured dataset ready for analysis.
eda.ipynb	Jupyter Notebook for the Exploratory Data Analysis (EDA) — produces visual and statistical summaries, including regional crime comparisons, crime type distribution, temporal patterns, and outcomes.
wales_crime_heatmap (external file to download)	High-resolution crime heatmap image showing spatial clustering across Wales. Download separately for a clearer view of geographic patterns.


Opening and Running the Project in VS Code

1)	Open the Project Folder

a)	Launch Visual Studio Code (VS Code).

b)	Go to File → Open Folder.

c)	Select and open:

C:\Police forces preprocessing

This will load your Jupyter notebooks (.ipynb) directly into VS Code.

2)	Install the Required Extensions


Before running the notebooks, make sure the following VS Code extensions are installed:
•	Python (Microsoft)
•	Jupyter (Microsoft)


3)	Set Up the Python Environment


You must have Python 3.8 or later installed.
Then, open the integrated terminal in VS Code and install the required libraries:
pip install pandas numpy matplotlib seaborn folium 


4)	Open and Run the Preprocessing Notebook


a)	In VS Code, open:

01_data_preprocessing_police_forces.ipynb

b)	Run the notebook cell by cell (Shift + Enter)

c)	This notebook:

i)	Loads the raw CSVs from C:\Police forces.

ii)	Merges data from all police forces.

iii)	Cleans, formats, and prepares it for analysis.

d)	The final cleaned dataset will be ready for use in the EDA notebook.

5)	Open and Run the EDA Notebook


a)	In VS Code, open:
eda.ipynb

b)	Run all cells to generate:

i)	Crime comparisons across police forces.

ii)	Top crime types by region.

iii)	Monthly trends and seasonal patterns.

iv)	Outcome analysis and spatial insights.

c)	For full interpretation of findings, refer to the Word document report titled “Crime in Wales – Detailed EDA Analysis”, which includes extended discussion, recommendations, and conclusions.


6)	Viewing the Crime Heatmap

a)	Download the file:
wales_crime_heatmap

b)	and open it using: 

i)	VS Code image preview, or

ii)	Any image viewer (recommended for full resolution). 


This heatmap visualises crime density and hotspot regions such as Cardiff, Swansea, Newport, and Wrexham. 
Additional Notes


•	The project relies on publicly available data from the UK Police Data Portal. 

•	File paths in the notebooks use absolute references to C:\Police forces, so the folder structure must remain unchanged. 

•	If you move the data folder, update the file paths in the notebooks accordingly.

•	The full written report provides the detailed interpretation, conclusions, and next steps for future analysis. 

