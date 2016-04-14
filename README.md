# moodcheck
Sinatra + elastic beanstalk test - goal is to use Alexa to get user to talk about their mood, record results in database

## Concept:

Create a system that asks user to rate their senses of physical and mental well-being on a scale of 1 to 10. Values are recording into a database and compared against previous values and trends. The system then prompts additional responses based on the results: if the user has been on a downswing for the past week, it says something like "I notice that you've been feeling steadily less physically healthy. Is there a reason why?" 

The initial goal will not be to process the non-numeric responses, but to simply stimulate introspection. 

Stretch goal is to add additional conversational handling for the 'why?' portion. 

A future feature that might be interesting to add is multiple users, all connected via VOIP accounts, and have the Alexa app actually connect users via VOIP if they decide they want to continue talking but with another human. Each user could have an availability schedule in the database, and an instance of Asterisk (free VOIP software) could be called to bridge the call, first prompting the callee to agree to accept the call before connecting users.
