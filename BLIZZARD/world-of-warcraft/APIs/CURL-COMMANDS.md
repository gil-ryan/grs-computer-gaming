# Utilize CURL for API Calls



## Examples

```
curl -u {client_id}:{client_secret} -d grant_type=client_credentials https://us.battle.net/oauth/token
```

```
curl -H "Authorization: Bearer {access_token}" https://us.api.blizzard.com/data/wow/token/?namespace=dynamic-us
```

```
{
    "_links": {
        "self": {
            "href": "https://us.api.blizzard.com/data/wow/token/index?namespace=dynamic-us"
        }
    },
    "last_updated_timestamp": 1536597360000,
    "price": 1138480000
}
```

## Python

OK - so I'm starting to finally make some kind of progess. Not a lot, but some.


```python
import requests,json

r = requests.get('https://us.api.blizzard.com/data/wow/leaderboard/hall-of-fame/uldir/alliance?namespace=dynamic-us&locale=en_US&access_token=US5jwGwLcqXejsw3A3RSiYJfuE6OsFXjxP')

j = json.loads(r.text)
print(json.dumps(j, indent=4))

x = r.json()
for key, value in x.items():
    print(key, ' : ', value)

x.items()
x.keys()
x.values()
```
