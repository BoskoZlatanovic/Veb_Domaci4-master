Choose Your Food - Meal Selection Application
Project Overview

This application enables users to select meals for each weekday from a predefined set of options. This system helps the client prepare the necessary meal quantities for the upcoming week based on user selections.
Features
Meal Selection

    Daily Meal Choices: Users can choose from three different meal options for each weekday through a dedicated selection form. All fields are mandatory.
    Confirmation: Upon confirming their choices, users' selections are saved, and they are redirected to a confirmation page.

Order Management

    Order Summary: A separate page for the client displays the total number of meals ordered for each day, grouped by the meal type.
    Reset Functionality: The client can delete all entries to allow users to make new selections for the next period.

Technical Requirements

    Servlet API: The web application must be developed using the Servlet API.
    Meal Data Loading: Meal options for each day are loaded from respective text files (e.g., monday.txt, tuesday.txt) at server startup. Meals are listed line-by-line in these files.
    Session Management: Users can select meals only once per session. Once a form is submitted, users should receive a message if they try to access the selection page again, showing their chosen meals until all orders are reset.
    State Persistence: The current state of the application (loaded meals and user selections) should be stored at the servlet instance level.
    Frontend: Developers have the freedom to enhance the frontend using libraries of their choice.
    Secure Access: Access to the selected meals page is password-protected, provided as a query parameter (/selected-meals?password={password}). The valid password is loaded from a file (password.txt) during servlet initialization.
