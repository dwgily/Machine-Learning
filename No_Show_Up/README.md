# Predict No Shows for Medical Appointments
Resource planning is crucial for any business; it's even more so for operations struggling with
resource crunch. Government sponsored medical services is a prime example of such an
operation. In almost all developing countries , there is severe shortage of medical personnel and
at the same time, not ideal living conditions for big chunk of the population further exacerbates
need of medical attention.

Governments have tried floating subsidised access to poor families to increase access to
healthcare . One big problem which stops better utilisation of this facility is that people make
appointments but do not show up without a notice. That time slot could have been given to a
needier person if authorities were able to determine who is very likely to not show-up and
followup appropriately .

Your task here is to make use of historical records to build a model for predicting a No-Show for
an appointement given appoint details, medical history and demographic details of the customer.

# Data Files
- Medical History = medical_history.csv
- Demographic Details = demographic_details.csv
- Train Dataset =train.csv
- Test Dataset = test_share.csv

## Medical History
- PatientId: A unique identifier for each patient in the dataset.
- Hipertension: Indicates whether the patient has hypertension (1 = Yes, 0 = No).
- Diabetes: Indicates whether the patient has diabetes (1 = Yes, 0 = No).
- Alcoholism: Indicates whether the patient has a history of alcoholism (1 = Yes, 0 = No).
- Handcap: Indicates the level of physical handicap (0 = None, 1-4 = Degree of handicap).

## Demographic Details
- PatientId: A unique identifier for each patient in the dataset.
- Gender: The gender of the patient (e.g., Male, Female).
- Age: The age of the patient at the time of the record.
- Neighbourhood: The area or locality where the patient resides.
- Scholarship: Indicates whether the patient is a recipient of a medical scholarship or assistance (1 = Yes, 0 = No).

## Training Dataset 
- PatientId: A unique identifier for each patient in the dataset.
- AppointmentID: A unique identifier for each medical appointment.
- ScheduledDay: The date and time when the appointment was scheduled.
- SMS_received: Indicates whether the patient received an SMS reminder for the appointment (1 = Yes, 0 = No).
- No-show: Indicates whether the patient attended the scheduled appointment (1 = No-show, 0 = Attended).

# Model Summary
| Model                | Accuracy | Precision | Recall  | F1 Score | ROC AUC  |
|----------------------|----------|-----------|---------|----------|----------|
| K-Nearest Neighbors   | 0.777164 | 0.379608  | 0.192879| 0.255791 | 0.666406 |
| Decision Tree         | 0.732536 | 0.326648  | 0.327033| 0.326840 | 0.579985 |
| Logistic Regression   | 0.798003 | 0.345345  | 0.019406| 0.036747 | 0.667373 |
| Random Forest         | 0.796797 | 0.467629  | 0.169423| 0.248730 | 0.727434 |
| AdaBoost              | 0.800784 | 0.462121  | 0.020587| 0.039418 | 0.727858 |
| Bagging Classifier    | 0.789125 | 0.425264  | 0.176679| 0.249642 | 0.694638 |
| Extra Trees           | 0.783563 | 0.410282  | 0.206041| 0.274320 | 0.702551 |
| Gradient Boosting     | 0.801488 | 0.505618  | 0.007594| 0.014963 | 0.732677 |
| XGBoost               | 0.801521 | 0.501168  | 0.072393| 0.126511 | 0.739448 |
| LightGBM              | 0.802794 | 0.563291  | 0.030037| 0.057033 | 0.738784 |

![image](https://github.com/user-attachments/assets/1185a849-232d-4aae-bd12-b95d2f61aef1)


