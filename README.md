# Quiz-game
def quiz_game():
    questions = {
        "What is the capital of France?": "Paris",
        "What is the largest planet in our solar system?": "Jupiter",
        "How many continents are there?": "7",
        "What is the chemical symbol for water?": "H2O",
        "What is the speed of light in vacuum?": "299792458 m/s",
    }
    score = 0
    for question, answer in questions.items():
        user_answer = input(f"{question} ")
        if user_answer.lower() == answer.lower():
            print("Correct!")
            score += 1
        else:
            print(f"Incorrect. The correct answer is {answer}.")
    print(f"You scored {score} out of {len(questions)}.")

if __name__ == "__main__":
    quiz_game()
