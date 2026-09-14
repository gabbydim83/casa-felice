# Casa Felice – Explore Brașov Template Type 1

Website demo for a guesthouse / villa with multiple rooms, built without assuming an unconfirmed number of rooms.

## Files
- `index.html` – public website, self-contained HTML + CSS + JavaScript
- `owner.html` – owner management demo, self-contained
- `images/` – local Casa Felice photography
- `serve.bat` / `serve.ps1` – local server helpers

## Run locally
Double-click `serve.bat`, then open `http://localhost:5500`.

## Explore Brașov data
The public page loads city, activities, restaurants, places, top destinations, guest services and transport providers directly from:
`gabridim18-lab/explore-brasov-data`

Weather is requested live from Open-Meteo using the coordinates stored for Brașov.

## Booking / availability demo
The public booking calendar is a date-request calendar. It does **not** claim final room availability because the exact room inventory for Casa Felice has not yet been confirmed.

`owner.html` can:
- store direct booking requests / reservations locally;
- optionally label a reservation with a room/unit later;
- block date ranges for the entire property;
- store Booking.com / Airbnb iCal URLs as future connection settings.

The public calendar only marks dates unavailable when the owner explicitly creates a **full-property block**.

Before production, add authentication and a shared backend or iCal/channel-manager synchronization if the owner purchases management functionality.
