# Personal Health Record App JSON Data Structure.

This data struture should be considered in development.

## Example Structure (as of 2013/12/18):

````json
{
  "user": {
    "id": "object_id",
    "firstName": "John",
    "middleName": "Random",
    "lastName": "Doe",
    "email": "john.doe@example.com",
    "createdAt": "2013/12/20",
    "updatedAt": "2013/12/20",
    "birthdate": "1980/10/20",
    "illnesses": [
      {
        "id": "object_id",
        "illness_type_id": "object_id",
        "startDate": "2013/12/20",
        "endDate": "2013/12/25",
        "createdAt": "2013/12/25",
        "updatedAt": "2013/12/25",
        "medicationsTaken": [
          {
            "medication_id": "object_id",
            "startDate": "2013/12/21",
            "endDate": "2013/12/25"
          }
        ],
        "versions": [
          {
            "id": "object_id",
            "illness_type_id": "object_id",
            "startDate": "2013/12/20",
            "endDate": "2013/12/25",
            "medicationsTaken": [
              {
                "medication_id": "object_id",
                "startDate": "2013/12/21",
                "endDate": "2013/12/25"
              }
            ]
          }
        ]
      }
    ],
    "activities": [
      {
        "id": "object_id",
        "type": "Bench Press",
        "date": "2013/12/20",
        "time": "20:30",
        "weight": "120",
        "reps": "8",
        "sets": "3"
      },
      {
        "id": "object_id",
        "type": "Exercise Bike",
        "date": "2013/12/19",
        "time": "20:30",
        "duration": "1800",
        "restingHeartRate": "103",
        "targetHeartRate": "132",
        "caloriesBurned": "189"
      }
    ],
    "conditions": [
      {
        "condition_id": "object_id",
        "startDate": "2010/1/3",
        "endDate": null,
        "medicationsTaken": [
          {
            "medication_id": "object_id",
            "datesTaken": [
              "2013/10/12",
              "2011/10/12"
            ]
          }
        ]
      }
    ],
    "currentMedications": [
      {
        "medication_id": "object_id",
        "medication_type_id": "object_id",
        "startDate": "2013/12/21",
        "condition_type": "illness or condition name",
        "condition_id": "object_id"
      }
    ],
    "medicationsTaken": [
      {
        "medication_id": "object_id",
        "medication_type_id": "object_id",
        "startDate": "2012/12/21",
        "endDate": "2012/12/25",
        "condition_type": "illness or condition name",
        "condition_id": "object_id"
      }
    ],
    "treatements": [
      {
        "treatement_id": "object_id",
        "treatment_type_id": "object_id",
        "treatement_name": "Phyiscal Therapy",
        "startDate": "2012/10/1",
        "endDate": "2012/12/3",
        "provider": "object_id",
        "activity_id": "object_id"
      }
    ]
  }
}
````