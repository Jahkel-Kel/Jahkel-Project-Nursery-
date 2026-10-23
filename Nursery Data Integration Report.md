Nursery Data Integration Report

1. The Three Datasets

The first dataset, batch101.csv, comes from a keycard badge reader that tracks who enters the room, such as a parent or a nurse. The format is CSV format which a single record represents a single entry event. The second dataset, named feed101.xml, is produced by medical monitors. It measures the patient's vitals, like heart rate, breathing rate, temperature, and their medical conditions, if they have any. The dataset is in XML format, and a single record represents one patient's vital signs at a specific moment. The last dataset source is stream101.json, which is in JSON format and is produced by smart room sensors that measure room temperature, room humidity, and the room status to see if the doors are open or closed. The single records represent the room environment at a specific time. 

2. Questions or Scenarios the Integrated File Can Answer

By combining the files, an analyst can answer complex questions, such as whether room temperature affects an infant's vital signs and whether nurses or parents opening and closing the door causes the baby's heart and breathing rate to spike. 

3. Format Choice

I chose JSON format because it's great for organizing data, like putting the patient vitals into one single record. Why I haven't chosen to put it as a CSV and an XML is because the CSV file would be untidy and have repetitive tables. For the XML file, it would be hard to work with because everything is too bulky.

4. Integrated Dataset

The integrated dataset is structured so one single record can match an infant's health vitals with their room conditions at the same time and moment. The fields it contains are timestamp and patientId, and the other fields are nested in patient vitals, which are heart rate, breathing rate, temperature, and medical condition. The nested room conditions are the room number, room temperature, door status, room humidity, and door access. These fields can relate to one another through the patient ID, which links to the baby health data and the room they're in, which can connect to the room conditions they're in.

5. Data Cleaning and Normalization

The cleaning I did was to standardize the temperature to Fahrenheit for the room temperature and patient temperature. For the missing information that I had blank, I changed it to null so it can look neater and more put together and lastly, I split all the data and time formats so they can be more easer to read better than putting the data and time in one field.  

6. Trade-offs

By combining the data, I gain an all-in-one view that connects the patient's health with the room environment and activity. What I lost was real-time tracking rather than the 5-minute updates for the records. The CSV data updates when someone enters or leaves the room, but I had to change it to group snapshots every 5 minutes.
