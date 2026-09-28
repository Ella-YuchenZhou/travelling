# Travel Your Way — New York
## Project idea
I enjoy traveling, so I wanted to make a tool that helps visitors organize a New York trip. Users can plan one to seven days based on their budget, interests, and pace, then change the plan themselves.
## Core interaction
When users generate or edit an itinerary, the schedule, estimated costs, and warnings update automatically. They can add, remove, reorder, or move places between days. They can also add nearby food and shopping stops and open locations or directions in Google Maps.
## How to use it
1. Download and unzip the repository.
2. Open index.html in a browser.
3. Choose your trip length, daily hours, budget, interests, starting area, pace, and lunch preferences.
4. Select any must-see places and click Generate my itinerary.
5. Review and adjust the plan.
No installation is needed. Planning works offline, but external links need internet access. Plans are saved in the current browser when local storage is available.
## Design choices
I wanted to keep nearby places together while letting users make their own choices. Different pace options leave more or less time for breaks. Nearby cafés and shops are optional, and a restaurant can replace a planned lunch.
I used taxi yellow, dark colors, green accents, and New York landmark illustrations to give the page a connection to the city.
## AI tools and selected prompts
I used Codex to build and revise the website and ChatGPT to help organize my ideas and review the code. These are excerpts from prompts I used.
### Planning goals
My two main design goals are to reduce unnecessary backtracking and give users control over their plans.
### Route changes
Prefer activities in the same area first. If no suitable activities remain there, consider nearby areas using distance and estimated travel time, while still checking interests, opening hours, budget, and pace.
### Lunch fix
Check lunch coverage after all schedule changes, not just before inserting a break. If a food-market visit serves as lunch, do not add a separate lunch allowance.
## Testing
I completed five browser checks covering generation with and without interests, lunch scheduling, itinerary editing, budget warnings, and saving and map links. The tested cases worked as expected. My results are in testing-notes.md.
## Reflection
At first, I thought asking AI to group nearby places would be enough. During AI-assisted reviews, some routes still went back and forth between areas. Stricter rules reduced this, but then one day had only the High Line. I asked the planner to consider nearby areas too. This made me think more carefully about what I meant by a “good itinerary.” I wanted to reduce travel time, but I also wanted each day to feel useful without being too busy.
Lunch caused another problem. Adding a lunch break could push a food-market visit into lunchtime, creating two meals in a row. I asked AI to check the final schedule again instead of just removing a charge. My final browser checks worked as expected, but I still do not understand every line of code. AI helped me build and check the project, while I decided which results made sense and what needed changing. The prices, hours, and travel times still need confirmation before a real trip.
## Limitations
1. Prices and opening hours are examples. Closures, reservations, and ticket availability are not fully handled.
2. Travel times are estimates. Google Maps opens separately and does not update the planner.
3. The place collection is limited. Nearby shops and cafés mainly cover Midtown and Chelsea/Meatpacking.
4. The budget includes listed activities and food, but excludes accommodation, flights, transportation, shopping, taxes, and tips.
5. The schedule does not include returning to accommodation.
6. Saved plans do not sync across devices. My tests do not cover every possible itinerary.
## Files
1. index.html — website
2. README.md — project description and reflection
3. testing-notes.md — test results