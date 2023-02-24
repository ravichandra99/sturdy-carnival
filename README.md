# Dyzio API simulator

## Prerequisites

Docker,
Docker Compose,
IDE

## Clone the repository

```git clone https://secureAck@dev.azure.com/secureAck/theRoom/_git/dyzioSimulatator```

## Change directory into dyzioSimulatator

```cd dyzioSimulatator```

## Run the app

```docker-compose up```

## Run the app in detached mode in background

```docker-compose up -d```


## Post the campaign for the API to start with

Set the following parameters in postman

URL : http://127.0.0.1:5000/papi/secure/campaigns  REQUEST: POST and following example data

```JSON
{
  "data": {
    "name": "API TEST Sep 22, 2020 4:34 PM",
    "currency": "GBP",
    "budget": 10000,
    "liveDate": "2019-10-05 23:00:00.000Z",
    "endDate": "2019-12-31 00:00:00.000Z",
    "hashtags": "#INFLUENCERS,@INFLUENCERS_UK",
    "influencers": [
      {
        "id": "101-xyz",
        "name": "Felix Kjellberg",
        "email": "kat@re6l.com",
        "youtube": "UC-lHJZR3Gqxm24_Vd_AJ5Yw",
        "instagram": "pewdiepie",
        "facebook": "pewdiepie",
        "twitter": "pewdiepie"
      },
      {
        "id": "abc-202",
        "name": "Alfie Deyes",
        "email": "alfie@xyz.com",
        "youtube": "UCF5UrKfIq5ap9skGOgm4W7w",
        "instagram": "alfiedeyes",
        "facebook": "alfiedeyes",
        "twitter": "alfiedeyes"
      }
    ]
  }
}
```

Example response data:

```JSON
{
  "data": {
    "name": "API TEST Sep 22, 2020 4:34 PM",
    "currency": "GBP",
    "budget": 10000,
    "liveDate": "2019-10-05 23:00:00.000Z",
    "endDate": "2019-12-31 00:00:00.000Z",
    "hashtags": "#INFLUENCERS,@INFLUENCERS_UK",
    "influencers": [
      {
        "id": "101-xyz",
        "name": "Felix Kjellberg",
        "email": "kat@re6l.com",
        "youtube": "UC-lHJZR3Gqxm24_Vd_AJ5Yw",
        "instagram": "pewdiepie",
        "facebook": "pewdiepie",
        "twitter": "pewdiepie"
      },
      {
        "id": "abc-202",
        "name": "Alfie Deyes",
        "email": "alfie@xyz.com",
        "youtube": "UCF5UrKfIq5ap9skGOgm4W7w",
        "instagram": "alfiedeyes",
        "facebook": "alfiedeyes",
        "twitter": "alfiedeyes"
      }
    ]
  }
}
```

Rest of the end points can be found in the url https://documenter.getpostman.com/view/6352809/TVKD4J2Z#235b6c0a-012a-4760-8f3f-7fe00907cb7e


