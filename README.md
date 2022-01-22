# Dialogflow basics
Lists out the basics of dialogflow

### Requirements
* Dialogflow login account

### Resources
* Uesflow youtube tutorial from youtube - https://youtu.be/O00K10xP5MU

### Setup
- Setting up a virtual assistant using dialogflow is very easy
- Click the '+' button against intents on the left pane
  - One can start with the training phrases section
  - In this type in all the various ways in which a user could ask a particular question
  - For example: if we are trying to create an automatic response for a user's query like - "How are you"; we are trying to make dialogflow understand the various ways in which various users could ask the same question with the same 'intend'
  - The various phrases could be "How are you" or "How's life" or "What's up" etc:-
- Next section to fill could be the Responses section
  - In this we train the model of the various ways it could respond to the question (Intend) being raised
- Save the intend and hurray you have created your first intend
- Now you can try out your intent by using some of the variation of the question intended/trained to the model by typing on the top right
- You will get mostly any of the responses that you had trained the model earlier
- If there is no response, put in more training phrases to make the model better understand the several various way in which the user can raise the question that it intends to ask

### Entity
- Entity are like variables which can assume different values while the user raises a query (intend)
- For example an entity could be pincode, country-name etc:-
- Many entities are available already in dialogflow itself
- Custom entities could be made by going to entities and then click create entity
  - Enter the synonyms or usual style in which the same is entered

### Using entities to capture parameters
- While creating the intent, go to action and parameters and create the requisite parameters; parameter's entity should be mentioned along with '$'name to recall the value
- You may tick whether the particular parameter is required or not
- Double click the word on the training phrases and select the parameter to which it has to be assigned
- In the response phrases, you can recall the value of the particular parameter using $'parametername' as described in the action and parameters part. Example:
  - If one of the training phrase is - Give me the country name for ISD code starting with '001'
  - The 001 can be double clicked to consider it as the input value for pincode parameter
  - While returning the response of the country name, the same could be recalled as well 
  - To the same the response code could be - The country name for code $pincode is X


