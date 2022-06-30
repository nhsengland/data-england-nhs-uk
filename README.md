The home page for [data.england.nhs.uk](https://data.england.nhs.uk)

deployment.
update your hosts.dev file with the correct server
e.g.
```
[webserver]
ec2-34-241-54-129.eu-west-1.compute.amazonaws.com
```

run
```
cd deployment
ansible-playbook setup.yml -i hosts.dev
```