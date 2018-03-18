# gh-hooks-server
A simple python server that runs a bash script when it receives a POST from a GitHub Webhook

# Install
```
python setup.py install
```
# Usage:
```
ghhooks [-h] [--port PORT] [-a MAPPINGS] [--secret SECRET]

optional arguments:
  -h, --help       show this help message and exit
  --port PORT      HTTP port to listen (default 8011)
  -a MAPPINGS      Add a new path mapping from a url path to a bash script
                   (format key:path)
  --secret SECRET  A secret that validates X-Hub-Signature
```

# Usage Demo
```
ghhooks --port 8899 -a deploy:~/deploy.sh --secret s3cret