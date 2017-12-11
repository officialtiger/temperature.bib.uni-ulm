# InfluxDB installation & configuration (Ubuntu/Debian)
## Installation
### Step 1: Downloading the InfluxDB-Package
```bash
wget https://dl.influxdata.com/influxdb/releases/influxdb_1.4.2_amd64.deb
```

### Step 2: Installation
```bash
sudo dpkg -i influxdb_1.4.2_amd64.deb
```

### Step 3: Start database server
```bash
influxd
```
##### Optionally start in screen
```bash
screen -d -m influxd
```
## Configuration
### Create database for measured values (do BEFORE Node-RED configuration!)
1. Open shell with `influx` on server (VM/Putty etc.)
2. `CREATE DATABASE DB_NAME`

#### For further configuration
Select database `USE DB_NAME`

Reset measured values `DROP SERIES FROM /.*/`
