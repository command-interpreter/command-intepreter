# Command-Interpreter
A Machine that interprets arbitrary textual commands.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Are language models seeking the Truth, machine?" \
  | uvx command-interpreter \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install command-interpreter
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
command-interpreter -a multilogue.txt
```
Or:
```bash
command-interpreter multilogue.txt > response.txt
```
Or:
```bash
command-interpreter -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import command_interpreter
```
