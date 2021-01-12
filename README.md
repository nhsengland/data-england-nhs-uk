The home page for [data.england.nhs.uk](https://data.england.nhs.uk)

deployment.
update your hosts file with the server and a variable called `DEV`.

DEV=1 will deploy update certbot, DEV=0 will just deploy to an ec2 server.

e.g.
```
[webserver]
ec2-34-241-54-129.eu-west-1.compute.amazonaws.com DEV=0
```

run
```
cd deployment
ansible-playbook setup.yml -i hosts.dev
```