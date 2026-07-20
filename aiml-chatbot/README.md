# 🤖 TechStore Virtual Assistant (AIML 2.0)

A multilingual, context-aware virtual assistant built with **AIML 2.0** for **Pandorabots** and other compatible AIML platforms. Designed for electronics e-commerce, the assistant delivers **24/7 automated customer support**, helping customers discover products, check prices, track orders, and receive assistance through natural conversations.

---

## 📋 Project Overview

The **TechStore Virtual Assistant** is an intelligent chatbot developed for a high-end electronics store specializing in:

- 💻 Laptops
- 📱 Smartphones
- 📟 Tablets

Instead of relying on simple keyword matching, the assistant utilizes **AIML 2.0 conversational features** to understand context, normalize user input, maintain dialogue flow, and recover gracefully from unexpected requests.

The project demonstrates how symbolic AI can be used to build structured, maintainable, and user-friendly conversational systems.

---

## ✨ Features

- 🌍 Multilingual support (English & Greek)
- 💬 Natural conversational interactions
- 🛒 Product price lookup
- 📦 Order tracking workflow
- 📞 Contact information assistance
- 🤝 Human agent handoff
- 🔄 Context-aware conversations
- ⚡ Fast symbolic pattern matching
- 🛡️ Robust fallback handling for unknown inputs

---

# 🏗️ Technical Architecture

The chatbot follows four fundamental conversational AI design principles.

## 1. Context Awareness

Implemented using the **`<that>`** tag.

The chatbot remembers its previous response, allowing it to correctly interpret short answers such as **"Yes"** or **"No"** based on the current conversation.

Example:

```
Bot: Do you have your order number?
User: Yes
```

Instead of treating *Yes* as an isolated message, the assistant understands the conversational context and continues the order tracking workflow.

---

## 2. Communicability

Implemented using:

- `<srai>`
- Wildcards (`*`, `^`)
- Input normalization

Different user expressions are redirected to the same knowledge category through **Symbolic Reduction**.

For example, all of the following inputs:

- Where are you located?
- How can I contact you?
- I need your phone number.
- Give me your contact information.

are redirected to a single internal category, making the chatbot easier to maintain while supporting more natural language.

---

## 3. Conscientiousness

Implemented through structured **feedback loops**.

After completing a request, the assistant verifies whether the user's issue has been resolved before ending the conversation.

Example:

```
Bot: The price is €999.
Bot: Did this answer your question?
```

This creates a more complete and user-focused interaction rather than abruptly ending the dialogue.

---

## 4. Damage Control

Implemented using:

- Universal Default Category (`*`)
- Human Agent Handoff

Whenever the assistant cannot understand a request, it avoids conversational dead ends by:

- Politely informing the user
- Asking for clarification
- Offering the option to connect with a human representative

This ensures a smooth user experience even when unexpected inputs occur.

---

# 📁 Project Structure

```
aiml-chatbot/
│
├── udc.aiml
├── prices.map
├── techstore.properties
├── elgreetings.set
├── engreetings.set
├── *.substitution
└── ...
```

### File Description

| File | Description |
|------|-------------|
| `udc.aiml` | Main chatbot logic, dialogue flows, categories, and AIML patterns |
| `prices.map` | Product price knowledge base separated from chatbot logic |
| `elgreetings.set` | Greek greeting recognition set |
| `engreetings.set` | English greeting recognition set |
| `techstore.properties` | Bot configuration and variables |
| `*.substitution` | Input normalization rules for user messages |

---

# 🛠️ Technologies Used

- AIML 2.0
- Pandorabots
- XML
- Symbolic AI
- Pattern Matching
- Knowledge Maps
- Sets
- Substitution Files

---

# 🚀 Deployment

To run the chatbot on **Pandorabots** (or another AIML 2.0 compatible platform):

1. Create a new bot.
2. Upload every file inside the `aiml-chatbot/` directory.
3. Import:
   - `.aiml`
   - `.map`
   - `.set`
   - `.substitution`
   - `.properties`
4. Configure the substitution files.
5. Train or publish the bot.
6. Start chatting.

---

# 🎯 Conversation Flow

```
Greeting
      │
      ▼
Main Menu
      │
      ├── Product Prices
      │
      ├── Order Tracking
      │
      ├── Contact Information
      │
      └── Human Representative
                     │
                     ▼
           Feedback Loop
                     │
          Issue Resolved?
              │        │
             Yes      No
              │        │
              ▼        ▼
           End Chat  Continue
```

---

# 💡 AIML Concepts Demonstrated

- Context Management (`<that>`)
- Symbolic Reduction (`<srai>`)
- Wildcard Pattern Matching
- Knowledge Separation using Maps
- Input Normalization
- Conversation Memory
- Feedback Loops
- Human Agent Escalation
- Universal Default Category
- Modular AIML Design

---

# 📚 Learning Objectives

This project demonstrates how AIML 2.0 can be used to create a conversational assistant capable of:

- Maintaining contextual conversations
- Handling multiple user expressions naturally
- Separating data from conversational logic
- Preventing dialogue dead ends
- Providing structured customer support workflows

It serves as an educational example of symbolic conversational AI and best practices for building maintainable AIML-based virtual assistants.

---
