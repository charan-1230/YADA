YADA - Yet Another Diet Assistant
=================================

OVERVIEW
--------
YADA is a diet tracking application that allows users to:
- Track daily food consumption and calorie intake
- Browse and search a database of basic and composite foods
- Create custom foods and recipes
- Calculate nutritional needs based on personal data

TECHNICAL DETAILS
-----------------
- Language Used : JAVA
- DataBase Format : JSON

OBJECT-ORIENTED PROGRAMMING (OOPS) USAGE
----------------------------------------
YADA is designed using core Object-Oriented Programming principles:
- **Encapsulation:** User, Food, and Diet Log data are managed through dedicated classes, keeping data and related methods together.
- **Abstraction:** Complex operations (like nutritional calculations and food management) are abstracted into methods and classes, hiding implementation details from the user.
- **Inheritance:** Food types (e.g., BasicFood, CompositeFood) are implemented as subclasses, allowing code reuse and extension.
- **Polymorphism:** The application can handle different food types and user actions through common interfaces and method overriding.


RUNNING THE APPLICATION
----------------------
1. Ensure Java is installed on your system (JDK 11 or later recommended)
2. Make sure to have JVM installed on your system
3. Make sure to have Maven installed on your system
4. Ensure you did maven clean
5. choose run java option by right clicking on App.java

Note: The application requires the json-simple library in the lib directory.

FEATURES AND HOW TO USE THEM
----------------------------

1. USER ACCOUNT MANAGEMENT
   - Sign up: Create a new account with your personal information
   - Login: Access your account with your username and password
   - Profile Management: Update your physical attributes and activity level

2. FOOD DATABASE
   - Browse foods by category (Dairy, Protein, Grains, Vegetables, Fruits, etc.)
   - Search foods by name or keywords
   - View detailed nutritional information for any food

3. CUSTOM FOOD CREATION
   - Add new basic foods with your own calorie information
   - Create composite foods (recipes) from existing foods
   - All custom foods are saved to your account

4. DIET DIARY
   - Log food consumption for any date
   - View daily calorie intake
   - Edit or delete existing entries
   - Undo recent actions

5. NUTRITIONAL NEEDS CALCULATOR
   - Calculate your Basal Metabolic Rate (BMR)
   - Get personalized calorie intake recommendations
   - Analyze your current diet against your goals

FOOD LOGGING BEHAVIOR
-------------------
When adding the same food to your diet log for the same day:
- The application will update the existing entry by adding the new servings
- For example, if you already logged 2 servings of an apple, then log 1 more serving,
  the entry will show 3 servings total instead of creating a duplicate entry

DATA STORAGE
-----------
The application stores data in three JSON files:
- userDatabase.json: User account information
- foodDatabase.json: Food items (both default and custom)
- dietLog.json: User food consumption logs

These files are automatically created in the application directory.

TIPS FOR BEST EXPERIENCE
----------------------
1. Save your database regularly using the "Save Database" option
2. Use detailed keywords when creating custom foods for better search results
3. Break complex recipes into their component ingredients for more accurate tracking

FUTURE IMPROVEMENTS
-------------------
- The design supports easy extension for importing food data from external websites.