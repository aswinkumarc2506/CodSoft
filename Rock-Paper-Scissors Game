import tkinter as tk
from tkinter import messagebox
import random

# Function to determine the winner
def determine_winner(player_choice, computer_choice):
    if player_choice == computer_choice:
        return "It's a tie!"
    elif (player_choice == 'Rock' and computer_choice == 'Scissors') or \
         (player_choice == 'Paper' and computer_choice == 'Rock') or \
         (player_choice == 'Scissors' and computer_choice == 'Paper'):
        return "You win!"
    else:
        return "Computer wins!"

# Function to handle player's choice
def play(player_choice):
    choices = ['Rock', 'Paper', 'Scissors']
    computer_choice = random.choice(choices)
    
    result = determine_winner(player_choice, computer_choice)
    messagebox.showinfo("Result", f"Player: {player_choice}\nComputer: {computer_choice}\n\n{result}")

# Create tkinter window
window = tk.Tk()
window.title("Rock-Paper-Scissors Game")

# Colors
rock_color = "#FF5733"   # Orange
paper_color = "#33FF7E"  # Green
scissors_color = "#338CFF"  # Blue

# Create widgets with colors
label = tk.Label(window, text="Select your choice:", font=("Arial", 14))
label.pack(pady=10)

rock_button = tk.Button(window, text="Rock", width=10, height=2, font=("Arial", 12), bg=rock_color, fg="white", command=lambda: play('Rock'))
rock_button.pack(pady=5)

paper_button = tk.Button(window, text="Paper", width=10, height=2, font=("Arial", 12), bg=paper_color, fg="white", command=lambda: play('Paper'))
paper_button.pack(pady=5)

scissors_button = tk.Button(window, text="Scissors", width=10, height=2, font=("Arial", 12), bg=scissors_color, fg="white", command=lambda: play('Scissors'))
scissors_button.pack(pady=5)

# Start the tkinter main loop
window.mainloop()
