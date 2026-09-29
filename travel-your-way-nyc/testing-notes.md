# Testing Notes
## Browser tests
I tested the final website in my browser. The file was called `4.html` during testing and is saved as `index.html` in this project. These are my manual checks, separate from the earlier AI-assisted code tests.
| Test | What I did | What I expected | What happened |
| --- | --- | --- | --- |
| With and without interests | Generated a three-day trip, then cleared all interests and generated again. | Both should generate activities if the time and budget allow. | Both worked. Leaving interests empty no longer gave me an empty plan. |
| Lunch scheduling | Generated a seven-day trip with Packed pace and checked the meals. | A food-market meal should count as lunch without an extra lunch charge. | I did not see the earlier problem of two lunches in a row. |
| Editing | Added, removed, reordered, and moved activities between days. | Times and costs should update, and moving a place should not duplicate it. | The schedule and costs updated, and moved activities appeared only on the new day. |
| Budget | Set the trip budget to $30, generated a plan, then added Empire State Building for $45. | The generated plan should stay within budget. Adding an activity over budget should keep it in the plan and show a warning. | The generated plan cost $18. After the addition, the total became $63, which was $33 over budget. The warning appeared and the activity stayed in the plan. |
| Saving and maps | Refreshed the page and opened several place and directions links. | My plan should return, and the links should open the correct places or routes. | The plan was restored, and the links I checked opened the intended locations. |
## Changes made before these tests
AI-assisted reviews helped identify several problems in earlier versions. I used those findings to ask for changes.
1. Some routes went back and forth between areas. The rules were adjusted to keep nearby places together while allowing visits to neighboring areas.
2. Free activities could still lead to an over-budget plan because of meal costs. Meals were added to the budget check.
3. Lunch could cause long waits or two meals in a row. The planner was changed to check the schedule again after adding lunch.
4. Leaving all interests unchecked could produce empty days. The planner now makes recommendations without requiring an interest selection.
5. Nearby cafés and shops used to go at the end of the day. They now go after a relevant attraction.
## Limits of my testing
These checks worked as expected, but I did not test every combination of settings or every browser and device. I checked several Google Maps links, not all of them.
I also did not confirm current prices, opening hours, or actual travel times. The website is a class prototype, and those details would still need to be checked before a real trip.
