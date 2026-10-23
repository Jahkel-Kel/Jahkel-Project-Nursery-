# Integrating IoT Sensor Data for Nursery Project

## What the Project Is

This project combines data from medical monitors, room sensors, and access logs into one JSON file. Instead of just looking at the patient's health, it helps analyze how well the hospital operates, the workflow of staff and parents, and how rooms are used. By bringing all this information together, hospital teams can see connections between staff visits, room temperature, and the patient's vital signs.

## What Each File Does

feed101.xml: Stores bedside medical monitor data, tracking infant heart rates, breathing rates, body temperatures, and their medical condition if they have any.

stream101.json: Captures real-time room environment telemetry, monitoring room temperature and door status (open/closed).

batch101.csv: Logs keycard badge entries, recording when staff or visitors (e.g., nurses, doctors, parents) enter specific rooms.

integratedDataset.json: Combines the data from all three files into a synchronized JSON dataset matching patient vitals with room conditions and entry logs at specific timestamps.
