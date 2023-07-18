# Hospital Management System

This is a simple Hospital Management System implemented in Python using object-oriented programming (OOP) principles.

The project allows you to manage doctors, patients, and rooms in a hospital. It provides basic functionalities such as adding and removing doctors and patients, assigning patients to rooms, discharging patients, and retrieving the number of doctors, patients, and rooms.

## Features

- Add doctors with their name and specialty.
- Add patients with their name and condition.
- Add rooms with room numbers.
- Assign patients to rooms.
- Discharge patients from rooms.
- Retrieve the number of doctors, patients, and rooms.
- Display detailed information about doctors, patients, and rooms.

## Code Sample

Here is an example of how to use the classes and methods provided by the project:

```python


hospital = Hospital()

doctor1 = Doctor("علی محمدی", "جراحی")
doctor2 = Doctor("مهدی علوی", "داخلی")
hospital.add_doctor(doctor1)
hospital.add_doctor(doctor2)

patient1 = Patient("علی احمدی", "سرماخوردگی")
patient2 = Patient("زهرا میرزایی", "آنفولانزا")
hospital.add_patient(patient1)
hospital.add_patient(patient2)

room1 = Room(101)
room2 = Room(102)
hospital.add_room(room1)
hospital.add_room(room2)

room1.assign_patient(patient1)
room2.assign_patient(patient2)

hospital.get_num_doctors()
hospital.get_num_patients()
hospital.get_num_rooms()

hospital.get_doctors()
hospital.get_patients()
hospital.get_rooms()

room1.discharge_patient()
room2.discharge_patient()

hospital.remove_patient(patient1)
hospital.remove_room(room2)

hospital.get_patients()
hospital.get_rooms()

