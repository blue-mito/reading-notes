Class Reading 03
Ken Lindsay

For this week's reading, we focused on logical operations and loops. We put that knowledge into
practice with out lastest Lab Class: #3. Our final question was to be on in which we
could have multiple correct answers. For instance, guess an item on a list of items.
For this, we needed to keep track of the guess and whether it applied to any possible answers.
For this, I went back on an older list of items in the code below.
However, as soon as I pushed it, I realized there was something that could make it better!

alert('All right. Final Question: Can you guess the pokemon I had when I faced the Elite Four in Pokemon Blue? You will have 6 guesses.');

let sixPokemon = ['Charizard', 'Polywrath', 'Alakazam', 'Victrebell', 'Raichu', 'Onyx']
//let pokeGuess = prompt('Guess a pokemon:');
let pokeGuessRemain = 6
let correctPokeGuess = 0

while (pokeGuessRemain > 0) {
    let pokeGuess = prompt('Guess a pokemon:');
    let teamCheck = 0; 
    while (teamCheck < 6) {
        if (pokeGuess == sixPokemon[teamCheck]) {
            alert("You guessed right!");
            correctPokeGuess++
            teamCheck = 6;
        }
        if (teamCheck == 5) {   
            alert("Nope. They weren't on my team...");
        }
        teamCheck++
    }
    pokeGuessRemain--
    if (pokeGuessRemain === 0) {
        alert("You are out of guesses. The Team I had when I faced the Elite Four was: Charizard, Polywrath, Alakazam, Victrebell, Raichu, and Onyx." )
        alert("You had " + correctPokeGuess + " correct answers.")
    } else {
        alert("You have: " + pokeGuessRemain + " guesses remaining.")
    }

In this code, it does keep track of the number of correct guesses, but what if the user 
makes the SAME guess multiple times? I think think could be improved by logging the
guesses and cross-checking them with each submission.
All in all, a great exercise in logic and loops.
