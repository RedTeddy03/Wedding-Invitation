# Wedding Invitation

A simple, elegant, static wedding invitation website built with HTML, CSS, and JavaScript.

The project has two main pages:
- `index.html`: envelope landing page
- `invitation.html`: full invitation experience

## Features

- Envelope opening screen that redirects to the invitation page
- Fully styled wedding invitation layout
- Countdown timer to event date and time
- Direct call buttons for contact persons
- Google Maps location button
- Background music (`song.mp3`) configured to loop
- Mobile responsive behavior with dedicated media queries

## Tech Stack

- HTML5
- CSS3
- JavaScript (Vanilla)
- Bootstrap 5 (CDN)
- Bootstrap Icons (CDN)
- Google Fonts (CDN)

## Project Structure

```text
Wedding-Invitation/
|- index.html
|- invitation.html
|- try.html
|- song.mp3
|- css/
|  |- index.css
|  `- invitation.css
|- js/
|  |- index.js
|  `- invitation.js
`- Images/
   `- (all image assets)
```

## Run Locally

Because this is a static project, you can run it in either of these ways:

1. Open `index.html` directly in your browser, or
2. Serve with a local static server (recommended for consistent behavior).

Example using VS Code Live Server or any static server:

```bash
# from project root
# choose one option:
npx serve .
# or
python -m http.server 5500
```

Then open:
- `http://localhost:5500/index.html`

## Configuration and Customization

### 1) Bride and Groom Details
Edit text content in `invitation.html`:
- Couple names
- Parent names
- Event date and day
- Schedule timeline
- Prayer section content

### 2) Countdown Date and Time
Update the date in `js/invitation.js`:

```js
const weddingDate = new Date('2026-07-18T11:00:00').getTime();
```

Use ISO format for best compatibility.

### 3) Location Button
Update the Google Maps URL in `invitation.html`:

```html
onclick="window.open('https://www.google.com/maps/search/?api=1&query=Royal+Gallery+Tuanku+Ja%27afar')"
```

### 4) Contact Buttons
Update phone numbers in `invitation.html` in the `tel:` links and labels.

### 5) Images and Branding
Replace files in `Images/` while keeping filenames the same, or update file references in:
- `index.html`
- `invitation.html`
- `css/index.css`
- `css/invitation.css`

### 6) Background Music
Replace `song.mp3` with your preferred audio file and keep the same filename, or change the `src` in `invitation.html`.

## Notes

- This project uses CDN resources (Bootstrap, Icons, Google Fonts), so internet access is needed for those assets.
- Auto-play behavior for audio depends on browser policy; user interaction is usually required.

## License

Personal-use project. Add a formal license section if you plan to distribute or open-source it.