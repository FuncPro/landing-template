update: venv/bin/python
	aws s3 sync www/ s3://$(python stack.py {{ cookiecutter.domain_name }}) --delete --acl public-read


venv/bin/python:
	virtualenv -p python3 venv
	venv/bin/pip install troposphere boto3 awscli
