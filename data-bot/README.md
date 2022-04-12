# Data Bot
> This is a python web crawler plus analysis generator. It scrapes data from SEC EDGAR's database for the required SaaS companies and uses Machine Learning, Natural Language Processing to analyse the scraped data.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Setup](#setup)

## General Information

- This repository serves as the web scraper of our submission to Inter IIT Tech Meet 2022's High Prep Problem Statement: DIGITAL ALPHA'S SEC FILING ANALYZER FOR SAAS COMPANIES.

- SaaS companies are customer-driven and are heavily dependent on their customer base. There
  are a set of metrics that can showcase the health of the SaaS companies and their aspects. These
  metrics and numbers are not readily available on publicly reported SEC Filings and need to be
  chalked out from the available forms (10-K, 10-Q, 8-K, etc.).

- Accessing these metrics can be of tremendous value to the users looking to invest. However, the forms filed in SEC are very detailed, diverse and take time to analyze. Thus, we propose an interactive dashboard capable of analyzing SEC Filings to the SaaS companies and investors alike to quickly overview the Key SaaS Goals and data to make an informed decision.

## Technologies Used
- Flask 
- Firebase
- XGBoost
- Transformers

## Features 
|                  | bad        | neutral    | good       |
|------------------|------------|------------|------------|
| precision_score: | 0.95454545 | 0.82       | 0.75       |
| recall_score:    | 0.91304348 | 0.84375    | 0.84375    |
| f1_score:        | 0.93333333 | 0.80392157 | 0.79411765 |

## Setup
- Install all the package requirements from requirements.txt using $ pip install -r requirements.txt
- Add your [refinitiv](https://developers.refinitiv.com/en) API token - [Here](https://github.com/hp-da17/HP_DA_T17/blob/d408b85c7a1016ca4decb2485976a3b1c5da35f2/data-bot/scrape_utils.py#L362)
- Add your [AlphaVantage](https://www.alphavantage.co/support/) API Token - [Here](https://github.com/hp-da17/HP_DA_T17/blob/d408b85c7a1016ca4decb2485976a3b1c5da35f2/data-bot/scrape_utils.py#L385)
