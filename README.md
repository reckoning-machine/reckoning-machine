# Reckoning-Machine
Reckoning machine.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Reckon the outcome, machine." \
  | uvx reckoning-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install reckoning-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
reckoning-machine -a multilogue.txt
```
Or:
```bash
reckoning-machine multilogue.txt > response.txt
```
Or:
```bash
reckoning-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import reckoning_machine
```
