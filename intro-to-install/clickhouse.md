# Install Clickhouse 

> Ubuntu 20.04

1. STEP 1: Install apt-transport Package
``` 
sudo apt update 
```

``` 
sudo apt install apt-transport-https ca-certificates 
```

2. STEP 2: Add the Repository GPG Key
``` 
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv E0C56BD4 
```

3. STEP 3: Add ClickHouse to APT Repository
``` 
echo "deb http://repo.yandex.ru/clickhouse/deb/stable/ main/" | sudo tee /etc/apt/sources.list.d/clickhouse.list 
```

``` 
sudo apt update 
```

4. STEP 4: Install ClickHouse Server and Client
``` 
sudo apt install clickhouse-server clickhouse-client 
```

Source: https://phoenixnap.com/kb/install-clickhouse-on-ubuntu-20-04
