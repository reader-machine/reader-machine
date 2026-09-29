# Reader-Machine
A Machine that reads.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Read this, machine." \
  | uvx reader-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install reader-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
reader-machine -a multilogue.txt
```
Or:
```bash
reader-machine multilogue.txt > response.txt
```
Or:
```bash
reader-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import reader_machine
```
