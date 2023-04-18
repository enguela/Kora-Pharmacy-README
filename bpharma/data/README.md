# Data

A RestFull API to distribute information to the various other components and to collect their information. 
`data` collect informations collected by `linker` in the pharmacy Information System and also by `mobile` provided by the user.
The informations provided by `linker` relates to the availability of medicines and the informations provided by `mobile` relates to the user's informations
like location, requested drug and others to help him to find the drug he wants.


## Endpoints
  
***1. <ins>Drugs <ins>*** 
  
root : `/drug`
  
- [ ] ***`url=(empty) method=GET params=page(int)`*** : list drugs

```jsonc
{
  "drugs": [
    {
      "dci": "Abacavir Lamivudine",
      "nom_specialite": "",
      "laboratory": {
        "label": "Sandoz",
        "description": "",
        "logo": "",
        // .
        // .
        // .
```
<!--
        "location": "",
        "city": "",
        "country": "",
        "timemodified": 0,
        "timecreated": 0,
        "contacts": {
          "2": [
            {
              "value": "(49) 8024 476 0",
              "owner": "5",
              "owner_group": "2",
              "type": "2",
              "id": 43
            }
          ],
          "3": {
            "value": "https://www.sandoz.com",
            "owner": "5",
            "owner_group": "2",
            "type": "3",
            "id": 37
          },
          "5": {
            "value": "https://www.facebook.com/sandozglobal/",
            "owner": "5",
            "owner_group": "2",
            "type": "5",
            "id": 38
          },
          "6": {
            "value": "https://twitter.com/sandoz_global",
            "owner": "5",
            "owner_group": "2",
            "type": "6",
            "id": 39
          },
          "8": {
            "value": "https://www.instagram.com/sandozglobal",
            "owner": "5",
            "owner_group": "2",
            "type": "8",
            "id": 41
          },
          "9": {
            "value": "https://www.youtube.com/user/Sandoz",
            "owner": "5",
            "owner_group": "2",
            "type": "9",
            "id": 42
          },
          "10": {
            "value": "https://www.linkedin.com/company/sandoz",
            "owner": "5",
            "owner_group": "2",
            "type": "10",
            "id": 40
          }
        },
        "id": 5
      },
      "timecreate": "1610670093",
      "timemodified": "1610670093",
      "modifierid": "1",
      "deleted": 0,
      "id": 11,
      "img_url": "http://data.bpharma.com/pix/drugs/sandoz/abacavir_lamivudine/abacavir_lamivudine",
      "classes": [
        {
          "id": 70,
          "label": "Antiretroviral",
          "description": "used for the treatment of retrovirus-related infections"
        }
      ]
     },
-->
```jsonc
        // .
        // .
        // .
  ],
  "page": 1,
  "maxpage": 3
}
```

- [ ] ***`url=/([0-9]+) method=GET`*** : list drug information (manufacturer, distributions)

