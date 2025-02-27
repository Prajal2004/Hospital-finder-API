# Hospital Finder API

## Introduction
The Hospital Finder API is a FastAPI-based service that helps users find nearby hospitals using their geographic location. It integrates with Google Maps Places API to fetch hospital details such as name, address, rating, and contact information.

## Features
- Fetches nearby hospitals based on latitude and longitude.
- Provides details like hospital name, address, rating, and Google Maps link.
- Uses Google Maps Places API for accurate data.

## Installation
### Prerequisites
- Python 3.8+
- FastAPI
- Uvicorn
- Requests library

### Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/hospital-finder-api.git
   cd hospital-finder-api
   ```
2. Install dependencies:
   ```sh
   pip install fastapi uvicorn requests
   ```
3. Set up your API key for Google Maps:
   - Replace `YOUR_GOOGLE_MAPS_API_KEY` in the code with your actual API key.

## Usage
### Running the API
Start the FastAPI server using Uvicorn:
```sh
uvicorn main:app --reload
```
The API will be available at `http://127.0.0.1:8000`.

### Example Request
```sh
GET /find-hospitals?latitude=37.7749&longitude=-122.4194
```

### Example Response
```json
{
  "hospitals": [
    {
      "name": "General Hospital",
      "address": "123 Main St, City",
      "rating": 4.5,
      "contact": "N/A",
      "maps_link": "https://www.google.com/maps/place/?q=place_id:XYZ"
    }
  ]
}
```

## Deployment
To deploy the API on a cloud platform like Heroku or AWS, follow their respective deployment guides.

## License
This project is licensed under the MIT License.

## Contact
For issues or improvements, please open an issue in the GitHub repository.

---

_Contributors are welcome!_ 🚀
