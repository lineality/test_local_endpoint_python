# test_local_endpoint_python


## Make Env, open editor:
```
python3 -m venv env; source env/bin/activate

python3 -m pip install --upgrade pip; python3 -m pip install requests

nano send_resquests.py
```

## Add text to file:
```
import requests 
text = input("enter text: ")
payload = {'text': text}
r = requests.post('http://10.88.0.4:5000', json=payload)
# print(r.text)
print("predictions: ", r.text)
```

## Run:
```
$ python send_resquests.py
```
