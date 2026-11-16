# Welcome to LunaNova Games!

We're a three-person team building **LunaNova**, an open-source web app for finding games and comparing their prices. It started as our entry for the Terranova Software *Gaming Explorer* challenge, and it's the first thing any of us has built with C#, ASP.NET Core or Angular.

In the code you'll see it called **Lune**, our internal name for the project.

![The LunaNova home page](https://github.com/Terranova-hackathon/lune/blob/main/docs/images/home-featured.png)

## The project in 10 minutes

<!-- For Minoka and Kelvin to fill out :)  -->

**[Video placeholder: the presentation video goes here]**

**[Summary placeholder: a short description of the project, the difficulties we ran into, and how we solved them]**

## What LunaNova does

You can search thousands of games by name, with suggestions as you type, and narrow the results by genre, platform, developer, publisher or critic score. Each game has its own page with a description, screenshots, ratings and related games, plus a price comparison showing the current price and the lowest recorded price on Steam and GG.deals. It has a game comparison tool that follows you across pages, letting you add games and compare key features and prices. With a free account you can save games to your favorites and return to them later. The site works on phones as well as desktops, in dark or light mode.

## How it's built

The backend is an ASP.NET Core API split into independent modules for accounts, games, favorites and prices, each with its own part of a SQL Server database. That design paid off when the game API suggested in the brief went offline partway through the project: we moved to IGDB without having to rework the rest of the app. The frontend is written in Angular, and the whole stack starts with a single `docker compose up`.

We also put time into making the project easy to check and to work on. The API documents itself in an interactive reference generated from the code, and an automated suite of 79 requests and 164 tests covers every endpoint, including its error cases.

## The team

We worked mostly asynchronously, coordinating through GitHub issues and reviewing each other's pull requests before anything was merged.

- **Kelvin Lemayian**, lead frontend developer
- **Minoka Kakizaki**, lead backend developer
- **Francesca Frattaroli**, testing, documentation and deployment

## Our repositories

- **[Lune](https://github.com/Terranova-hackathon/lune)** is the LunaNova app itself: backend, frontend, tests and documentation. It was frozen for evaluation on 2026-11-15, so this is the place to start. Its README explains how to [run it yourself](https://github.com/Terranova-hackathon/lune#quick-start).
- **[AspNet-Angular Prototype](https://github.com/Terranova-hackathon/asp.net-angular-prototype)** is where we taught ourselves ASP.NET Core and Angular before starting on Lune.
- **[Lune Launch](LAUNCH_REPO_URL)** will hold our experiments with deploying LunaNova to production...for future development.
