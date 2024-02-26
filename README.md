# Flight Finder 

A website that gives you real-time details on current flights.

---

## Deployment Steps

Testing.

1. Download this project folder or `git clone` the repo
2. Open terminal, cd to this project's root directory
3. Run `npm install` 
4. Run `npm run dev`
5. Open the localhost URL that appears in the terminal

---

## Assumptions and Limitations

1. I couldn't use the AviationStack API as it doesn't allow any https requests on a free subscription. Looked around and found airlabs.co, whose API seemed like the best free option and has most of the details needed.
2. The AirLabs API doesn't accept latitude, longitude, and status as request params though, so to implement those filters I retrieved all records and then filtered the array. This has affected the website's performance.
3. The user-facing input form only accepts IATA codes for airlines and airports and not their full names for now. (You can only enter "AA" and not "American Airlines" to get a valid response. Same for airports - only "IAD" and not "Dulles International" will work.)
4. The website only displays the flight number, departure and arrival, and status of the queried flights. I've abstracted out the other details for now.
