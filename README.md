# Meraki Data analysis through isolation forest algorithm

In this code we analyze data from Meraki API. We've enhanced our Meraki data analysis toolkit by integrating the Isolation Forest algorithm. This powerful method is excellent for detecting anomalies in large datasets, helping to identify unusual patterns or outliers that standard analysis might miss.

## Installation
Install `docker` and `docker-compose` previously.

Clone the repo
```bash
git clone https://github.com/mighidalgo/isolation-forest.git
```

Go to your project folder
```bash
cd isolation-forest
```

## Usage

Run docker compose
```bash
docker-compose up -d
```

Now you have the project up and running, enter the URL
```bash
http://localhost:8001/isolation-forest - Isolation forest algorithm.
```

## Configuration

- In order to fetch data from Meraki API, we need to set this env variables in the `docker-compose` file
  - `BASE_URL` - Required, Meraki API URL.
  - `API_KEY` - Required, Apikey to access the API.
  - `ORG_ID` - Optional, if you want the data from a specific organization of the Meraki data, set this var.
  - `ISOLATION_SENSITIVITY` - Required, value used with the isolation forest algorithm

## Example
- Run the Isolation Forest analysis on your Meraki dataset to identify potential anomalies. The output will list any data points that are considered statistically unusual, aiding in deeper data investigations.

## Additional Notes
The Isolation Forest algorithm is particularly effective on large datasets. Performance may vary depending on the size and complexity of your data.

## Hardware and Software requirements

You can run this project by just installing `docker` and `docker-compose` on your machine or server.
Recommendend hardware is 4 GB of ram and a dual core processor.
