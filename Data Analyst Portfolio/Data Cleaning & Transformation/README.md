# UWB Clinical Surveillance Dataset Cleaning and Transformation Project

This project is focused on cleaning and transforming a dataset obtained from an Ultra-Wideband (UWB) surveillance system implemented in a hospital environment. The system is designed to track patient movement within the hospital to help enhance patient management and streamline hospital operations. 

## Dataset Description

The dataset has 610 rows and 8 columns, each row representing individual timing pulses sent from UWB tags worn by the patients. 

The columns include:

1. `id`: Unique identifier for each record.
2. `anchorID`: Identifier for the UWB anchor.
3. `tagID`: Identifier for the UWB tag (wearable) attached to patients.
4. `sequenceID`: Sequence number representing the order of the timing pulses.
5. `pan`: An attribute to be further explored.
6. `processed_flag`: Flag indicating whether the data record has been processed.
7. `timestampToA`: Timestamp of the timing pulse.
8. `Timestamp ToA`: Another version of the timestamp of the timing pulse.

## Project Goals

The project's primary aim is to clean and transform the dataset, preparing it for further analysis and modeling. The specific goals include:

1. **Data Integrity and Completeness**: Confirming that there are no missing values in the dataset and handling any inconsistencies or errors.
2. **Data Consistency**: Checking data type consistency across the dataset and identifying any discrepancies or anomalies.
3. **Data Normalization**: Normalizing or standardizing the numerical data to prepare the dataset for machine learning algorithms.
4. **Feature Engineering**: Creating additional features from the existing data, such as the time spent by patients in specific hospital areas or their movement frequency.
5. **Data Privacy**: Ensuring that the dataset does not contain any sensitive information compromising patient privacy.
6. **Outlier Detection**: Identifying any outliers in the numerical data.
7. **Data Use**: Preparing the data for future analyses or models, ensuring it's appropriately formatted.

## Technologies Used

- Python
- Pandas
- Sklearn
- Matplotlib
- Seaborn

## Key Findings

Through this project, we:

- Confirmed data completeness and consistency, with no missing values or discrepancies found.
- Normalized and standardized the `timestampToA` attribute to ensure data consistency for machine learning algorithms.
- Engineered a new feature, `time_diff`, to analyze the time spent by patients in different hospital areas.
- Ensured that the dataset does not contain any sensitive information and is compliant with data privacy regulations.
- Checked for outliers using boxplots and found no significant outliers in the normalized and standardized `timestampToA` data.

## Potential Uses

This cleaned and transformed dataset can be used for:

- Analyzing patient movement patterns within the hospital, which can assist in optimizing hospital layout and improving patient care.
- Understanding the efficiency of the UWB surveillance system through the `processed_flag` attribute.
- Tracking the sequence of patients' movements using the `sequenceID` attribute.
- Identifying patient locations at different times using the `anchorID` attribute. 

## Project Files

- `uwb_clinical_surveillance.ipynb`: Jupyter notebook containing the code for data cleaning, transformation, and analysis.
- `blink.csv`: The raw dataset file.
- `README.md`: This file, providing an overview of the project.

## Contributing

This project is open-source and accepts contributions. If you wish to contribute, please open a pull request. If you have any questions, please feel free to contact me.

## License

This project is available under the MIT License - see the LICENSE.md file for details.

## Author

Haochen Miao

<br> email: haochen.miao2000@gmail.com