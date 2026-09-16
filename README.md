# AI Project 1: Pac-Man

CSE 537, Fall 2026.

Maitreya Vaghulade (117437999) and Karan Jain (117420953).

## Project files

- [search.zip](search.zip): all seven solutions, original supporting files, documentation, reproducible validation scripts, and Mac demo launchers.
- [Project01_Report.pdf](Project01_Report.pdf): revised submission report with both team members, measured results, heuristic proofs, and critical analysis.
- [Project01_PacMan_Presentation.pptx](Project01_PacMan_Presentation.pptx): 12-slide presentation with editable charts and speaker notes.

## Run

Download and extract `search.zip`. Use Python 3.11 and run commands in the extracted directory.

```sh
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
python pacman.py -l mediumCorners -p AStarCornersAgent
python pacman.py -l trickySearch -p AStarFoodSearchAgent
```

Append `-q` to run without graphics. See the README inside the archive for more instructions.

### Mac presentation demos

After extracting the ZIP, double-click `Run_Pacman.command` for food search, or `Demo_Pacman.command` for a choice of demonstrations. The launchers require Python 3.11 with Tkinter. Normal demo playback uses a 0.04-second delay per move.

From the extracted folder, you can also run:

```sh
./Demo_Pacman.command bfs
./Demo_Pacman.command corners
./Demo_Pacman.command food
```

Use `./Demo_Pacman.command step` to advance one move at a time, or `./Demo_Pacman.command fast` to remove animation delays. In step mode, any key advances one move and `q` resumes playback.

## Validation

The final archive passed 13 regression tests and 20 complete-game examples. A* expanded 741 states on `mediumCorners` and 255 on `trickySearch`, below the stated stretch and extra-credit thresholds. The official course autograder was not supplied. The optional 108-food `mediumSearch` challenge did not finish within the five-second diagnostic.

## Attribution

The framework comes from UC Berkeley, with original notices retained: http://ai.berkeley.edu. Requirements come from the supplied CSE 537 Project01 assignment. Implementation, validation, report, and presentation preparation used OpenAI Codex assistance.
