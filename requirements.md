# Software Requirements

## Vision

- What is the vision of this product?

> Refrigerator social application that allows users to track what is in their refrigerator and the date it entered.  Also able to view other community members refrigerators and either message or comment.

- What pain point does this project solve?

> This application will be focused on reducing food waste in a community.  This app will provide visibility to a user about what foods are nearing their expiration and should be used, and will also have a social aspect that will allow for local bartering of ingredients among  neighbors.

- Why should we care about your product?

> We should care about this project because food waste is a persistent problem that can only be solved through community action. Our goal is to create an application that helps make it easier for individuals to find consumers for their food which would otherwise be spoiled, and to gain access to other community members who may be looking to get rid of some of their food as well.

## Scope

- In
  - Allow users to add and delete ingredients from their own refrigerator
  - Allow users to view other community members refrigerators and their contents
  - Allow commenting on other users refrigerators to propose transactions
  - Allow users to edit their personal information at any time
  - Allows an admin user to create, delete, or edit other user profiles
  - Allows users to view a full list of other application users in their area

- Out
  - Will not provide product specific information or dietary information
  - Will not allow for direct messaging functionality
  - Will not expose exact addresses to general community members
  - Will not link to any third party websites or API's


## Stretch
What stretch goals are you going to aim for?

- Community Feed of recent completed trades in the users area.
- Detailed search of ingredients from the user search page

## Functional Requirements

- An admin can create and delete user accounts
- A user can update their profile information
- A user can add and delete items from their refrigerator inventory
- A user can view all other users in their community
- A user can view a specific other users refrigerator and leave a comment
- Refrigerator owner can view comments made on their page.

## Data Flow

- When the user goes to our website, they will be greeted with a splash page with information about how the website works and a login and sign up buttons.
- Upon login, and verification using spring security, user will be pathed to their profile, where they can make changes to personal information, or reroute to view their refrigerator page.
- At the users refrigerator page, the user can view comments left by other users, add items to their refrigerator, and delete items from their refrigerator.
- Nav links at the top by template for all authorized pages, user can navigate to the all users index page and view other community members.  From the community members page, a user can path to a specific users refrigerator to view and interact with its contents.
- Upon logout, user is rerouted back to home splash page.

## Non Functional Requirements

- Security: We will utilize Spring security for this application which will protect against SQL injection and cross site scripting.  All user passwords will be hashed and salted prior to storage (no plain text pw's)
- Testability: We will create unit and integration tests for all major features of the application.  This will at minimum include:
  - Creating a user
  - Editing a user
  - Creating an ingredient
  - Deleting an ingredient
  - Creating a comment
  - Deleting a comment
