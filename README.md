# resume_ai_agent
includes the AI agent I created with n8n for the Kura Labs Rise Up Program 
Overview
AI Agent Flow diagram

To find images go to this URL: [
](https://docs.google.com/document/d/1WZPOWsWtpCD3xXIDUxBrkf9IkjIffuUB1weo0j6JIog/edit?usp=sharing)
PROD form:

On form submission:

HTTP node:

AI Agent Node:

Email Node:

Email Output:


Building the Agent
What approach did you take to design your agent?
I started with creating a diagram in draw.io, from there I referred that and the assignment we created in class to begin. 
Once I got to the AI agent step I utilized chatgpt to help me create the prompt. 
What challenges did you face in parsing, formatting, or integrating?
Determining how to grab the position posting URL. Needed to note not to use a URL that requires any credentials. 
With parsing, I wasn’t sure what would be the best format to do so. I started with using the parsing output, but wasn’t using it correctly so I turned to ChatGPT which actually took me on a more complex path attempting to use a code node to parse the data with JavaScript; however, I ultimately couldn’t get it to work. 
How did you ensure that the AI returned JSON reliably?
Ultimately I was unable to use the output parser correctly, and realized similar to what we did in the activity it had to be executed first to then be able to grab JSON fields from the AI agent output. However, I noticed it wasn’t necessary, I ran it multiple times and it formatted as expected and provided the correct data without grabbing the fields into the parser. I did pull them into the sent email. 
Troubleshooting
What issues did you encounter and how did you resolve them?
I believe this was explained in the challenges. But it took me a while to figure out how to properly parse the data, attempting multiple nodes and coding types (JSON, Javascript, HTML). Ultimately it worked wit the Output parser, using JSON and a combination of HTML and JSON in the sent email. 
Optimization
What might you improve or add in future iterations?
I went back and included name on the form so I could pull that into the email for personalization
I also included additional HTML in the email message to help with leading
As a next step I would look to continue to tweak the prompt. There are still some items that are not coming through like I want after providing an ATS score to explain why that score was given. 
Another future state would be the AI agent fully reformatting the resume for the user, or outputting a resume that implemented the recommendations. 
