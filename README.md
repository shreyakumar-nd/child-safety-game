# Online Safety Learning Game

An interactive online safety education game for children, parents, caregivers, and teachers. The project uses scenario-based role play to teach safer responses to online grooming, exploitation risks, and other child safety concerns.

## About

Players choose one of three roles:

- **Parent**: Navigate decisions about keeping children safe while supporting healthy internet access.
- **Child**: Practice recognizing risky online interactions and making safer trust decisions.
- **Teacher**: Respond to concerning student situations while preserving trust and involving appropriate support.

The experience includes sensitive material about online harm, grooming, exploitation, and child safety. Younger participants should use it with an informed, trusted adult nearby.

## Project Structure

```text
.
├── index.html          # Landing page and role selection
├── css/
│   ├── main.css        # Twine/game styling support
│   └── site-theme.css  # Main site theme
├── images/            # Homepage and role-selection assets
└── pages/
    ├── child.html     # Child role game
    ├── parent.html    # Parent role game
    └── teacher.html   # Teacher role game
```

## Run Locally

This is a static site. No package install or build step is required.

Open `index.html` directly in a browser, or serve the folder with a local static server:

```bash
python3 -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Main Files

- `index.html`: Homepage, navigation, resource links, and role cards.
- `pages/*.html`: Self-contained Twine/Harlowe game exports for each role.
- `css/site-theme.css`: Site layout, theme colors, homepage components, and responsive styling.
- `css/main.css`: Shared game styling support.

## External Dependencies

The homepage loads Bootstrap 5.3.3 from the jsDelivr CDN. The role games are exported as self-contained HTML files.