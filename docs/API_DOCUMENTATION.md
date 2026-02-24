# API Documentation

## Base URL

All API endpoints are versioned under:

http://localhost:8000/api/v1

---

# 1. VIN Decoder API

## Endpoint

GET /vin/decode/{vin}

## Description

This endpoint decodes a 17-character Vehicle Identification Number (VIN) and returns structured vehicle details.

## Example Request

GET /api/v1/vin/decode/1HGCM82633A004352

## Example Response

{
  "vin": "1HGCM82633A004352",
  "manufacturer": "Honda",
  "country": "Japan",
  "model_year": 2003,
  "vehicle_type": "Passenger Car"
}

## Error Response Example

{
  "detail": "Invalid VIN format"
}

---

# 2. FAQ API

## Endpoint

POST /faq

## Description

This endpoint accepts a question related to automotive concepts and returns an appropriate answer.

## Request Body

{
  "question": "What is an engine?"
}

## Example Response

{
  "answer": "The engine is the heart of the car. It converts fuel into mechanical power."
}

## Fallback Response

If the question is not recognized:

{
  "answer": "Sorry, I don't have information about that yet."
}
