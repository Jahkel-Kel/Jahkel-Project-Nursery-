| Field name | Data Type | Units | What it represents |
| :--- | :--- | :--- | :--- |
| date | String (Year-Month-Day) | None | The date the data was recorded |
| timeWindow | String | Hours/Minutes | Start and end time of the monitoring period |
| records | Array of Objects | None | A list of all the reading taken over time |
| timestamp | String (00:00) | Time (Minutes) | The exact time the reading was taken |
| patientId | String | None | The ID number that was assigned to the patient |
| heartRate | String (Numeric) | Beats per minute (BPM) | How fast the patients heart is beating |
| breathingRate | String (Numeric) | Breaths per minute (Brpm) | How many breaths they took every minute |
| temperature | String (Numeric) | Fahrenheit | The patients body temperature |
| medicalCondition | String (Null) | None | Whether the patient has a medical condition and what specific condition |
| roomNumber | String (Integer) | None | The room where the patient is staying |
| roomTempF | Float | Fahrenheit | The temperature of the room the patient is in |
| doorStatus | String | None | Whether the room door is open or closed |
| roomHumidity | Float (Null) | Percentage (%) | The Humidity level in the room |
| doorAccess | String (Null) | None | A record who opened or entered the room |
| patientVitals | Object | None | A group with all the patient's health readings |
| roomConditions | Object | None | A group that contains all the information about the patient's room |
