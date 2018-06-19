# Face Identification

Fece tracking and recognition using Microsoft Azure's Face APIs. The request is only send when a new face is detected.

## Installation
The `requirements.txt` file contains much more than the strict requirements to run this app, but saves time to just install everything at once.

### Setup
Run these scripts sequentialy. You will need to appropriately edit these scripts to include the correct Face API subscription key, names, and images of the people.

```sh
# Create a group
python Azure/train_faces_create_person_group_1.py

# Add people to the group
python Azure/train_faces_add_person_2.py

# Add faces for the poeple
python Azure/train_faces_add_face_3.py

# Train the API to learn the faces and associate the features wiht the people
python Azure/train_faces_train_4.py
```

### Execution
To run the detector:
```sh
python demo - detect and track.py
```

This script internally imports `train_faces_detect_face_5.py` which takes the address of a local image on the disk and returns the `name`, `confidence` of the person with highest score.

# Screenshots

