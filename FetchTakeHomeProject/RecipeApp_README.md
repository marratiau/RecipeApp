Fetch Recipe App – Take Home Project

# Summary
A SwiftUI app that retrieves and lists recipes from a remote JSON API. The user can:
- View and filter recipes by cuisine
- View full recipe details
- Add and edit their own recipes (locally stored)
- Search by name or cuisine
- Refresh to retrieve the latest from API

Link to video demo: https://drive.google.com/file/d/1O_yFAT7k2vaZXv24A7mGrQ3MLCGaDrVB/view?usp=sharing

# Focus Areas
- Correct API integration using Swift Concurrency (`async/await`)
- Trying to maintain a clean, modular SwiftUI architecture (MVVM)
- Manual image caching to disk with no external dependencies
- Adding features like add recipes and filter recipes by cuisine.

# Time Spent
~Approximately 7 days total:

12-14 hours on networking, JSON decoding, creating the model layer (RecipeModel) and adding async/await logic to RecipeNetworkCaller and RecipeViewModel. A lot of this time was figuring out how to organize the data and get it loading properly.

8-10 hours on UI architecture in SwiftUI: creating the main screens such as IntroMenuView, RecipeListView, RecipeDetailView, and connecting them through NavigationStack using MVVM.

6–8 hours incorporating additional features like image caching, cuisine filtering, and search functionality — all of which required coordination across the model, view model, and views.
 
6–7 hours on incorporating and editing recipes locally (including local JSON persistence, image handling, sorting and alphabetization logic), ensuring consistency everywhere in the app.
 
5–6 hours on polish and testing: bug fixing (including image persistence and filter problems), adding unit tests, UI tweaks, and final cleanup.


# Trade-offs & Decisions
- Used local JSON persistence for new/edited recipes instead of server upload

# Weakest Part of the Project
- No integration or UI testing
- Local additions don't get synced with server (as it is read only)


It was really fun doing this and definitely challenged my skills and knowledge. I learned a lot in the process.