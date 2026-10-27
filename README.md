# ALTROVE
ALTROVE — An AI-powered travel itinerary planner that transforms your dream destinations into personalized journeys based on your budget, preferences, and travel duration

# ✈️ ALTROVE

### Your Journey. Your Budget. Your Perfect Plan.

ALTROVE is an AI-powered travel itinerary planner that helps
users create personalized travel plans based on their destination,
budget, trip duration, and travel preferences.

Built using HTML, CSS, JavaScript, and the Google Gemini API.

## 🌍 Project Overview

Planning a trip often requires researching destinations,
estimating expenses, choosing attractions, and organizing
daily activities.

VoyageIQ simplifies this process by using generative AI
to create a personalized travel itinerary.

Users provide:
- Destination
- Total budget
- Currency
- Number of days
- Number of travelers
- Travel style
- Accommodation preference
- Special requirements

ALTROVE generates:
- Day-wise itinerary
- Morning, afternoon, and evening activities
- Estimated budget breakdown
- Recommended attractions
- Local food suggestions
- Packing checklist
- Travel tips
- Budget-saving recommendations

##  Features

### 1. AI Itinerary Generator

Uses the Google Gemini API to create personalized
travel itineraries.

### 2. Day-Wise Travel Planner

Displays a structured daily itinerary with:
- Morning activities
- Afternoon activities
- Evening activities
- Suggested locations
- Estimated activity costs

### 3. Smart Budget Analyzer

Compares the user's budget with estimated trip expenses.

Expense categories:
- Accommodation
- Food
- Local transportation
- Activities
- Miscellaneous

Displays whether the trip is estimated to be within budget.

### 4. Destination Explorer

Displays recommended tourist attractions and local
food experiences.

### 5. Interactive Packing Checklist

Users can mark items as packed.

Checklist progress is saved with a saved trip.

### 6. Saved Trips

Uses browser localStorage to save generated itineraries.

Users can:
- Save trips
- Reopen trips
- Delete individual trips
- Clear saved trips

### 7. Download Itinerary

Downloads a generated itinerary as a TXT file.

### 8. Dark and Light Mode

Supports two visual themes.

### 9. Travel Dashboard

Displays:
- Number of trips generated
- Total travel days planned
- Number of saved trips

### 10. Responsive Design

Works on desktop, tablet, and mobile screens.

## 🛠️ Technology Stack

| Technology | Purpose |
|------------|---------|
| HTML5 | Website structure |
| CSS3 | Styling and responsive design |
| JavaScript | Application functionality |
| Gemini API | AI itinerary generation |
| Fetch API | HTTP requests |
| Async/Await | Asynchronous operations |
| JSON | Structured AI responses |
| localStorage | Saved trips and preferences |
| DOM API | Dynamic content rendering |

## 📁 Project Structure

```text
VoyageIQ/
├── index.html
├── style.css
├── script.js
├── README.md
└── .gitignore
```

## 🚀 How to Run

1. Clone or download the project.
2. Open the folder in Visual Studio Code.
3. Install the Live Server extension.
4. Open index.html with Live Server.
5. Create a Gemini API key using Google AI Studio.
6. Open API Settings in VoyageIQ.
7. Enter your API key.
8. Fill in the trip details.
9. Click Generate My Itinerary.

## 🤖 Gemini API Integration

VoyageIQ uses the Gemini REST API.

The application sends an HTTP POST request using fetch().

Example:

```javascript
const response = await fetch(API_URL, {
  method: "POST",
  headers: {
    "Content-Type": "application/json",
    "x-goog-api-key": apiKey
  },
  body: JSON.stringify(requestBody)
});
```

The application uses async/await to handle asynchronous
API requests.

The AI response is parsed as JSON and validated before
displaying the generated itinerary.

## 💾 Local Storage

VoyageIQ uses localStorage to store:

- Saved trips
- Trip generation statistics
- Selected theme
- Optional API key preference

Data is stored locally in the user's browser.

## ⚠️ Important Limitations

- AI-generated prices are estimates.
- The application does not provide live hotel or flight prices.
- The application does not make reservations.
- Opening hours and attraction availability must be verified.
- Budget estimates may exclude travel to the destination.
- The API key is sent directly from the browser.
- Browser storage is not a secure location for production API keys.

##  Future Improvements

- Interactive maps
- Live weather information
- PDF itinerary export
- Cloud-based trip storage
- User authentication
- Real-time accommodation pricing
- Collaborative trip planning

## 👩‍💻 Author

Developed as a Web Technology project.

## 📜 License

Created for educational purposes.
