# [MasterMindIQ](https://adampillis.github.io/MasterMind-IQ-Challenege/)

## 1. **Introduction**

### **What is it?**
MasterMindIQ is a general quiz designed to test the general knowledge of young adults from around the age of 16 and upwards. 
- The quiz application has a difficulty section of three levels and five general categories for the players to chose from to their liking.
- Each game consists of 10 questions with a player feedback at the end of each game which are score number specific. 

The **Project Aim** was to design a game that most age groups of online user can play if they wish so. *MasterMindIQ* was also designed to be as *interactive *with its players as possible and allowing them to *fully control* the type of game they each wish to play.
 A quiz game was chosen for this reason and five categories were included with three difficulty levels to match the interest and knowledge level of each player. The category topics are general rather than being specific to give players the opportunity and like the quiz game. If one can't answer any question because they're too related, they may lose interest and never return in the future. 

 ### **How it works?**
 1. The landing page welcomes the user and automatically starts interacting with them by asking them to enter their player name and either click the button or press 'Enter'. 
 2. This is followed by the menu page with a personalised message at the top with details taken from the form of the landing page. Underneath, each player can chose a difficulty level (easy level is automatically checked) followed by five general categories to include the interest of most players. 
 3. Once the player has clicked on their chosen category, a rule page pops up to explain the rules of the game before the actual game begins. The game includes a player score board showing the score, question number and number of incorrect answers. This is followed by the question and four possible answers with only one correct answer.
 4. Once the game is finished, i.e 10 questions have been answered, each player jumps to the end user feedback page where a warm welcome message awaits followed by their score number and based on that, a specific end comment. 

 ### **Who is it for**
The target audience is global and any user from the age of 16 has good potential to get a couple of questions correct. Another reason the creator build a quiz game was to include all age groups of the global target audience. 

**New User** : Each new user has the ability to play up to 15 games with different questions if they so wish. Each of the 5 categories consist of 3 levels of 10 questions. A young adult with secondary school knowledge should have the knowledge to test themselves on easy levels while medium and hard levels are designed for older generations. The landing page asks each player to enter a player name to personalise the game. 

**Returning User** : The chances of playing all 15 games during their first visit is low which means that as a returning user, other categories can be played at several difficulty levels. One of the first updates of this potential quiz game would be to implement APIs and expand the question database of each category to enhance the number of returning users. 

![Introduction Image](assets/images/landing-page-screenshot.PNG "Introduction page/landing page")

### **Planning**

The planning process started by designing one html page (**index.html**) with each page represented by a section. CSS and Javascript was then used to hide and display depending on what the user is clicking on. 

**1. Start-Screen Section**

**INCLUDE SCREENSHOT**

**2. Menu-Screen Section**

**INCLUDE SCREENSHOT**

**3. Rule-Screen Section**

**INCLUDE SCREENSHOT**

**4. Game-Screen Section**

**INCLUDE SCREENSHOT**

**5. Exit-Screen Section**

**INCLUDE SCREENSHOT**

**6. End-Screen Section**

**INCLUDE SCREENSHOT**

The creator has also made a rough sketch of functions he is going to use within his *script.js* to make the quiz game work. 

**Planning Functions Sketch**

**INCLUDE SCRENSHOT OF FUNCTIONS**

