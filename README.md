# CC-GCP-Meaty
Google Cloud Platform needs 

Project Team Members:
  - Damarjati Surya Kusuma (A210DSX1407) - Mobile Development - Jenderal Soedirman University
  - Sian Nadao Sinaga (A146DSX3704) - Mobile Development - University of Bengkulu
  - Haryanda Alfitroh (C253DSX0751) - Cloud Computing - University of Muhammadiyah Purwokerto
  - Alviona Retno Amalia (C181DSY3063) - Cloud Computing - University of Indonesia
  - Indah Noviyanti (M181DSY0087) - Machine Learning - University of Indonesia
  - Karlina Rana Salsabila (M181DSY0300) - Machine Learning - University of Indonesia

# API DOCS

## Register User

Endpoint : POST https://our-project.com/api/register/

Request Body :

```json
{
  "id" : "2",
  "first_name" : "a",
  "last_name" : "a",
  "username" : "a",
  "email" : "a@gmail.com",
  "password" : "",
  "usia" : "20",
  "domisili" : "jakarta",
  "pekerjaan" : "mahasiswa",
  "gender" : "P"
}
```

Response Body :

```json
{
  "error" : "false",
  "message" : "user created" 
}
```


## Login User

Endpoint : POST https://our-project.com/api/login/

Request Body :

```json
{
  "email" : "rra@gmail.com",
  "password" : "rahasia"
}
```

Response Body :

```json
{
  "error" : "false",
  "message" : "success",
  "loginResult" : {
      "userId" : "1",
      "name" : "g",
      "token" : "blablablabala"
  }
}
```

## Upload Image

Endpoint : POST https://our-project.com/api/upload/

Request Body :

```json
{
  "image" : "(select file)",
  "notes" : "jjj"
}
```

Response Body :

```json
{
  "error" : "false",
  "prediction" : "Fresh"
}
```

## History

Endpoint : GET https://our-project.com/api/history/(idUser)

Response Body :

```json
{
  "image": "https://blabla.jpg",
  "timestamp": "2023-06-13T02:52:55.298673Z",
  "prediction": "Fresh",
  "notes": null
}
```