```jsonc
{
  "classes": [
    {
      "id": 74,
      "label": "Antibacterial",
      "description": "substance used to fight against bacteria"
    }
  ],
  "distributions": [
    {
      "id": 10,
      // .
      // .
      // .
```
<!--
      "galenical_form": {
        "salable": false,
        "label": "Pommade"
      },
      "drug_usage": "external",
      "administration_way": "Dermal",
      "dosage": "300mg",
      "substances": [
        {
          "id": 209,
          "label": "Fusidic acid",
          "weight": "300",
          "active": true
        },
        {
          "id": 206,
          "label": "Cetyl alcohol",
          "weight": 0,
          "active": false
        },
        {
          "id": 18,
          "label": "Eau purifiée",
          "weight": 0,
          "active": false
        },
        {
          "id": 40,
          "label": "Glycerol",
          "weight": 0,
          "active": false
        },
        {
          "id": 210,
          "label": "Butylated hydroxyanisole",
          "weight": 0,
          "active": false
        },
        {
          "id": 211,
          "label": "Soft white kerosene",
          "weight": 0,
          "active": false
        },
        {
          "id": 107,
          "label": "Light liquid paraffin",
          "weight": 0,
          "active": false
        },
        {
          "id": 33,
          "label": "polysorbate 80",
          "weight": 0,
          "active": false
        },
        {
          "id": 17,
          "label": "Sorbate de potassium",
          "weight": 0,
          "active": false
        }
      ],
      "packages": {
        "1": {
          "type": "1",
          "label": "Tube",
          "capacities": [
            {
              "capacity": "15",
              "unit": "g",
              "price": 0
            }
          ]
        },
        "2": {
          "type": "2",
          "label": "Box Manufacture",
          "capacities": [
            {
              "capacity": "1",
              "unit": "Tube",
              "price": 0
            }
          ]
        }
      },
      "img_url": "http://data.bpharma.com/pix/drugs/mylan/acide_fusidique/cr_300mg"
    }
  ],
  "laboratory": {
    "label": "Mylan",
    "description": "",
    "logo": "http://data.bpharma.com/pix/drugs/mylan/",
    "location": "",
    "city": "",
    "country": "",
    "timemodified": 0,
    "timecreated": 0,
    "contacts": {
      "1": [
        {
          "value": "communications@viatris.com",
          "owner": "3",
          "owner_group": "2",
          "type": "1",
          "id": 33
        }
      ],
      "2": [
        {
          "value": "(1) 724 514 1968",
          "owner": "3",
          "owner_group": "2",
          "type": "2",
          "id": 34
        }
      ],
      "3": {
        "value": "https://www.mylan.com",
        "owner": "3",
        "owner_group": "2",
        "type": "3",
        "id": 29
      },
      "5": {
        "value": "https://www.facebook.com/MylanFrance",
        "owner": "3",
        "owner_group": "2",
        "type": "5",
        "id": 30
      },
      "9": {
        "value": "https://www.youtube.com/channel/UCboEkEfL0GYoo09ftmlMMHg",
        "owner": "3",
        "owner_group": "2",
        "type": "9",
        "id": 31
      },
      "10": {
        "value": "https://www.linkedin.com/company/mylan-france/",
        "owner": "3",
        "owner_group": "2",
        "type": "10",
        "id": 32
      }
    },
-->
```jsonc
       // .
       // .
       // .
    "id": 3
  }
}

```
  
***<ins>Drug distributions<ins> :***
  
root : `/distribution`
  
- [ ] ***`url=(empty) method=GET params=page(int)`*** : list distributions

```jsonc
{
  "distributions": [
    {
      "id": 1,
      "dci": "Bimalaril",
       // .
       // .
       // .
```
<!--
      "laboratory": "Medicale Pharmaceutique",
      "form": "Suspension",
      "dosage": "20-120mg/5ml",
      "img_url": "http://data.bpharma.com/pix/drugs/medicale_pharmaceutique/bimalaril/susp_20_120mg_5ml"
    },
-->
```jsonc
       // .
       // .
       // .
  ],
  "page": 1,
  "maxpage": 5
}

```
  
<!--***`url=/listforpages method=GET params=page(int)`*** :-->
  
