# quiz-game
# 20-question quiz game in Python

questions = [
    {
        "question": "1. What is the capital of India?",
        "options": ["A. Mumbai", "B. Delhi", "C. Kolkata", "D. Chennai"],
        "answer": "B"
    },
    {
        "question": "2. Who discovered gravity?",
        "options": ["A. Newton", "B. Einstein", "C. Galileo", "D. Tesla"],
        "answer": "A"
    },
    {
        "question": "3. What is the chemical symbol for water?",
        "options": ["A. CO2", "B. H2O", "C. NaCl", "D. O2"],
        "answer": "B"
    },
    {
        "question": "4. Which planet is known as the Red Planet?",
        "options": ["A. Earth", "B. Mars", "C. Venus", "D. Jupiter"],
        "answer": "B"
    },
    {
        "question": "5. Who is known as the Father of Computers?",
        "options": ["A. Alan Turing", "B. Charles Babbage", "C. Bill Gates", "D. Steve Jobs"],
        "answer": "B"
    },
    {
        "question": "6. What gas do plants absorb from the atmosphere?",
        "options": ["A. Oxygen", "B. Hydrogen", "C. Carbon Dioxide", "D. Nitrogen"],
        "answer": "C"
    },
    {
        "question": "7. Which organ purifies blood in humans?",
        "options": ["A. Liver", "B. Kidney", "C. Lungs", "D. Heart"],
        "answer": "B"
    },
    {
        "question": "8. What is the square root of 64?",
        "options": ["A. 6", "B. 7", "C. 8", "D. 9"],
        "answer": "C"
    },
    {
        "question": "9. What is the currency of Japan?",
        "options": ["A. Won", "B. Yen", "C. Dollar", "D. Ringgit"],
        "answer": "B"
    },
    {
        "question": "10. Who wrote the Harry Potter series?",
        "options": ["A. Tolkien", "B. J.K. Rowling", "C. Shakespeare", "D. C.S. Lewis"],
        "answer": "B"
    },
    {
        "question": "11. How many continents are there?",
        "options": ["A. 5", "B. 6", "C. 7", "D. 8"],
        "answer": "C"
    },
    {
        "question": "12. What is the largest ocean?",
        "options": ["A. Atlantic", "B. Indian", "C. Pacific", "D. Arctic"],
        "answer": "C"
    },
    {
        "question": "13. What is 15 x 3?",
        "options": ["A. 30", "B. 45", "C. 60", "D. 50"],
        "answer": "B"
    },
    {
        "question": "14. Which bird is known for its mimicry?",
        "options": ["A. Parrot", "B. Sparrow", "C. Eagle", "D. Owl"],
        "answer": "A"
    },
    {
        "question": "15. What does CPU stand for?",
        "options": ["A. Central Processing Unit", "B. Computer Program Unit", "C. Control Panel Utility", "D. Central Print Unit"],
        "answer": "A"
    },
    {
        "question": "16. Which vitamin is produced when skin is exposed to sunlight?",
        "options": ["A. Vitamin A", "B. Vitamin B", "C. Vitamin C", "D. Vitamin D"],
        "answer": "D"
    },
    {
        "question": "17. What is the national animal of India?",
        "options": ["A. Lion", "B. Tiger", "C. Elephant", "D. Deer"],
        "answer": "B"
    },
    {
        "question": "18. What does WWW stand for?",
        "options": ["A. Web World Wide", "B. World Web Wide", "C. World Wide Web", "D. Wide World Web"],
        "answer": "C"
    },
    {
        "question": "19. What planet is closest to the Sun?",
        "options": ["A. Earth", "B. Mercury", "C. Mars", "D. Venus"],
        "answer": "B"
    },
    {
        "question": "20. What is the hardest substance in the human body?",
        "options": ["A. Bone", "B. Enamel", "C. Cartilage", "D. Skin"],
        "answer": "B"
    }
]

# Start quiz
print("🎮 Welcome to the 20-Question Quiz Game!")
score = 0

for q in questions:
    print(f"\n{q['question']}")
    for option in q["options"]:
        print(option)
    user_answer = input("Enter your answer (A/B/C/D): ").strip().upper()
    if user_answer == q["answer"]:
        print("✅ Correct!")
        score += 1
    else:
        print(f"❌ Wrong! The correct answer is {q['answer']}")

print("\n🏁 Quiz Finished!")
print(f"Your total score is: {score}/20")

if score == 20:
    print("🏆 Perfect! You're a genius!")
elif score >= 15:
    print("👏 Great job!")
elif score >= 10:
    print("👍 Good effort!")
else:
    print("💡 Keep practicing and try again!")