**Planning Colours**
The creator used [coolors.co](https://coolors.co/palettes/trending) website to chose six colors including a neutral body color, red for incorrect, green for incorrect and the rest for other parts and buttons. The colors he chose are as follows and used **hsl** in this project to test it out. 

![Project Colours](assets/images/project-colors-screenshot.PNG "Project colours")

In terms of screen sizes, the creator used *flex-display* through each section to ensure that the game looks identical on every screen-size. As a result, the sketches for each section above also represent smaller and bigger screens using flex and different font and buttons sizes. 

## 2. **Features (existing)

### 1. **Landing Page**

#### *Header*
The *header* contains the quiz game's official name to the left and it is consistent by displaying in every page throughout the game.

![header](assets/images/header-screenshot.PNG "Project header")

#### *Landing page message*
Each user is greeted with a warm 'welcome message' followed by an inspiring quote which outlines one of the main functions of this project, *to test each visitor's general knowledge*.

![Landing page message](assets/images/landing-page-text-screenshot.PNG "Landing page message")

#### *Landing page submit form*
The quiz game starts interacting with each user as soon as they land on the page. The text input of the form is focused on to indicate the user their action is necessary to continue. They cannot proceed if the input is left empty. Above the text input, is a label to ensure the user knows what they need to enter. The language used is just in-between form and informal language for an equal balance. 
Once the above step is complete and the **Let's go** button is pressed, JavaScript is used to hide the land-screen section and display the main menu. In terms of contrast and user friendly design, the body color is used to style the button and the font-size also increases when hovered over. Javascript has also been used to allow the **Enter button** to also work as this can be an automatic action by some users.

![Form within landing page](assets/images/form-screenshot.PNG "Form within landing page")

### 2. **Menu Page**

#### *Menu - Personalised Message*
Once the user submit's their form with their nickname, the *welcome message* will include their chosen name using JS followed by a brief guide as to what is expected from the user in order to continue. Warm language is used to inspire the player to *want* to play the quiz. 

![Menu welcome message](assets/images/menu-message-screenshot.PNG "Menu welcome message")

#### *Difficulty level area*
Right under the welcoming message, there are three radio buttons - easy, medium and hard. The easy radio button is set to be checked automatically unless the user changes it to medium or hard. These radio buttons are used by JS to determine the difficulty level selected and this is one argument to source the correct array of questions. The styling has been kept clear and basic for ease of use by any age group. 

![Menu difficulty buttons](assets/images/difficulty-levels-screenshot.PNG "Menu difficulty buttons")

#### *Category Buttons*
Once the difficulty button is selected by the user, they each get to chose one of the five categories which is the second argument to determine which array of questions to use. The buttons use the same class to look identical with the same margin and padding. Each of these buttons is aria-labelled and have a unique ID which is linked with an event listener through JS. When hovered over, the text color changes and also increases in size for better visuals from a user perspective. 

![Menu category buttons](assets/images/category-buttons-screenshot.PNG "Menu category buttons")

### 3. **Rules Page**

#### *Rules Box*
Consists of 4 rules altogether with an interactive message with the player to ensure they are all set and ready to play. The creator ensured that the user is also aware of current *in-game* features above the question container where their score, question number and incorrect answers are stored and monitored by JS in some functions. 

#### *Let's Go Button*
This button starts the game by hiding the rules-section and displaying the game-screen page with the first question and possible answers. When hovered over, the **color** of the text and background changes to enhance visual looks for the user. 

![Rules screen section](assets/images/rules-screen-screenshot.PNG "Rules screen section")

### 4. **In-game Page**
#### *Game Screen Header*
Within this page, a 'Door icon' is added to the *right-hand corner* of the header. This enables the user to exit the game whenever they wish while giving them full control of their time spent on the web application. This is the only section or page that is shown with an additional header feature. 

![Header icon in game screen section](assets/images/game-header-screenshot.PNG "Header icon in game screen section")

#### *Player Score Area*
Just above the quiz container, as outlined to the user in the rules section, this area provides information to the user which is also used by Javascript to create a message at the end of each game. 
The features it contains are:
- **Score counter** - For each correct answer, the score number increases by one.
- **Question Number** - This shows the question number being answer in the center and goes up to 10. 
- **Incorrect counter** - Displays the number of incorrect answers. 

Each of the above own a JS function to reset the number at the end of each game. 

![Score Area in game screen section](assets/images/game-score-area-screenshot.PNG "Score Area in game screen section")

#### *Quiz Container*
Contains the question and four possible answers attached to it. 
The possible answers are displayed in four buttons which are manipulated using JavaScript. The buttons are aria-labelled for better accessibility. 
The innerHTML of the question area and each of the four buttons is used by JavaScript to display each question of each array. When hovered over, the background changes for improved user visuality.

![Quiz container in game screen section](assets/images/game-quiz-container-screenshot.PNG "Quiz container in game screen section")

If the user clicks the correct answer, a JavaScript function displays the **hue correct** body and button colors.

![Correct - body style in game screen section](assets/images/game-correct-style.PNG "Correct - body style in game screen section")

If the user clicks the incorrect answer, the same applies just displaying the **hue incorrect** color. 

![Incorrect - body style in game screen section](assets/images/game-incorrect-style.PNG "Incorrect - body style in game screen section")



### 5. **Exit Page**
Activated when the **door icon** is pressed in the top right-hand corner within the header (hides game-screen and displays rules-section).

A small box pops up to double check the player wants to leave for sure. 

The box contains two buttons:
- Yes, to go back to the main menu.

or
- No, resume game by closing rules-screen and reopening game-screen section. 

![Exit screen section](assets/images/exit-section-screenshot.PNG "Exit screen section")


### 6. **End Page**

## 3. Testing

## 4. Deployment

For deployment, GitHub was used and the data was pushed from GitPod. 

The steps needed to take to deploy this project are as follows: 

1. Visit GitHub's official website.

2. In the top right-hand corner of the menu section, click on the **small array shown**, just above the icon. 

3. Select **Your Repositaries**.

4. Select **MasterMindsIQ Challenge Project**.

5. Just above the GitPod button, click on **settings**.

6. Scroll down to roughly 80% of the page and click on **GitHub Pages**.

7. From the *source section*, select **main branch**.

8. Click **save**.

9. Update the page and once the project is deployed, the link will show in *green* and ready for use. 

![Deployment stage of project](assets/images/deployment-screenshot.PNG "Deployment stage of project")

Click here for the offical GitHub link for this project 
[MasterMind-IQ-Challenege](https://adampillis.github.io/MasterMind-IQ-Challenege/)

## 5. Credits