BitcoinBundle
========================

Instalation
-----------

Install via composer
```shell
composer require blockchainrndhub/bitcoin-bundle
```
Enable the bundle in your kernel
-----------
```php
# app/AppKernel.php
$bundles = [
    //...
    new Blockchainrndhub\BitcoinBundle\BlockchainrndhubBitcoinBundle(),
    //...
];
```
Add config
-----------
```yaml
# app/config/config.yml
  
    blockchainrndhub_bitcoin:
        bitcoin_api_key: '%bitcoin_api_key%'
```


Add parameters
-----------
```yaml
# app/config/parameters.yml
  
    parameters:
        bitcoin_api_key: YOUR_API_KEY
```


Usage
-----------
```yaml

  $bitcoinscan = $this->container->get('bitcoin_scan');

    
```
