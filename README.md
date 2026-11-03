# Voting-Machine
A machine that votes in one of the voting schemes.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: How will you cast your vote, machine?" \
  | uvx voting-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install voting-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
voting-machine -a multilogue.txt
```
Or:
```bash
voting-machine multilogue.txt > response.txt
```
Or:
```bash
voting-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import voting_machine
```
