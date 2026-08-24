# Data Dictionary — NovaHealth Executive Operations Dataset

| Column Name | Description | Data Type |
|---|---|---|
| `Patient_ID` | Unique identifier assigned to each patient record. | Numeric |
| `Month` | The month of the year the appointment was made. | Date |
| `Month_Num` | The month number of the 12-month calendar. | Numeric |
| `Admission_Date` | Date the patient was admitted to the healthcare facility. | Date |
| `Facility_Name` | Name of the hospital or clinic where the patient received care. | String |
| `Gender` | Biological sex of the patient (Male/Female). | String |
| `Age` | Patient's age at the time of admission. | Numeric |
| `Clinical_Status` | Current treatment or recovery status of the patient. | String |
| `CareStage_Location` | Combined field containing the patient's care stage and assigned medical department, separated by a comma. | String |
| `Medical_Department` | Hospital department responsible for the patient's care, after splitting the combined field. | String |
| `Patient_Bill` | Total amount billed for the patient's hospital stay and medical services. | Numeric (Currency) |
| `Operational_Cost` | The amount spent on treating each patient. | Currency |
| `Staff_Overtime_Hrs` | Total overtime hours logged by the attending healthcare staff. | Numeric |
| `Risk_Tier` | Patient risk category (Low-Risk, Moderate-Risk, High-Risk), determined using the Care Stage value. | String |
| `Age_Group_Class` | Age group classification (Pediatric, Adult, Geriatric), based on patient age. | String |

**Note:** The original dataset included a `Patient_Name` field. This column was removed prior to publishing — `Patient_ID` is retained as the sole identifier to avoid publishing any personally-identifiable-looking data on a public repository.
