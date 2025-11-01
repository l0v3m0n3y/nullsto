# nullsto
temp email web api nullsto.edu.pl nim-lang
# Example
```nim
import asyncdispatch, nullsto, json
waitFor init_cookie()
let data = waitFor get_messages()
echo data["mailbox"].getStr
let messages = waitFor get_messages()
echo messages["messages"]
```
# Launch (your script)
```
nim c -d:ssl -r  your_app.nim
```
