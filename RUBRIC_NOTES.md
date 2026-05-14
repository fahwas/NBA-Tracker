# Rubric Notes

These notes explain where each rubric category appears in the code.

- List: `RosterService` stores players in `ArrayList<Player>`. `Player` stores stats in `List<GameStat>`.
- Map: `StatService` stores stats in `HashMap<String, List<GameStat>>`.
- Queue: `PropAlertService` stores alerts in `PriorityQueue<PropAlert>`.
- Stack: `ViewHistoryService` stores viewing history in `Stack<Player>`.
- Custom Objects: `Player`, `GameStat`, and `PropAlert` are custom objects.
- Sorting/Comparable: `Player implements Comparable<Player>`, `PropAlert implements Comparable<PropAlert>`, and `RosterService` has merge sort.
- Compilation: Run `javac -d out $(find src/main/java -name "*.java")`.
- Code Organization: Packages are separated into app, model, service, and UI layers.
- README: Included in the project root.
- Javadoc: Added to classes and major methods.
- GitHub Correctly Configured and Used: Must be completed by uploading to GitHub and making commits.
- Deliverables: Still need screenshots, GitHub link, and final submission upload.
- Write Up: Included inside the README.
- Project Implementation Completion: The project fulfills the NBA prop tracker proposal with stats, sorting, alerts, and history.
