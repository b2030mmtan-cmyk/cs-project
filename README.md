# CS3SY26_ProjectProposal by ErDelValle, ShRenacido, MiTan

## Project Proposal Template

### Decked Out!: Flashcard Study Buddy
### Section			   	      :   9 - Magnesium
### Group Members			    :   DEL VALLE, RENACIDO, TAN
### Date (Proposal Date)  :   13 November 2026 

### Project Description:

- A brief summary of the project description and the need for it.
- Describes system components, features, and expected outputs clearly and logically. NOTE: Clearly described the elements(classes), their attributes and methods and how they will interact with each other.
- Include the description as well of your target demographics as the user of your application. 
- The description is then followed by the class diagram, depicting clearly what was described.

- **_Decked Out!_** is a flashcard application with the purpose of helping students study and review more effectively by letting them digitally create and store flashcards, and use this to test their knowledge on those topics. The target users for this application are students and learners who use flashcards to study and prepare for exams, quizzes, and other assessments. Their needs that we aim to address is that of being able to easily organize and keep the flashcards they used for studying digitally. The problem this aims to solve is the unreliability of physical flashcards, as these can be easily torn, soaked, lost, or damaged. When this happens, a student's learning is disrupted and their hard work in making said flashcards are put to waste. The components of the program (classes, attributes, methods), the class diagram, and the interactions are the following:
  
- **User Class**
  - (atr): _username_ - What the system will call the user, string input.
  - (atr): _decks_ - List of all decks a user has, starts as an empty list.
  - (method): _addDeck()_ - Appends a deck to the list.
  - (method): _displayDecks()_ - Displays all the decks of a user in a formatted form using N. DeckTitle, where the number (N) is index + 1 to avoid starting with zero.
  - (method): _deleteDeck()_ - Pops the index (N input - 1) of a user's chosen deck.
  - (method): _combineDeck()_ - Combines the questions of two decks into one deck.
- **Deck Class**
  - (atr): _title_ - Title of the deck, string input.
  - (atr): _cards_ - List of all cards a deck has, starts as an empty list.
  - (method): _addCard()_ - Appends a card to the deck.
  - (method): _deleteCard()_ - Pops the index (N - 1) of a user's chosen card.
  - (method): _displayCards()_ - Displays all the cards of a deck in a formatted form using N. CardQuestion, where the number (N) is index + 1 to avoid starting with zero.
- **Card Class**
  - _abstract class which serves as the blueprint for the type-specific card classes_
  - (atr): _question_ - Question of the card that the system will prompt, string input.
  - (atr): _answer_ - The correct answer of the question, string input.
  - (method): _displayQuestion()_ - Prints the question content and prompts the user to input their answer.
  - (method): _checkAnswer()_ - Compares answer input and the correct answer, and returns a remark based on the result (If correct, "Correct Answer!", if not, "Incorrect Answer!, the correct answer is" _answer_., 
- **MulCho Card Class**
  - (atr): _question_ - Card question, inherited from Card Class
  - (atr): _answer_ - Correct answer, inherited from Card Class
  - (atr): _options_ - List of all values the user must choose from.
  - (method): _displayQuestion()_ - Displays the question content and prompting the user to answer, inherited from Card Class.
  - (method): _checkAnswer()_ - Compares input to accepted value (answer) and returns a remark on the result, inherited from Card Class.
  - (method): _displayOptions()_ - Displays all choices the user can choose from.
  - (method): _shuffleOptions()_ - Shuffles the list and the order in which choices are displayed.
- **True or False Card Class**
  - (atr): _question_ - Card question, inherited from Card Class
  - (atr): _answer_ - Correct answer, inherited from Card Class
  - (method): _displayQuestion()_ - Displays the question content and prompting the user to answer, inherited from Card Class. Additionally, it prompts (True/False), if the user answers neither, the system will prompt the user to input another answer.
  - (method): _checkAnswer()_ - Compares input to accepted value (answer) and returns a remark on the result, inherited from Card Class.
- **Identification Card Class**
  - (atr): _question_ - Card question, inherited from Card Class
  - (atr): _answer_ - Correct answer, inherited from Card Class
  - (method): _displayQuestion()_ - Displays the question content and prompting the user to answer, inherited from Card Class.
  - (method): _checkAnswer()_ - Compares input to accepted value (answer) and returns a remark on the result, inherited from Card Class. 
- **Class Diagram**
<img width="1245" height="864" alt="image" src="https://github.com/user-attachments/assets/1013fec8-8532-400b-b129-8dce636f6496" />
- **Interactions**
  - User-Deck and Deck-Card has a one-to-many composition relationship.
  - Card is the parent abstract class which MulCho Card, True or False Card, and Identification Card inherits.

### Goals:

To develop an intuitive study companion and application that encourages learners organize and create custom flashcards, test their knowledge, and of course, improve long-term retention across any subject.

- Objective 1: Build a user management system that allows learners to create, view, delete, and combine flashcard decks.
- Objective 2: Implement deck management tools for adding, viewing, and removing individual cards in a collection.
- Objective 3: Design a versatile card system supporting various question formats.
- Objective 4: Develop an interactive quiz feature that checks user answers and provides immediate feedback to support active recall.

[Click here for Rubrics and Sample projects](https://docs.google.com/document/d/1xKd1CqK6DcNWS2_oJPBNtY5n3I3Hqiw8FY3W295Iqfk/edit?usp=sharing)
