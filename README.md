# Football World Cup Scoreboard

A React app simulating a **Live Football World Cup Scoreboard**⚽ that shows matches and scores.

**Notes:** The current implementation uses manually set timers and time intervals for simulating the playing of the games. Here
is a brief explanation of the intended logic:
 1. When the app loads initially a 3...2...1 timer is started to visualize the start of the games
 2. Then another time interval is being triggered so that we can have randomly starting and finishing games (they are being finalized when the playing time expires)
 3. A third time interval is being used for updating, randomly, the scores per game and per team
 4. After the playing time ends (currently hard coded to be 90 seconds) and all the games finish, the updates are canceled, i.e. the time intervals are cleared

_A GitHub Actions CI is setup to run build and tests on each commit in the main branch._

## Tech stack 💾
- React (with Vite)
- Vitest / React Testing Library
- CSS Modules (SASS)

### Screenshots 📸

![Animated](https://github.com/Aklilu-Mandefro/football-scoreboard-app-using-react-vite-and-vitest/blob/main/screenshots/animated.gif)
![Starting games](https://github.com/Aklilu-Mandefro/football-scoreboard-app-using-react-vite-and-vitest/blob/main/screenshots/starting-games.png)
![Running games](https://github.com/Aklilu-Mandefro/scoreboard/blob/main/screenshots/running-games.png)
![Finalizing games](https://github.com/Aklilu-Mandefro/football-scoreboard-app-using-react-vite-and-vitest/blob/main/screenshots/finalizing-games.png)
![Desktop View](https://github.com/Aklilu-Mandefro/football-scoreboard-app-using-react-vite-and-vitest/blob/main/screenshots/desktop-view.png)
![iPad View](https://github.com/Aklilu-Mandefro/football-scoreboard-app-using-react-vite-and-vitest/blob/main/screenshots/ipad-view.png)


## Application features: ⚙️
**Live Football World Cup Scoreboard** that shows matches and scores.

The board supports the following operations:

1. Start a game. When a game starts, it should capture (being initial score 0 – 0):
    a. Home team
    b. Away team

2. Finish game. It will remove a match from the scoreboard.

3. Update score. Receiving the pair score; home team score and away team score updates a game score.

4. Get a summary of games by total score. Those games with the same total score will be returned ordered by the most recently added to our system.

✍️ As an example, being the current data in the system:

    a. Mexico - Canada: 0 - 5
    b. Spain - Brazil: 10 – 2
    c. Germany - France: 2 – 2
    d. Uruguay - Italy: 6 – 6
    e. Argentina - Australia: 3 - 1

The summary would provide with the following information:

    1. Uruguay 6 - Italy 6
    2. Spain 10 - Brazil 2
    3. Mexico 0 - Canada 5
    4. Argentina 3 - Australia 1
    5. Germany 2 - France 2

  ### Possible Improvements 🚀
    - Add a clock under the game status, say counting down the seconds, to make it look more like a real-time app
    - Add some animation to when updating the scores to make it easier for the user to spot the change
    - Add some interactivity in general:
        - Clicking on each game leading to a details pane with the match details
        - Option for selecting favourite team
    - Add another page/tab where the history summary of the past games can be read



### Running The App locally

To run the app, follow these steps.

1. Ensure that [NodeJS](http://nodejs.org/) is installed.
2. Install [yarn](https://classic.yarnpkg.com/en/docs/install).
3. From the project folder, execute the following commands:

To install dependencies:
```shell
  yarn install
```
To run the client app:

```shell
  yarn dev
```
To run the tests:

```shell
  yarn test
```
## ✍️ Please give this repo a ⭐ if you found it helpful.
