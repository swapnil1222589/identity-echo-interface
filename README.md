# 📡 The Identity Echo Interface

> A simple interactive Streamlit application that captures a user's identity and message, validates the input, and displays useful message statistics.

**Built for the MirAI School of Technology Virtual Summer Internship 2026.**

## ✨ Overview

The **Identity Echo Interface** is a beginner-friendly Streamlit web application designed to demonstrate core concepts of interactive Python web apps.

Users can enter their name and a message, then press **Transmit** to receive a personalized confirmation along with basic message and token statistics.

The project focuses on:

* Interactive user input
* Input validation
* Conditional UI feedback
* Basic string processing
* Streamlit layout and metrics
* Estimating token usage from message length

## 🎯 Features

### 👤 Identity Input

Enter your name through an interactive text field.

### 💬 Message Input

Enter a message that you want to transmit through the interface.

### 📡 Transmission Validation

The application checks whether both the name and message have been provided before processing the request.

### ✅ Success Feedback

After a valid submission, the application displays a personalized transmission confirmation.

### 📊 Message Statistics

The interface calculates and displays:

* Total character count
* Estimated token count

### 🧮 Token Estimation

The current implementation uses a simple approximation:

```text
Estimated Tokens ≈ Number of Characters ÷ 4
```

This is only a rough estimate and should not be treated as an exact tokenizer result.

## 🖥️ Application Flow

```text
User enters Name
       ↓
User enters Message
       ↓
     Transmit
       ↓
Input Validation
   ↙         ↘
Invalid       Valid
  ↓             ↓
Error/Warning  Success Message
                  ↓
            Message Statistics
                  ↓
        Characters + Estimated Tokens
```

## 🛠️ Tech Stack

| Technology   | Purpose                            |
| ------------ | ---------------------------------- |
| Python       | Application logic                  |
| Streamlit    | Interactive web interface          |
| Git / GitHub | Version control and source hosting |

## 📂 Project Structure

```text
identity-echo-interface/
├── app.py
├── requirements.txt
├── README.md
├── LICENSE
└── .gitignore
```

### File Description

**app.py**
Contains the complete Streamlit application, including UI components, validation, transmission logic, and message statistics.

**requirements.txt**
Contains the Streamlit dependency required to run the application.

**README.md**
Project documentation and setup instructions.

**LICENSE**
MIT License for the project.

## 🚀 Getting Started

### Prerequisites

Make sure you have:

* Python 3.9+
* pip
* Git

### 1. Clone the Repository

```bash
git clone https://github.com/swapnil1222589/identity-echo-interface.git
cd identity-echo-interface
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the Application

```bash
streamlit run app.py
```

Streamlit will provide a local URL in your terminal, typically:

```text
http://localhost:8501
```

Open that URL in your browser.

## 🧪 Example

Enter:

**Name**

```text
Swapnil
```

**Message**

```text
Hello from the Identity Echo Interface!
```

The application will return a personalized transmission message and show the message's character count and estimated token count.

## 📊 Example Output

For a message containing 40 characters:

```text
Characters: 40
Estimated Tokens: 10.00
```

The estimate is calculated using:

```text
40 ÷ 4 = 10 tokens
```

## 🎓 Internship Context

This project was created as part of the **MirAI School of Technology Virtual Summer Internship 2026**, as an implementation of the **Identity Echo Interface** assignment.

The project demonstrates practical use of Python and Streamlit to create an interactive browser-based application.

## 🔮 Future Improvements

Possible improvements include:

* Real tokenizer-based token counting
* Message history
* Character and word counters
* Session state support
* Custom UI styling
* Dark/light theme controls
* Export submitted messages
* Timestamped transmissions
* Persistent database storage
* Deployment with Streamlit Community Cloud

## 🌐 Deployment

This application can be deployed using Streamlit-compatible hosting platforms.

Typical workflow:

```text
GitHub Repository
       ↓
Connect Repository
       ↓
Configure Python Environment
       ↓
Install requirements.txt
       ↓
Run app.py
```

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Commit your changes.
5. Open a pull request.

