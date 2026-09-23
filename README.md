# T01 (a): Build Appliance Energy Consumption Website

Built for **COS30045 Data Visualisation**, Swinburne University of Technology,
Sarawak Campus.

## Data Story 
This section of the site tells a story for people shopping for a new TV who want to understand what it will actually cost to run before they buy. Rather than just showing raw numbers, the Televisions page walks through all six of the questions explored in T02: what screen technologies are most common, what screen sizes are most common, which brands have the most models, which technology uses the least power, how screen size affects running cost, and whether a higher star rating is worth paying for.

## About the Data 
### Data source 
The Australian Government's GEMS (Greenhouse and Energy Minimum Standards) Energy Rating register for televisions, found via data.gov.au. The export used here is dated 6 September 2026 and covers 5,018 registered TV models. 
### Data processing 
The raw data was cleaned and transformed in KNIME: unused/empty columns were dropped, duplicate model registrations were removed (keeping only the most recently submitted version of each model), and the data was filtered to only currently available models sold in Australia. Screen size was converted from the register's centimetre measurement to inches.
### Privacy 
This dataset describes television products, not individuals. It contains no personal or identifiable information about any person, so there are no personal privacy concerns with this data. 
### Accuracy and limitations 
Estimated running costs assume a flat $0.33/kWh electricity price, a rough 2026 national average; real bills vary by state, retailer and tariff. The "labelled energy consumption" figures come from standardised test conditions, not real household usage, which will vary. The data reflects a single snapshot in time (September 2026) and does not include models registered afterward. ### Ethics All figures shown are calculated directly from the real dataset, with assumptions (like the electricity price) stated clearly rather than hidden. No brand is singled out unfairly. The same calculations are applied equally across all models and brands in the dataset.

### How I used GenAI
I used Claude to help generate the site's HTML, CSS and JavaScript. 
I reviewed everything it produced against the assignment's requirements,
and asked for changes where something didn't match what was asked.

### Reflection
The trickiest part to follow at first was the JavaScript that swaps between pages when a nav link is clicked. I couldn't immediately see how everything connected. I asked about one specific line of code, the data-page attribute on a nav link and that was enough to make the rest of the logic click. More broadly, I asked for several things to be simplified or removed along the way. Not because they were wrong, but because I wanted to stay confident I could explain everything in the final result. That approach worked well, and it's one I'd repeat: ask for an explanation of a specific piece of code whenever something doesn't immediately make sense, rather than moving on without actually following it.
