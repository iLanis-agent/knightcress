# Knightcress 1.0 TEST
Native Android anti-knight Latin puzzle. Android8+ min26/target35. Package com.gg007.knightcress.

## Rules
Known anti-knight Latin-square adaptation on a 4x4 grid. Place 1-4 once in every row and column. Equal digits cannot be a chess-knight move apart: two cells along one axis and one along the other. There is no 2x2 box rule; diagonal repeats may be legal. Four gold givens stay fixed. Tap an editable tile through blank, 1, 2, 3, 4, blank. Twelve independently generated, uniquely solved clue layouts and twelve distinct completed boards. Each has 3-5 ordinary Latin completions, so the knight rule is needed. Undo/reset, levels and saved palette/knight-reach marks. Reach marks show all destinations from the last editable tile tapped.

## Download and status
https://mega.co.nz/#!0Q1QSDQK!V_Es3ghmSm5EMEhXYeE459p1-N6TKpQhypmacekeaeA
APK 16878 bytes; SHA256 151ffb918b2e8dfde4294078914108cfd266f90441e2951c975fb47fcc673f70. Original certificate SHA2561651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597; no requested permissions; original GG007 icon unchanged. Anonymous downloaded bytes match.

## Checks
Seed-841110 generator enumerates 576 Latin grids, 96 anti-knight grids and 72 anti-knight grids that break Sudoku boxes. Every chosen completed board is one of those 72. Independent pair-distance oracle agrees with production row/column and eight-offset checks on all 331,776 row-permutation grids for all twelve levels (3,981,312 comparisons), plus 120,000 random/invalid arrays and levels. Each puzzle has exactly one answer. Fixed locks, bounds, undo/replay/reset and solved lock pass. Actual drawing-adapter cell-center digit taps solve all twelve and check levels, next, menus, privacy, saved palette/reach marks and completion. Seven drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
All 215 prior studio descriptions and 803 legacy entries reviewed. Orderfern uses inequality arrows, Copperdot adjacent difference/double dots and Violetpath consecutive path sets. Nightstride is knight travel over cells, not digit placement. Knightcress instead applies a nonlocal knight-conflict graph to Latin digits. No matching existing mechanic found. Known anti-knight Latin-square adaptation, not a globally new interaction. Original generated clue layouts, code and visuals; no copied source grids. Six fully read sources include a mathematician explaining anti-knight Latin squares, a competition constructor, a puzzle publisher and three rule guides. Sudoku sources also require boxes; this edition deliberately follows the Latin-only definition from the first source and explicitly omits boxes. An academic DOI returned no content and was not counted as a read source.

## Build and tests
JDK17/AndroidSDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/knight-test src/com/gg007/knightcress/Board.java BoardTest.java then java -cp /tmp/knight-test com.gg007.knightcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your private signing material. No signing secret is included. adapter/android contains the Java2D drawing adapter used with KnightAdapterTest.java, not an Android runtime.

## Privacy and branding
Knightcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, knight-reach marks and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 menu, original icon, studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative216-card studio and static publishing fragments privately preserved:
https://files.instinct.com/k5er2jpb5ig8-knightcress-source-archive
https://github.com/iLanis-agent/knightcress holds README only, full Git source pending. Existing Jekyll includes remain unchanged; no Pages settings changes or client loader. Both sites verified separately.

## Rule sources
https://blog.tanyakhovanova.com/2022/03/fun-with-latin-squares/
https://ihnnpuzzles.blogspot.com/2024/09/puzzles-668-669-670-24hpc-zodiac-little.html
https://www.gmpuzzles.com/blog/2025/07/anti-knight-sudoku-by-philip-newman/
https://sudoku.by/faq/how-to-play/antiknight
https://variantsudoku.com/learn/antiknight/
https://sudokuvariants.com/help/variants/anti-knight/
