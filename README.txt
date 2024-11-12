# MagicalArenaTest
 README.md file that you can use for your Magical Arena Java game project. This README provides an overview of the project, instructions on how to set it up, and details on how to run the game.
 How to Use this README:
Save this as README.md in the root directory of your project.
Customize any sections if necessary (e.g., add your GitHub username or change the license type).
You can also include additional sections for unit tests, build systems, or other tools you may be using (like Maven, Gradle, etc.).

Game Components
1. Player Class
The Player class represents each participant in the battle. It has the following attributes:

Health: The player's health, which decreases when they take damage.
Strength: A defensive attribute, used to mitigate the damage received.
Attack: An offensive attribute, used to calculate the damage inflicted.
Methods in the Player class:

rollDie() - Simulates rolling a 6-sided die.
attackDamage(int roll) - Calculates attack damage based on the player's attack and the die roll.
defenseDamage(int roll) - Calculates defense damage based on the player's strength and the die roll.
takeDamage(int damage) - Reduces the player’s health by the specified damage.
2. MagicalArena Class
The MagicalArena class is responsible for the game’s main logic:

The game proceeds in rounds where the attacker and defender roll dice and calculate damage.
The player with the lower health attacks first. If both players have the same health, the attacker is chosen randomly.
The game ends when one player’s health reaches 0.
