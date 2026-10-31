# IAI-project
# AI Interview Telegram Chatbot

## 1. Project Overview

The **AI Interview Telegram Chatbot** is an automated mock interview chatbot developed using **n8n** and the **Telegram Bot API**.

The project helps students practise interview questions through Telegram. Users can choose between Technical and HR mock interviews and receive automated responses and feedback based on their answers.

The current implementation uses conditional logic and automated message handling in n8n.

## 2. Objectives

- To provide an easy-to-use interview practice platform.
- To help students prepare for technical and HR interviews.
- To automate interview question delivery through Telegram.
- To provide basic feedback on students' answers.
- To demonstrate workflow automation using n8n.

## 3. Technologies Used

- **n8n:** Workflow automation platform.
- **Telegram Bot API:** Communication between the chatbot and users.
- **IF Node:** Conditional checking and decision-making.
- **Telegram Trigger:** Receives incoming Telegram messages.
- **Telegram Send Message Node:** Sends interview questions and feedback.

## 4. Features

### A. Start Interview
When the user sends `/start`, the chatbot welcomes the user and displays two interview options:

1. Technical Interview
2. HR Interview

### B. Technical Mock Interview
When the user selects `TECHNICAL`, the chatbot asks:

"What is the main difference between a list and a tuple in Python?"

The chatbot checks whether the answer contains the expected keyword related to mutability and sends an appropriate response.

### C. HR Mock Interview
When the user selects `HR`, the chatbot asks:

"Tell me about yourself."

After the user submits an answer, the chatbot provides general feedback encouraging the user to explain their strengths, relevant skills, and career goals.

### D. Automated Feedback
The chatbot uses conditional logic to determine which response should be sent to the user.

## 5. Workflow Architecture

The workflow follows this sequence:

1. Telegram Trigger receives a message.
2. IF node checks whether the user entered `/start`.
3. The chatbot displays the interview options.
4. IF nodes identify the selected interview type.
5. The appropriate interview question is sent.
6. Further IF nodes check the user's response.
7. Telegram sends feedback based on the condition.

## 6. Workflow Structure

**Main n8n Nodes:**

- Telegram Trigger
- IF
- Send a Text Message 1
- IF1
- Send a Text Message 2
- IF2
- Send a Text Message 3
- IF3
- Send a Text Message 4
- Send a Text Message 5
- IF4
- Send a Text Message 6
- Send a Text Message 7

## 7. How to Use

1. Open Telegram.
2. Search for the configured Telegram bot.
3. Start a conversation using `/start`.
4. Choose `TECHNICAL` or `HR`.
5. Answer the displayed interview question.
6. Receive automated feedback from the chatbot.

## 8. Advantages

- Easy access through Telegram.
- Simple and user-friendly interaction.
- Helps students practise interview questions.
- Automates basic interview communication.
- Demonstrates practical workflow automation.

## 9. Future Enhancements

The project can be enhanced with:

- AI Agent integration for intelligent interview conversations.
- Large Language Model (LLM) integration for answer evaluation.
- More technical and HR interview questions.
- Personalized feedback and improvement suggestions.
- Interview performance tracking.
- Support for multiple programming languages.

## 10. Conclusion

The AI Interview Telegram Chatbot demonstrates how workflow automation can be used to create an interactive interview practice system.

By combining Telegram and n8n, the project provides students with a simple platform to practise technical and HR interview questions and receive automated feedback.

## 11. Author

Developed as an academic project for ISE2.