- [ ] ***`url=/([0-9]+) method=GET`*** : read distribution description
```jsonc
{
  "classes": [
    {
      "id": 48,
      "label": "Antipaludic",
      "description": "Drug used in the short-term prevention and treatment of malaria"
    }
  ],
  "distribution": {
    "id": 1,
    "galenical_form": {
      "salable": false,
      "label": "Suspension"
       // .
       // .
       // .
```
<!--
    },
    "drug_usage": "internal",
    "administration_way": "Oral",
    "dosage": "20-120mg/5ml",
    "substances": [
      {
        "id": 72,
        "label": "Artemether",
        "weight": "20",
        "active": true
      },
      {
        "id": 190,
        "label": "Lumefantrine",
        "weight": "120",
        "active": true
      },
      {
        "id": 140,
        "label": "Sodium citrate",
        "weight": 0,
        "active": false
      },
      {
        "id": 62,
        "label": "Xanthan gum",
        "weight": 0,
        "active": false
      },
      {
        "id": 11,
        "label": "Saccharine sodique",
        "weight": 0,
        "active": false
      },
      {
        "id": 191,
        "label": "Sucrose",
        "weight": 0,
        "active": false
      },
      {
        "id": 192,
        "label": "Vanillin",
        "weight": 0,
        "active": false
      }
    ],
    "packages": {
      "1": {
        "type": "1",
        "label": "Bottle",
        "capacities": [
          {
            "capacity": "30",
            "unit": "ml",
            "price": "3500"
          }
        ]
      },
      "2": {
        "type": "2",
        "label": "Box Manufacture",
        "capacities": [
          {
            "capacity": "1",
            "unit": "Bottle",
            "price": "3500"
          }
        ]
      }
    },
    "img_url": "http://data.bpharma.com/pix/drugs/medicale_pharmaceutique/bimalaril/susp_20_120mg_5ml"
  },
  "laboratory": {
    "label": "Medicale Pharmaceutique",
    "description": "",
    "logo": "http://data.bpharma.com/pix/drugs/medicale_pharmaceutique/",
    "location": "",
    "city": "",
    "country": "",
    "timemodified": 0,
    "timecreated": 0,
-->
```jsonc
       // .
       // .
       // .
    "contacts": [],
    "id": 15
  }
}
```
  
- [ ] ***`url=/([0-9]+)/search method=GET params=page(int)`*** : check distribution avaibility

```jsonc
{
  "found": true,
  "pharmacies": {
    "pharmacies": [
      {
        "pix_url": "yaounde/beato_mamaso",
        "name": "Pharmacie BEATO MAMASO",        
       // .
       // .
       // .
```
<!--
        "phone": "+237 2 22 31 57 52",
        "pharmacy_key": "1",
        "subscription": "3",
        "activated": "",
        "district": "Biyem-Assi",
        "town_area": 0,
        "latitude": "3.8554538886233396",
        "longitude": "11.481579221340173",
        "contacts": [],
        "id": 1,
        "town": "Yaoundé",
        "working_times": [
          {
            "day": "",
            "start": "",
            "end": "",
            "pharmacy": "1",
            "id": 1
          },
          {
            "day": "1",
            "start": "09:00 AM",
            "end": "05:00 PM",
            "pharmacy": "1",
            "id": 2
          },
          {
            "day": "2",
            "start": "09:00 AM",
            "end": "05:00 PM",
            "pharmacy": "1",
            "id": 3
          },
          {
            "day": "3",
            "start": "09:00 AM",
            "end": "05:00 PM",
            "pharmacy": "1",
            "id": 4
          },
          {
            "day": "4",
            "start": "09:00 AM",
            "end": "05:00 PM",
            "pharmacy": "1",
            "id": 5
          },
          {
            "day": "5",
            "start": "09:00 AM",
            "end": "05:00 PM",
            "pharmacy": "1",
            "id": 6
          },
          {
            "day": "6",
            "start": "09:00 AM",
            "end": "05:00 PM",
            "pharmacy": "1",
            "id": 7
          }
        ],
        "changedate": "Monday",
        "changetime": "09:00 AM",
-->
```jsonc
       // .
       // .
       // .
        "changestring": "monday at 09:00 AM",
        "opened": false
      }
    ]
  }
}
```
  
- [ ] ***`url=/availability method=POST`*** : update distribution avaibility by `linker`
```json
{
  "success": true,
}
```
  
 <!--***`url=/([0-9]+)/store method=GET params=page(int)`*** : check distribution avaibility-->

***<ins>Drug classes<ins> :*** 
  
- [ ] ***`url=/class method=GET params=page(int)`*** : list drug classes
```jsonc
{
  "classes": [
    {
      "id": 41,
      "label": "Antalgic",       
       // .
       // .
       // .
```
<!--     
      "description": "Alleviate pain"
    },
    {
      "id": 76,
      "label": "Anthelmintic",
      "description": "an antiparasitic drug1 that eradicates parasitic worms, especially gastrointestinal worms in humans or animals"
    },    
-->
```jsonc
       // .
       // .
       // .
  ],
  "page": 1,
  "maxpage": 2
}
```
  
***<ins>Drug forms<ins> :*** 
  
- [ ] ***`url=/form method=GET params=page(int)`*** : list drug forms
```jsonc
{
  "forms": [
    {
      "id": 41,
      "label": "Powder",       
       // .
       // .
       // .
```
<!--     
      "description": "formed by dried solids particles, free and thin"
    },
    {
      "id": 76,
      "label": "Tablet",
      "description": ""
    },    
