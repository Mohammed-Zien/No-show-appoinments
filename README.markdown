# No-Show Appointments Data Analysis Project

## Overview
This project analyzes a dataset of 110,527 medical appointments to identify patterns and factors influencing patient no-shows. Using Python, I explored variables like gender, age, SMS reminders, and chronic conditions to answer key questions, cleaned the data, and visualized findings to inform healthcare strategies for reducing no-show rates.

## Dataset
- **Source**: [No-Show Appointments Dataset (Kaggle, May 2016)](https://www.kaggle.com/datasets/joniarroba/noshowappointments)
- **Description**: Contains 110,527 records of patient appointments with 14 features:
  - `PatientId`: Unique patient identifier (Number)
  - `AppointmentID`: Unique appointment identifier (Number)
  - `Gender`: "M" for male, "F" for female (String)
  - `ScheduledDay`: Date of appointment booking (Date)
  - `AppointmentDay`: Date of the actual appointment (Date)
  - `Age`: Patient age (Number)
  - `Neighbourhood`: Appointment location (String)
  - `Scholarship`: Enrollment in poverty elimination program (Boolean)
  - `Hipertension`: Hypertension status (Boolean)
  - `Diabetes`: Diabetes status (Boolean)
  - `Alcoholism`: Alcoholism status (Boolean)
  - `Handcap`: Handicap status (Boolean)
  - `SMS_received`: Number of SMS reminders received (Number)
  - `No-show`: "Yes" if patient missed, "No" if attended (String)

## Objectives
- Investigate average appointments per patient and impact on no-show rates
- Analyze gender distribution and its effect on attendance
- Calculate waiting time between scheduling and appointment
- Explore influence of age, scholarships, chronic conditions, handicaps, and SMS reminders on no-shows

## Tools Used
- **Python**: Core programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Matplotlib & Seaborn**: Data visualization

## Key Findings
- 61% of patients book one appointment; mean is 1.7 appointments
- No-show rates decrease with more prior appointments, possibly due to treatment progress
- Females account for 64.3% of appointments, but gender has minimal impact on no-show rates
- Patients without SMS reminders showed higher attendance (e.g., ~80% vs. ~72% for SMS recipients)
- Handicapped patients slightly more likely to attend, possibly due to caregivers

## Project Structure
- **Investigate_a_Dataset.ipynb**: Jupyter Notebook with:
  - Data wrangling (type conversion, outlier checks)
  - Exploratory data analysis (summary stats, visualizations)
  - Conclusions and limitations
- **Database_No_show_appointments/noshowappointments-kagglev2-may-2016.csv**: Raw dataset

## Setup
1. **Clone the Repository**:
   ```bash
   git clone [your-repo-link]
   ```
2. **Install Dependencies**:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. **Run the Notebook**:
   - Open `Investigate_a_Dataset.ipynb` in Jupyter Notebook or JupyterLab
   - Ensure the CSV file is in the `Database_No_show_appointments` folder
   - Execute cells to reproduce the analysis

## Limitations
- Lacks data on caregivers, which may influence no-shows
- Unclear meaning of `Handcap` values beyond 0 and 1
- No holiday or weekend data to assess scheduling impacts
- Long waiting times (e.g., >100 days) need further investigation

## Future Work
- Analyze no-show patterns on holidays and weekends
- Investigate criteria for scholarship assignment
- Combine chronic conditions (hypertension, diabetes, alcoholism) for deeper analysis

## Author
- Mohammed Zien
- mohammed_z_elabdine@hotmail.com

## License
This project is licensed under the MIT License. Feel free to use and modify with attribution.