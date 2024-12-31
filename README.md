# Scraping-Football-Statistics

축구 통계를 제공하는 웹사이트 whoscored.com(후스코어드닷컴)을 스크랩하는 파이썬 코드입니다.

## Data

Team Statistics(팀 통계)와 Player Statistics(선수 통계)를 각각 스크랩합니다.


### Team Statistics

> 예: [England Premier League 2023-2024](https://1xbet.whoscored.com/Regions/252/Tournaments/2/Seasons/10316/Stages/23400/TeamStatistics/England-Premier-League-2024-2025)

모든 테이블에 공통적으로 포함된 열
- Team

각 테이블에 포함된 열
- Summary
    - Team
    - Tournament
    - Goals
    - Shots pg
    - Discipline
    - Possession%
    - Pass%
    - AerialsWon
    - Rating
- Defensive
    - Team
    - Shots pg
    - Tackles pg
    - Interceptions pg
    - Fouls pg
    - Offsides pg
    - Rating
- Offensive
    - Team
    - Shots pg
    - Shots OT pg
    - Dribbles pg
    - Fouled pg
    - Rating
- xG
    - Team
    - xG
    - Goals*
    - xGDiff
    - Shots
    - xG/Shots
    - Rating

> [!NOTE]
> `Summary`, `Offensive` 테이블 포함된 `"Shots pg"`는 경기당 시도한 슈팅 수를 의미하지만,   
> `Defensive` 테이블에 포함된(동일한 이름의) 열 `"Shots pg"`은 경기당 허용한 슈팅 수를 의미합니다.


### Player Statistics

> 예: [England Premier League 2023-2024](https://1xbet.whoscored.com/Regions/252/Tournaments/2/Seasons/9618/Stages/22076/PlayerStatistics/England-Premier-League-2023-2024)

모든 테이블에 공통적으로 포함된 열
- Rank
- Player
- Team
- Age
- Position
- Apps
- Mins

각 테이블에 포함된 열
- Summary
    - Goals
    - Assists
    - Yel
    - Red
    - SpG
    - PS%
    - AerialsWon
    - MotM
- Defensive
    - Tackles
    - Inter
    - Fouls
    - Offsides
    - Clear
    - Drb
    - Blocks
    - OwnG
- Offensive
    - Goals
    - Assists
    - SpG
    - KeyP
    - Drb
    - Fouled
    - Off
    - Disp
    - UnsTch
- Passing
    - Assists
    - KeyP
    - AvgP
    - PS%
    - Crosses
    - LongB
    - ThrB
- xG
    - xG
    - Goals
    - xGDiff
    - xG/90
    - Shots
    - xG/Shots
