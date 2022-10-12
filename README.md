# GHL_BackendToFHIR **API** 參考

## **GET**：http://localhost:3080/ghl/fhir/Patient?name=吳爸爸

可帶入參數：id、identifier、name、birthDate、gender。  

### **response** ：Array

```json
[
    {
        "resourceType": "Patient",
        "_id": "E125678198",
        "identifier": [
            {
                "use": "official",
                "type": {
                    "coding": [
                        {
                            "system": "http://terminology.hl7.org/CodeSystem/v2-0203",
                            "code": "NI"
                        }
                    ]
                },
                "system": "http://www.moi.gov.tw/",
                "value": "E125678198"
            }
        ],
        "active": true,
        "name": [
            {
                "use": "official",
                "text": "吳爸爸D",
                "family": "吳",
                "given": "爸爸"
            }
        ],
        "telecom": [
            {
                "system": "phone",
                "value": "0911710942",
                "use": "mobile",
                "period": {
                    "start": "2022-07-31",
                    "end": "2024-07-31"
                }
            }
        ],
        "gender": "female",
        "birthDate": "2011-09-07T16:00:00.000Z"
    }
]
```

## **GET**：http://localhost:3080/ghl/fhir/Patient/E125678198

### **response** ：object

```json
{
    "resourceType": "Patient",
    "_id": "E125678198",
    "identifier": [
        {
            "use": "official",
            "type": {
                "coding": [
                    {
                        "system": "http://terminology.hl7.org/CodeSystem/v2-0203",
                        "code": "NI"
                    }
                ]
            },
            "system": "http://www.moi.gov.tw/",
            "value": "E125678198"
        }
    ],
    "active": true,
    "name": [
        {
            "use": "official",
            "text": "吳爸爸D",
            "family": "吳",
            "given": "爸爸"
        }
    ],
    "telecom": [
        {
            "system": "phone",
            "value": "0911710942",
            "use": "mobile",
            "period": {
                "start": "2022-07-31",
                "end": "2024-07-31"
            }
        }
    ],
    "gender": "female",
    "birthDate": "2011-09-07T16:00:00.000Z"
}
```


## **POST**：http://localhost:3080/ghl/fhir/Patient
### **request** ：object
```json 
{
    "resourceType": "Patient",
    "_id": "E125678198",
    "identifier": [
        {
            "use": "official",
            "type": {
                "coding": [
                    {
                        "system": "http://terminology.hl7.org/CodeSystem/v2-0203",
                        "code": "NI"
                    }
                ]
            },
            "system": "http://www.moi.gov.tw/",
            "value": "E125678198"
        }
    ],
    "active": true,
    "name": [
        {
            "use": "official",
            "text": "吳爸爸D",
            "family": "吳",
            "given": "爸爸"
        }
    ],
    "telecom": [
        {
            "system": "phone",
            "value": "0911710942",
            "use": "mobile",
            "period": {
                "start": "2022-07-31",
                "end": "2024-07-31"
            }
        }
    ],
    "gender": "female",
    "birthDate": "2011-09-07T16:00:00.000Z"
}
```
 ### **response** ：object
 ```json 
{
    "resourceType": "Patient",
    "_id": "E125678198",
    "identifier": [
        {
            "use": "official",
            "type": {
                "coding": [
                    {
                        "system": "http://terminology.hl7.org/CodeSystem/v2-0203",
                        "code": "NI"
                    }
                ]
            },
            "system": "http://www.moi.gov.tw/",
            "value": "E125678198"
        }
    ],
    "active": true,
    "name": [
        {
            "use": "official",
            "text": "吳爸爸D",
            "family": "吳",
            "given": "爸爸"
        }
    ],
    "telecom": [
        {
            "system": "phone",
            "value": "0911710942",
            "use": "mobile",
            "period": {
                "start": "2022-07-31",
                "end": "2024-07-31"
            }
        }
    ],
    "gender": "female",
    "birthDate": "2011-09-07T16:00:00.000Z"
}
 ```





## **PUT**：http://localhost:3080/ghl/fhir/Patient/E125678198
### **request** ：object
```json 
{
    "resourceType": "Patient",
    "_id": "E125678198",
    "identifier": [
        {
            "use": "official",
            "type": {
                "coding": [
                    {
                        "system": "http://terminology.hl7.org/CodeSystem/v2-0203",
                        "code": "NI"
                    }
                ]
            },
            "system": "http://www.moi.gov.tw/",
            "value": "E125678198"
        }
    ],
    "active": true,
    "name": [
        {
            "use": "official",
            "text": "吳爸爸AFWA",
            "family": "吳",
            "given": "爸爸"
        }
    ],
    "telecom": [
        {
            "system": "phone",
            "value": "0911710942",
            "use": "mobile",
            "period": {
                "start": "2022-07-31",
                "end": "2024-07-31"
            }
        }
    ],
    "gender": "female",
    "birthDate": "2011-09-07T16:00:00.000Z"
}
```
 ### **response** ：object
 ```json 
{
    "resourceType": "Patient",
    "_id": "E125678198",
    "identifier": [
        {
            "use": "official",
            "type": {
                "coding": [
                    {
                        "system": "http://terminology.hl7.org/CodeSystem/v2-0203",
                        "code": "NI"
                    }
                ]
            },
            "system": "http://www.moi.gov.tw/",
            "value": "E125678198"
        }
    ],
    "active": true,
    "name": [
        {
            "use": "official",
            "text": "吳爸爸AFWA",
            "family": "吳",
            "given": "爸爸"
        }
    ],
    "telecom": [
        {
            "system": "phone",
            "value": "0911710942",
            "use": "mobile",
            "period": {
                "start": "2022-07-31",
                "end": "2024-07-31"
            }
        }
    ],
    "gender": "female",
    "birthDate": "2011-09-07T16:00:00.000Z"
}
 ```



 ## **DELETE**：http://localhost:3080/ghl/fhir/Patient/E125678198
