# 🎯 Number Guessing Game (CLI)

A fun and interactive Command Line Number Guessing Game built using Python.  
The program generates a random number, and the player keeps guessing until the correct number is found.

---

## 📌 Features

✔ Random number generation  
✔ Unlimited guessing attempts  
✔ Hint system (Too High / Too Low)  
✔ Attempt counter  
✔ Invalid input handling  

---

## 🚀 Technologies Used

- Python 3
- Random Module

---

## 📂 Project Structure

```bash
number-guessing-game/
│
├── guessing_game.py
└── README.md
```

---

## ▶ How to Run the Project

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/number-guessing-game.git
```

### 2️⃣ Navigate to the Project Folder

```bash
cd number-guessing-game
```

### 3️⃣ Run the Program

```bash
python guessing_game.py
```

---

## 💻 Program Code

```python
import random

# Generate random number between 1 and 100
secret_number = random.randint(1, 100)

attempts = 0

print("Welcome to the Number Guessing Game!")
print("Guess a number between 1 and 100")

while True:
    try:
        # Take user input
        guess = int(input("Enter your guess: "))
        attempts += 1

        # Check guess
        if guess > secret_number:
            print("Too high!")

        elif guess < secret_number:
            print("Too low!")

        else:
            print("Congratulations! You guessed correctly.")
            print("Total attempts:", attempts)
            break

    except ValueError:
        print("Invalid input! Please enter a number.")
```

---

## 📸 Example Output

```bash
Welcome to the Number Guessing Game!
Guess a number between 1 and 100

Enter your guess: 70
Too high!

Enter your guess: 30
Too low!

Enter your guess: 50
Congratulations! You guessed correctly.
Total attempts: 3
```

---

## ⚠ Error Handling

The program handles:
- Invalid numeric inputs
- Unexpected user entries

Example:

```bash
Invalid input! Please enter a number.
```

---

## 📚 Concepts Used

- Variables
- Loops
- Conditional Statements
- Exception Handling
- Random Number Generation
- User Input Handling

---

## 🔮 Future Improvements

- Add limited attempts
- Add difficulty levels
- Add score system
- Multiplayer mode
- GUI version using Tkinter
- Sound effects

---

## 🤝 Contributing

Contributions are welcome.  
Feel free to fork this repository and improve the project.

---

## 📜 License

This project is open-source and available under the MIT License.

---