-->
```jsonc
       // .
       // .
       // .
  ],
  "page": 1,
  "maxpage": 2
}
```
- [ ] ***<ins>Drug stores<ins> :*** 
  
root : `/pharmacy`
  
- [ ] ***`url=(empty) method=GET params=page(int)`*** : list drug stores
```jsonc
{
  "page": 1,
  "maxpage": 2
  "pharmacies": {
    "pharmacies": [
      {
        "pix_url": "yaounde/beato_mamaso",
        "name": "Pharmacie BEATO MAMASO",        
       // .
       // .
       // .
```
<!--
        "phone": "+237 2 22 31 57 52",
        "pharmacy_key": "1",
        "subscription": "3",
        "activated": "",
        "district": "Biyem-Assi",
        "town_area": 0,
        "latitude": "3.8554538886233396",
        "longitude": "11.481579221340173",
        "contacts": [],
        "id": 1,
        "town": "Yaoundé",
        "working_times": [
          {
            "day": "",
            "start": "",
            "end": "",
            "pharmacy": "1",
            "id": 1
          },
          {
            "day": "1",
            "start": "09:00 AM",
            "end": "05:00 PM",
            "pharmacy": "1",
            "id": 2
          },
          {
            "day": "2",
            "start": "09:00 AM",
            "end": "05:00 PM",
            "pharmacy": "1",
            "id": 3
          },
          {
            "day": "3",
            "start": "09:00 AM",
            "end": "05:00 PM",
            "pharmacy": "1",
            "id": 4
          },
          {
            "day": "4",
            "start": "09:00 AM",
            "end": "05:00 PM",
            "pharmacy": "1",
            "id": 5
          },
          {
            "day": "5",
            "start": "09:00 AM",
            "end": "05:00 PM",
            "pharmacy": "1",
            "id": 6
          },
          {
            "day": "6",
            "start": "09:00 AM",
            "end": "05:00 PM",
            "pharmacy": "1",
            "id": 7
          }
        ],
        "changedate": "Monday",
        "changetime": "09:00 AM",
-->
```jsonc
       // .
       // .
       // .
        "changestring": "monday at 09:00 AM",
        "opened": false
      }
    ]
  }
}
```
  
