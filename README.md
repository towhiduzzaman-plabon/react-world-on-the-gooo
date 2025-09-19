Programming Hero Countries API
Endpoints

https://openapi.programming-hero.com/api/all
https://openapi.programming-hero.com/api/alpha/116
https://openapi.programming-hero.com/api/lang/english
https://openapi.programming-hero.com/api/name/bangladesh
Usage

// Fetch all countries
fetch("https://openapi.programming-hero.com/api/all")
  .then((res) => res.json())
  .then((data) => console.log(data));

// Fetch country by ISO code
fetch("https://openapi.programming-hero.com/api/alpha/116")
  .then((res) => res.json())
  .then((data) => console.log(data));

// Fetch countries by language
fetch("https://openapi.programming-hero.com/api/lang/english")
  .then((res) => res.json())
  .then((data) => console.log(data));

// Fetch country by name
fetch("https://openapi.programming-hero.com/api/name/bangladesh")
  .then((res) => res.json())
  .then((data) => console.log(data));
Getting Started
To set up this project locally:

Clone the repository

Install dependencies (if any)

e.g. npm install or yarn install
Create any configuration file if needed (e.g. for environment variables)

Run the app

e.g. npm start
Example Responses
Here are example shapes of JSON responses you may get (fields may vary):

/api/all
[
  {
    "name": "Afghanistan",
    "alpha2Code": "AF",
    "alpha3Code": "AFG",
    "capital": "Kabul",
    "region": "Asia",
    "population": 40218234
    // ... more fields
  },
  {
    "name": "Albania",
    "alpha2Code": "AL",
    "alpha3Code": "ALB",
    "capital": "Tirana",
    "region": "Europe",
    "population": 2877797
    // ...
  }
  // ... many more
]
/api/alpha/116
{
  "name": "Country-Name",
  "alpha2Code": "XX",
  "alpha3Code": "XXX",
  "capital": "...",
  "region": "...",
  "population": ...,
  // ... other details
}
/api/lang/english
[
  {
    "name": "United Kingdom",
    "alpha2Code": "GB",
    "capital": "London"
    // ...
  },
  {
    "name": "United States of America",
    "alpha2Code": "US",
    "capital": "Washington D.C."
    // ...
  }
  // ... more countries
]
/api/name/bangladesh
[
  {
    "name": "Bangladesh",
    "alpha2Code": "BD",
    "alpha3Code": "BGD",
    "capital": "Dhaka",
    "region": "Asia",
    "population": ...,
    // ...
  }
]
