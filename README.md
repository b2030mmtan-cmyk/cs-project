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

- This program, **_Decked Out!_**, will help students and other learners in studying topics of their choosing by serving as an online application which can help store their flashcards and flashcard decks that they use in reviewing. Along with this, the users will be able to test themselves using these cards. The components (classes and their attributed and methods) are the following:
  
- **User Class**
  - (atr): _username_ - What the system will call the user, string input.
  - (atr): _decks_ - List of all decks a user has.
  - (method): _addDeck()_ - Appends a deck to the list.
  - (method): _displayDecks()_ - Displays all the decks of a user in a formatted form using #. DeckName, where the number is index + 1 to avoid starting with zero.
  - (method): _deleteDeck()_ - Pops the index (number - 1) of a user's chosen deck.
  - (method): _combineDeck()_ - Combines the questions of two decks into one deck.
- **Deck Class**
  - (atr): _title_ - What the system will call the collection of cards, string input
  - (atr): _cards_ - List of all cards a deck has.
  - (method): _addCard()_ - Appends a card to the deck.
  - (method): _deleteCard()_ - Pops the index (number - 1) of a user's chosen card.
  - (method): _displayCards()_ - Displays all the cards of a deck in a formatted form using #. CardName, where the number is index + 1 to avoid starting with zero.
- **Card Class**
  - (atr): _question_ - What the system will call the card (card title), string input; 
  - (atr): _answer_ - Accepted value, inherited from Card Class
  - (method): _displayQuestion()_ - Displays the question content and prompting the user to answer
  - (method): _checkAnswer()_ - Compares input to accepted value (answer) and returns a remark on the result
- **MulCho Card Class**
  - (atr): _question_ - Card title, inherited from Card Class
  - (atr): _answer_ - Accepted value, inherited from Card Class
  - (atr): _options_ - List of all values the user must choose from.
  - (method): _displayQuestion()_ - Displays the question content and prompting the user to answer, inherited from Card Class
  - (method): _checkAnswer()_ - Compares input to accepted value (answer) and returns a remark on the result, inherited from Card Class
  - (method): _displayOptions()_ - Displays all choices the user can choose from
  - (method): _shuffleOptions()_ - Scrambles the order in which choices are displayed
- **True or False Class**
  - (atr): _question_ - Card title, inherited from Card Class
  - (atr): _answer_ - Accepted value, inherited from Card Class
  - (method): _displayQuestion()_ - Displays the question content and prompting the user to answer, inherited from Card Class
  - (method): _checkAnswer()_ - Compares input to accepted value (answer) and returns a remark on the result, inherited from Card Class
- **Identification Class**
  - (atr): _question_ - Card title, inherited from Card Class
  - (atr): _answer_ - Accepted value, inherited from Card Class
  - (method): _displayQuestion()_ - Displays the question content and prompting the user to answer, inherited from Card Class
  - (method): _checkAnswer()_ - Compares input to accepted value (answer) and returns a remark on the result, inherited from Card Class
    
- **Class Diagram**
<img width="1245" height="864" alt="image" src="https://github.com/user-attachments/assets/1013fec8-8532-400b-b129-8dce636f6496" />


### Goals:

To develop an intuitive study companion and application that encourages learners organize and create custom flashcards, test their knowledge, and of course, improve long-term retention across any subject.

- Objective 1: Build a user management system that allows learners to create, view, delete, and combine flashcard decks.
- Objective 2: Implement deck management tools for adding, viewing, and removing individual cards in a collection.
- Objective 3: Design a versatile card system supporting various question formats.
- Objective 4: Develop an interactive quiz feature that checks user answers and provides immediate feedback to support active recall.

[Click here for Rubrics and Sample projects](https://docs.google.com/document/d/1xKd1CqK6DcNWS2_oJPBNtY5n3I3Hqiw8FY3W295Iqfk/edit?usp=sharing)
