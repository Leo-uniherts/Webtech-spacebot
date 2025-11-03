# 🚀 Space Bot API Investigation Sheet

**Total Marks: 30**  
**Part 1: Collect Required API Documentation**

This investigation sheet helps you gather key technical information from the three APIs required for the Space Bot project: **Webex Messaging API**, **ISS Current Location API**, and a **Geocoding API** (LocationIQ or Mapbox or other), plus the Python time module.

---

## ✅ Section 1: Webex Messaging API (7 marks)

| Criteria | Details |
|---------|---------|
| API Base URL | `https://webexapis.com/v1` |
| Authentication Method | `API key` |
| Endpoint to list rooms | `https://webexapis.com/v1/rooms` |
| Endpoint to get messages | `https://webexapis.com/v1/messages` |
| Endpoint to send message | `https://webexapis.com/v1/messages` |
| Required headers | `The API key and the json` |
| Sample full GET or POST request | `PostData = {
                            "roomId": room["id"],
                            "text": responseMessage
                        }' |

---

## 🛰️ Section 2: ISS Current Location API (3 marks)

| Criteria | Details |
|---------|---------|
| API Base URL | `http://api.open-notify.org/iss-now.json` |
| Endpoint for current ISS location | `http://api.open-notify.org/iss-now.json` |
| Sample response format (example JSON) |  Json - the ISS was flying over a body of water at latitude -1.4638° and longitude 58.3433°.
```

```
|

---

## 🗺️ Section 3: Geocoding API (LocationIQ or Mapbox or other) (6 marks)

| Criteria | Details |
|---------|---------|
| Provider used (circle one) | ** open weather api** |
| API Base URL | `https://api.openweathermap.org/data/2.5/weather?lat={lat}&lon={lng}&appid=[API Key]` |
| Endpoint for reverse geocoding | `https://api.openweathermap.org/data/2.5/reverse` |
| Authentication method | `API key` |
| Required query parameters | `roomID, ` |
| Sample request with latitude/longitude | `_______________________________` |
| Sample JSON response (formatted example) |  {
  "coord": { "lon": -95.3698, "lat": 29.7604 },
  "weather": [...],
  "main": { ... },
  "sys": { "country": "US" },
  "name": "Houston"
}
```

```
|

---

## ⏰ Section 4: Epoch to Human Time Conversion (Python time module) (2 marks)

| Criteria | Details |
|---------|---------|
| Library used | `datetime` |
| Function used to convert epoch | `time.ctime()` |
| Sample code to convert timestamp |  timeString - time.ctime(timestamp)
```  
```
|
| Output (human-readable time) | `On Mon Oct 27 08:32:51` |

---

## 🧩 Section 5: Web Architecture & MVC Design Pattern (12 marks)

### 🌐 Web Architecture – Client-Server Model

- **Client**: 
- **Server**: 
- (Explain the communication between them & include a block diagram )

### 🔁 RESTful API Usage
REST API enables client and server communication over HTTP with standard requests and responses.
- 
- client -> http, URL -> Server
  ^                        l
  l                        V
     <-------------    json
- 

### 🧠 MVC Pattern in Space Bot

| Component   | Description |
|------------|-------------|
| **Model**  |handles the data and business logic  |
| **View**   |handles the presentation and output  |
| **Controller** | handles the input and the flow logic, coordinating between model and view |


#### Example:
- Model: the code to request the data
- View: code to print the data
- Controller: the code that manages the data in the while true loop

---

### 📝 Notes

- Use official documentation for accuracy (e.g. developer.webex.com, locationiq.com or Mapbox, open-notify.org or other ISS API).
- Be prepared to explain your findings to your instructor or demo how you retrieved them using tools like Postman, Curl, or Python scripts.

---

### ✅ Total: /30
