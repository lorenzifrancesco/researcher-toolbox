# Julia installation in CloudVeneto machine
Installation in a Ubuntu machine
## Install Julia
```sudo apt-get install snap``` 
```sudo snap install julia --classic```
run julia updates

## Setting up GitHub 
generate the key https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

after the generation, just add to the GitHub ssh access keys https://github.com/settings/keys, bey copying the content of the file ```cat ~/.ssh/id_rsa.pub``` 

one can configure the local Git to use the account
```git config --global user.email "francesco.lorenzi.2@phd.unipd.it"```
test with 
```ssh -T git@github.com```

## Add package to be developed in ~/.julia/dev
If the github repo is private, copy the ssh key or generate a new one (better)
```scp -P 2080 -i ~/.ssh/certificates/Lorenzi.pem ~/.ssh/certificates/Lorenzi.pem ubuntu@localhost:/home/ubuntu/.ssh/Lorenzi.pem```