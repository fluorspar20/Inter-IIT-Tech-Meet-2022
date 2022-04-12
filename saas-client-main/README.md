# Saas Client
SEC Filing Analyzer for Saas Companies
> Live demo [_here_](https://festive-raman-e6e4ba.netlify.app/)

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Features](#features)
* [Setup](#setup)
* [Usage](#usage)
* [Screenshots](#screenshots)

## General Information
- This repository serves as the frontend of our submission to Inter IIT Tech Meet 2022's High Prep Problem Statement: DIGITAL ALPHA'S SEC FILING ANALYZER FOR SAAS COMPANIES.

## Technologies Used
- React
- Apollo Client with GraphQL
- Tailwind CSS
- ReChart
- AntD

## Features
- Easy Navigation for SEC filings
  - Breakdown into seperate sections of 10-K and 10-Q forms
  - Corresponding links attached
- Highly Interactive Drilldown menu
  - Capable of zooming and pannig across time range
- Various financial ratios' calculation and display
- Overall score prediction using Machine Learning on the basis of financial ratios
- Detailed Summary of 8-K forms using NLP for sentiment analysis
- Comparison of Multiple Companies for raw data and financial ratios
- Downloadable data in different formats


## Setup
`Node` is a required dependency.
```bash
# to install dependencies
$ npm install
```

## For Docker: 
```bash
docker build . -t saas-app          
docker run -p 5000:5000 -d  --name node2 saas-app
docker rm node2 -f
```

## Usage
```bash
# to start server
$ npm run dev # for development mode
$ npm run prod # for production mode
```
