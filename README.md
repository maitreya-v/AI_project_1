# AI Project 1: Pac-Man

CSE 537, Fall 2026.

## Project files

- [search.zip](search.zip): all seven solutions, original supporting files, documentation, and reproducible validation scripts.
- [Project01_Report.pdf](Project01_Report.pdf): measured results, heuristic proofs, and critical analysis.
- [Project01_PacMan_Presentation.pptx](Project01_PacMan_Presentation.pptx): 12-slide presentation with editable charts and speaker notes.

## Run

Download and extract `search.zip`. Use Python 3.11 and run commands in the extracted directory.

```sh
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
python pacman.py -l mediumCorners -p AStarCornersAgent
python pacman.py -l trickySearch -p AStarFoodSearchAgent
```

Append `-q` to run without graphics. See the README inside the archive for more instructions.

## Validation

The final archive passed 13 regression tests and 20 complete-game examples. A* expanded 741 states on `mediumCorners` and 255 on `trickySearch`, below the stated stretch and extra-credit thresholds. The official course autograder was not supplied. The optional 108-food `mediumSearch` challenge did not finish within the five-second diagnostic.

## Attribution

The framework comes from UC Berkeley, with original notices retained: http://ai.berkeley.edu. Requirements come from the supplied CSE 537 Project01 assignment. Implementation, validation, report, and presentation preparation used OpenAI Codex assistance.
