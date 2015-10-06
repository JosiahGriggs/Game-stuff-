
K@echo off
cls
echo Hello and Welcome.
:loop
:menu
cls
color 0a
color 1a
cls
echo 1.)Start
echo 2.)Exit
set /p number=

if %number% == 1 goto Game
if %number% == 2 Exit


if not defined number (
cls
goto loop
)

:Game
cls
echo Hello whats you name???
set /p name=
cls
echo Hello %name% would you like to start the game??? (y/n)
set /p hey=

if %hey% == y goto thegame
if %hey% == n menu
if %hey% == N menu
if %hey% == Y goto thegame

:thegame
echo The is the one and only level.
echo.
echo do pig like mud??? (y/n)
set /p level=

if %hey% == y goto youwin
if %hey% == n menu
if %hey% == N menu
if %hey% == Y goto youwin




:youwin
cls
echo wow that was hard how did you win???
echo by
goto menu
