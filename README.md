# NBA Prop Line Tracker

## Project Summary
NBA Prop Line Tracker is a Java console application that tracks NBA players, game statistics, player averages, prop line alerts, sorting, and recently viewed players.

The project uses multiple Java collections and custom objects to meet the data structures project requirements.

## How to Run
From the project folder, compile and run with:

```bash
javac -d out $(find src/main/java -name "*.java")
java -cp out org.csu.nba.App
```

## Main Features
- View a sample NBA roster
- View individual player stats and averages
- Add new players
- Add game stats
- Sort players by name or average points
- Create prop alerts
- View prop alerts ranked by edge
- View recent player history
- Go back to a previously viewed player

## Rubric Coverage

| Category | Where It Is Shown |
|---|---|
| List | `RosterService` uses `ArrayList<Player>` for the roster. `Player` uses `List<GameStat>` for stat logs. |
| Map | `StatService` uses `HashMap<String, List<GameStat>>` to map player names to stat lists. |
| Queue | `PropAlertService` uses `PriorityQueue<PropAlert>` to rank alerts. |
| Stack | `ViewHistoryService` uses `Stack<Player>` for recently viewed players. |
| Custom Objects | `Player`, `GameStat`, and `PropAlert` are custom model classes. |
| Sorting/Comparable | `Player` and `PropAlert` implement `Comparable`. `RosterService` includes merge sort logic. |
| Compilation | Code compiles with `javac`. |
| Code Organization | Code is separated into `model`, `service`, and `ui` packages. |
| README | This file explains the project, features, and run commands. |
| Javadoc | Classes and methods include Javadoc comments. |
| GitHub Correctly Configured and Used | Add this project to a GitHub repository with commits and screenshots. |
| Deliverables | Include source code, README, screenshots, reflection, and GitHub repository link. |
| Write Up | Use the included reflection/write-up section below. |
| Project Implementation Completion | The implementation matches the proposal for an NBA prop/stat tracker. |

## Reflection / Write Up
For this project, I built an NBA Prop Line Tracker that lets a user manage players, add game stats, calculate averages, sort players, and create prop line alerts. I used different data structures to organize the project. An ArrayList stores the roster, a HashMap connects player names to stat logs, a PriorityQueue ranks prop alerts by edge, and a Stack tracks recently viewed players.

The project also includes custom objects such as Player, GameStat, and PropAlert. I used Comparable in Player and PropAlert so the program can sort players and prioritize alerts. One challenge was keeping the code organized while connecting the menu, services, and model classes. I solved this by separating the project into model, service, and UI packages.

If I had more time, I would add file saving so players and stats could remain after the program closes. I would also add input validation to prevent errors when the user enters letters instead of numbers.

## Screenshots to Include
Take screenshots of the following when submitting:
1. Program running in the terminal
2. Viewing the roster
3. Viewing player stats
4. Sorting roster
5. Prop alerts showing in priority order
6. Viewing history / go back feature
7. GitHub repository page
8. Git commit history

## GitHub Submission Checklist
- [ ] Create a GitHub repository
- [ ] Upload the full project folder
- [ ] Commit files with meaningful commit messages
- [ ] Add screenshots to the repository or submission
- [ ] Submit the GitHub repository link
- [ ] Submit the reflection/write-up
