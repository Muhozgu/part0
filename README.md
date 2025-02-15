# part0

 Diagram Structure:
User Interface (Frontend)

[User] → Clicks "New Note" button
[SPA] → Displays note creation form (without page reload)
[SPA] → Captures form input and sends a POST request (/api/notes)
Backend (Server/API)

[API] → Receives the POST request
[API] → Saves the new note to the database
[API] → Returns a JSON response with the created note
Frontend Update (Without Page Reload)

[SPA] → Updates the note list immediately (optimistic update)
[SPA] → Displays success message or handles errors if needed
