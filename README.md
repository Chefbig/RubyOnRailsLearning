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

Mid term reviews
  * [data types and variables](reviews/mid-review-data_types.md)
  * [control flow](reviews/control_flow.md)
  * [find, merge, collect, sort, inject](reviews/code_block.md)
  * [method](reviews/method.md)
  * [class](reviews/class.md)
  * [modules](review/modules.md)
  
Magic variables
``` ruby
  $: # folders where ruby will search for files
  __FILE__ # current file path
```
