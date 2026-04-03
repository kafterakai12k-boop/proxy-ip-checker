import requests
url = 'https://ip.decodo.com/json'
username = 'user-spswmfhurf-country-us-zip-20715'
password = 'Ui8wK9GuOa4uy6i+sf'
proxy = f"http://{username}:{password}@us.decodo.com:10001"
result = requests.get(url, proxies = {
    'http': proxy,
    'https': proxy
})
print(result.text)
