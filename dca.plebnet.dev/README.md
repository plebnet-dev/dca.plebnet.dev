[![Fly Deploy DCA Calculator](https://github.com/bitkarrot/dca-calculator/actions/workflows/main.yml/badge.svg)](https://github.com/bitkarrot/dca-calculator/actions/workflows/main.yml)

# DCA calculator for Bitcoin

This is an educational tool built with dash plotly python for dollar cost averaging of bitcoin, custom tailored for https://bitcoin.org.hk, with usd and hkd options.

Users can select options for daily, weekly, monthly Dollar Cost averaging of bitcoin in multiple currencies. The result of the form will be a total amount of bitcoin stacked and a plot chart that shows total accumulation over a the specified time range. 

## Install

```sh

git clone https://github.com/bitkarrot/dca-calculator.git
cd dca-calculator
python3 -m venv venv 
pip install -r requirements.txt
python3 app.py
```

## Deploy on fly.io

deploy using the Docker container with 

```sh
  fly launch --dockerfile Dockerfile
```

## Run with gunicorn

```sh
gunicorn app:server

```
