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
## numbers
  * ``` 12345.6789.round ``` => 12346
  * ``` 12345.6789.to_i  ``` => 12345
  * ``` 12345.6789.ceil ``` => 12346
  * ``` 12345.6789.floor  ``` => 12345

## String
  * "Hello"
  * "1" * 5 ==> 11111
  * ```"\'"  ``` ====> escape \ 
