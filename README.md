# Assisting-Machine
A machine that assists.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Can you help me with that, machine?" \
  | uvx assisting-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install assisting-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
assisting-machine -a multilogue.txt
```
Or:
```bash
assisting-machine multilogue.txt > response.txt
```
Or:
```bash
assisting-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import assisting_machine
```
