# Project Background

## The Problem
For those unfamiliar with the game it is a six player board game during which players will vie for control of areas on the board aiming to maintain a grasp on enough castles to be declared the winner. Remaining true to the books and show players inevitably end up making and breaking truces, fighting, lying, manipulating and frustrating one another over the course of several hours. 

This is a complicated game with several different mechanics, partially disclosed information, and many many moving parts. In this version I am attemping to create a game which players can play with one another simultaneously online (as they might in person) or over a longer period of time, where they log-in to their game and are prompted for thier next move. Whilst people have enjoyed play-by-forum games these require an additional person to act as moderator, managing the secret orders and moving the game on. I am aiming to automate the whole game such that no moderator is required. 

## The Previous Attempts

This is my sixth (I think) attempt to produce a system through which players could play remotely from one another. The first five ideas are outlined below. 
1. Google Sheets & Google Script - a system of seven google interlinked google sheets (one for each player plus a moderator) by which the six players could submit their orders in obfuscated text and then have these orders automatically returned to plain text when all secret order submisions were made. The game was then played manually using the online [play-by-forum game maps](tinyurl.com/5bmhdayp).
2. Goodle Sheets & Google Script V2 - built on the previous system this also included the ability to submit house cards, secretly view the wildling deck, have the westeros deck cards automatically generated. Several rounds of a game were successfully played using this system. Unfortunately I broke the version we were using by removing image files hosted elsewhere...
3. HTML and iframes - an entirely unsuccessful short lived endevour to use the existing play-by-forum maps within an iframe and automate the rest of the game on the page. 
4. HTML, CSS and Javascript - a purpose built version of the play-by-forum map using javascript to run the game in browser (providing prompts, decisions, and information). This is the first iteration of the game that is currently in development. The major flaw was that while several players could play simultaneously each would have to reload their webpage to check for changes in the game state and potentially move the game on.
5. HTML, CSS, Javascrip and NodeJS - A very nearly complete version of the game. A server running nodeJS handling the game itself, pushing infomation out to each player and processing information players sent back. While this attempt was planned and written in a modular fashion it's stability certainly suffered from the constant editing of functionality during development as different phases of the game were programmed. Additionally the approach to manipulating and storing the game state created headaches later on. The current version is essentially this approach of server-side and client-side javascript rewritten to utilise a better data structure in a more modular way.

## Disclaimer

I am not a programmer by education, I have taught myself HTML, CSS and Javascript in the process of working on this project. As I have learnt more about programming in JS, utilising different techniques and features of the language I suspect I have over-used particular tools where others would be more appropriate, and written some generally inefficient code. Please do point out my poor programming and help me improve!
I have also found out recently there now exists an official online version of the game! I don't consider the time entirely wasted - only partially. 
