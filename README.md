## Install postgresql

```sh
sudo apt install postgresql
sudo -u postgres psql template1
alter user postgres with encrypted password 'postgres';
\q
psql -h localhost -U postgres
create user galaktika encrypted password 'galaktika' createdb;
create database galaktika template template0 owner galaktika locale 'en_US.utf8' encoding UTF8;
\q
```

## Install python

```sh
sudo apt install software-properties-common -y
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt install python3.12 python3.12-venv
```

In the project directory, create a python virtualenv and install pip

```sh
python3.12 -m venv .python_venv
```
