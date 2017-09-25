# Docker workstation setup
After cloning the directory, symlink it to your home directory

```bash
ln -s docker-workstation/docker-compose.yml ~/docker-compose.yml
```

and add the following lines to your ~/.zshrc or ~/.bashrc
```
alias drush='docker-compose exec php drush'
alias drupal='docker-compose exec php drupal'
```

## php container with drupal code

## dns container for resolving docker hostnames
  
### Setup

```bash
echo "nameserver	127.0.0.1" | sudo --tee /etc/resolver/docker2
```
