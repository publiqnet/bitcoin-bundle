BitcoinBundle
========================

Instalation
-----------

Install via composer
```shell
composer require blockchainrndhub/ethereum-bundle
```
Enable the bundle in your kernel
-----------
```php
# app/AppKernel.php
$bundles = [
    //...
    new Blockchainrndhub\EthereumBundle\BlockchainrndhubEthereumBundle(),
    //...
];
```
Add config
-----------
```yaml
# app/config/config.yml
  
    blockchainrndhub_ethereum:
        etherscan_api_key: '%etherscan_api_key%'
```


Add parameters
-----------
```yaml
# app/config/parameters.yml
  
    parameters:
        etherscan_api_key: YOUR_API_KEY
```


Usage
-----------
```yaml

  $etherscan = $this->container->get('ethereum_etherscan');

    
```
