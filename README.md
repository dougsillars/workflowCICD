# workflowCICD
CI/CD example of a conductor workflow


In this repo, we have 2 versions of a weather workflow. We are using CI/CD via a Github action to update the Conductor instance (in this case [Orkes Playground](https://play.orkes.io).)

There are 4 steps to the action

1. checkout
2. authentication: using Github secrets to store the Key/Secret, we can call the token endpoint to generate a JWT token. 
3. 4. Using the JWT token for authentication, we can send the two JSON files to conductor to update the workflows. 