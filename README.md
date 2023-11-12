DONE  createSchedule(): Spielplan[Spieltag1-n] // Spieltag:[{"homeClub":club.initials, "awayClub": ...}, {match2-n}]
  
matchCalc(): club.str + randomVal -> {matchResult}

matchDayCalc(): 
  call matchCalc() with all match{}, save results{}/direkt to match{}, 
  push to matchResultArr[]

matchDay():
  matchResultArr[] -> update club{}s

DONE  seasonTable(): returns sorted clubs

closeSeason(): 
  chronik table: add (push) season table
  (...calc SaisonEnd-Werte...)
  club{}: update/reset values

createSeason()
  ? assign club{} zu League (evl. league = league_nextYear, league_nextYear = 0)
  ? update League Spielplan (Abst1 === Aufst1, Abst2 === Aufst2)



Tabellen Pro Liga:
- Saison Tabelle [{Club1}, {...}] .sort()
- Chronik Tabelle [{"season": 2023, [Saison Tabelle]}]
- Ewige Tabelle [{Club1}... alle Clubs]


Collections:
clubs_initial
clubs <-lfd, Saison Tabelle zieht + sorted in []
chronik_tabelle1 + 2 <- update pusht sorted clubs []
ewige_tabelle1 + 2 <- update ändert club, goals/points für akt. league