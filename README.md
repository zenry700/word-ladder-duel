# Word Ladder Duel

A browser word-ladder puzzle: change one letter at a time to turn the start word into the target word, with every step a real word.

## Play

Open `index.html` in a browser — no build step or server required.

## How it works

- `words.js` holds curated word banks for 3, 4, and 5-letter puzzles.
- `index.html` builds a graph of words that differ by one letter, then uses BFS to generate solvable start/target pairs, verify moves, offer hints, and reveal a full solution path.
- Best scores (fewest moves, then fastest time) are saved per word length in `localStorage`.
