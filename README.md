## Prompt Engineering for Devs (by DeepLearning)

### Requirements
asdf (to read the .tools-versions file)
Python 3.12+

### Running APP
```shell
python -m venv .venv
```

```shell
source .venv/bin/activate
```

```shell
python -m pip install --upgrade pip
```

```shell
pip install -r devtools/requirements.txt
```

### How do get OPENAI Keys
https://platform.openai.com/docs/overview?lang=python

### If you installed new libraries, check the differences, to add on devtools/requirements.txt
```shell
diff <(pip list --not-required --format=freeze) devtools/requirements.txt | grep '^<' | while read -r line; do echo "${line#< }"; done
```