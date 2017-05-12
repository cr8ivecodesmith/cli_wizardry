#### Check your public IP and geolocation

This uses freely available web services

Usage:

```
curl -s icanhazip.com/s | xargs printf 'freegeoip.net/json/%s' | xargs curl -s
```


#### Make this your own script

```
echo "curl -s icanhazip.com/s | xargs printf 'freegeoip.net/json/%s' | xargs curl -s" \
    | sudo tee -a /usr/bin/whatismyip
sudo chmod +x /usr/bin/whatismyip
```

or as single command:

```
echo "curl -s icanhazip.com/s | xargs printf 'freegeoip.net/json/%s' | xargs curl -s" | sudo tee -a /usr/bin/whatismyip && sudo chmod +x /usr/bin/whatismyip
```

Usage:

```
whatismyip
```
