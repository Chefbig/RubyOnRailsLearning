# RubyOnRailsLearning


When vagrant report GuestAdditions not match with the host:

```shell
vagrant plugin install vagrant-vbguest
```
The above command can help.

When guest report it need upgrade:

```shell
sudo apt-get update
sudo apt-get upgrade
```

## variables
  * variable's name
   * bad ones: var-some var_Some varSome aw_count * what's aw??  
   * good atricle_written snake_count

  * variable scope
   * Global $variable
   * Class @@variable
   * Instance @variable
   * Local variable
   * Block variable