- [ ] ***`url=/([0-9]+) method=GET params=page(int)`*** : read drug store information
```jsonc
{
  "pix_url": "yaounde/beato_mamaso",
  "name": "Pharmacie BEATO MAMASO",        
       // .
       // .
       // .
```
<!--
  "phone": "+237 2 22 31 57 52",
  "pharmacy_key": "1",
  "subscription": "3",
  "activated": "",
  "district": "Biyem-Assi",
  "town_area": 0,
  "latitude": "3.8554538886233396",
  "longitude": "11.481579221340173",
  "contacts": [],
  "id": 1,
  "img_url": "http://data.bpharma.com/pix/stores/yaounde/beato_mamaso?user=WF0IXKO9nbrnITST7Q22QRUfEcUOdic4AVhVbSl68pr6XKzees/IHOmytsXBaSO8XjNTJed531LGnBb7XDqqaSBwJJ55Qdtc/S3CTK9yZL+Ic+4mqA27XlpA+gK8pz+NbMZMmTpY8UD37/AOg7FplXCa2g7ZHB1Ak+2DFK6tT1HxSacvU3SnqGEbIVKGnFUolTHsbdrd5XBEZZHnVcLHS//irU+VV5MIV8QroN8GMFrxfezmJGnZjTSH/S6YTzQl+bc1IaI/EEG3zsxCnqJbZBTql1K/yG3ul34QRyFMgQoR0FkoukLVqtxhC0gH3Gh/4sgpuZkl41cOjok2NewAdpwqNnB0+naerpG4f8uaTnxpQD9EOtU1c32hVPAhT1+LIh3UW38sDsiyeD2DC/w3k/59Lvc1Q46zV0h1aVUym74MPjrscN+jw8CbrgrtWqOwxQc6DMDokAUwuMtAEFc+6L21L4i6BEyu19EY8Ez2PEFwlXJTcf+V1vCS+JJvYwzYYecB0WEPpQCqov0diy7W63SQvv/ZWRsO07knpWj+ZnqYUfWm+eSt3s2dmC6c+NaR4z74UG2Low+b5rZlwjFHRwDVmKNAR0MiieijHG397nXBbharOHShqgwLBKa7+Pf9HyxXnl8jFrYNwBVaAGuWyIl4ZU1BrNFCMIK2QwSGZKwj958JigD9dtcZmY2kteD0SXEOK7eyVbR2PCM3YwDdD/jCoM+De+rxoyS0Nw4BvXFWO5gFul7gGLiY4C6nBSp2TF0hcOJpjSkqwTMIe8ozy2TOb9rFl7Onca7CgZ8xZ8csP3yDdASEBM5auUNlfb9IXhHly/Wpv/tRoriPY1p8+ExK2ddoW1U7xE4wY3iK478tXjcVVbm2LeMtrfH6JAJImTt2CIR8e/eQFc8Dohcb1s+7NB1jkBhGksptlQ8qdDRxunYP8ksixJAMrR+9UlEYDFbQL9ip4TZlAf6GNNUGNaP4P9f8EVX3BGIf0n5An0h9GG0i5OttvZxS4F0aiDKR8xfhB1+yNCui/MVd/U52Nfel4wWH9C9eTtijR+63KS33AMS4UXYVTCGOIJoGalNdT1V7VvXcnM2BFwMgukZJnFzA2FijW0mLgBJH8kWtCIMThDKie9nhSkBS6ezo4BSoSvpvEDfIN26p7fj8bPkmJqWHZpm+UnGBqrK1WcY9xUh1NJ4tBEJMy2X2lMZJ96Oi1kkQ8r3THy4aECqwoTWlRErCQcpZ6xMK0x0lhceH9hnNv+aqKurEFK88NIXK0oqIxwLepRdgZsBPKra8R2DoTYw/v39lyozp9lR77JS9bgt6J7Ce6Q7Fdlw5Id/OkOqj",
  "town": "Yaoundé",
  "working_times": [
    {
      "day": "",
      "start": "",
      "end": "",
      "pharmacy": "1",
      "id": 1
    },
    {
      "day": "1",
      "start": "09:00 AM",
      "end": "05:00 PM",
      "pharmacy": "1",
      "id": 2
    },
    {
      "day": "2",
      "start": "09:00 AM",
      "end": "05:00 PM",
      "pharmacy": "1",
      "id": 3
    },
    {
      "day": "3",
      "start": "09:00 AM",
      "end": "05:00 PM",
      "pharmacy": "1",
      "id": 4
    },
    {
      "day": "4",
      "start": "09:00 AM",
      "end": "05:00 PM",
      "pharmacy": "1",
      "id": 5
    },
    {
      "day": "5",
      "start": "09:00 AM",
      "end": "05:00 PM",
      "pharmacy": "1",
      "id": 6
    },
    {
      "day": "6",
      "start": "09:00 AM",
      "end": "05:00 PM",
      "pharmacy": "1",
      "id": 7
    }
  ],
  "changedate": "Monday",
  "changetime": "09:00 AM",
-->
```jsonc
       // .
       // .
       // .
  "changestring": "monday at 09:00 AM",
  "opened": false,
  "on_call": false
}
```
  
- [ ] ***`url=/([a-zA-Z0-9]+)/status method=GET params=page(int)`*** : read drug store activation status
```jsonc
{
  "activated": true
}
```
  
***<ins>Towns <ins> :*** 
  
- [ ] ***`url=/form method=GET params=page(int)`*** : list towns
```jsonc
{
  "towns": [
    {
      "id": 41,
      "label": "Abong-Mbang",       
       // .
       // .
       // .
```
<!--     
      "timecreated":0
      "timemodified":0
      "country":"Cameroon"
      "region":"Adamawa"
    },   
-->
```jsonc
       // .
       // .
       // .
  ],
  "page": 1,
  "maxpage": 2
}
```
  
***<ins>User <ins> :*** 
  
- [ ] ***`url=/user/([A-Za-z0-9\=\+/]+) method=GET`*** : read user information
  

**2.Security**

The system is built to communicate only with authentified user : `linker`, `mobile` and `doc`.
