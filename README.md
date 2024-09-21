[![PHP](https://github.com/olegabr/php-ethereum-address/actions/workflows/php.yml/badge.svg)](https://github.com/olegabr/php-ethereum-address/actions/workflows/php.yml)
[![codecov](https://codecov.io/gh/olegabr/php-ethereum-address/branch/main/graph/badge.svg)](https://codecov.io/gh/olegabr/php-ethereum-address)
[![Licensed under the MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/olegabr/php-ethereum-address/blob/main/LICENSE)

```lang=bash
$ composer require olegabr/ethereum-address
```

## Usage

Create a new address:

```php
<?php

require_once 'vendor/autoload.php';

use kornrunner\Ethereum\Address;

$address = new Address();

// get address
$address->get();
// 4e1c45599f667b4dc3604d69e43722d4ace6b770

$address->getPrivateKey();
// 33eb576d927573cff6ae50a9e09fc60b672a8dafdfbe3045c7f62955fc55ccb4

$address->getPublicKey();
// 20876c03fff2b09ea01861f3b3789ada54a20a8c5e90170618364cbb02d8e6408401e120158f489376a1db3f8cde24f9432976d2f89aeb193fb5becc094a28b9
```

Or load one from private key:

```php
<?php

require_once 'vendor/autoload.php';

use kornrunner\Ethereum\Address;

$privateKey = '33eb576d927573cff6ae50a9e09fc60b672a8dafdfbe3045c7f62955fc55ccb4';
$address = new Address($privateKey);

// get address
$address->get();
// 4e1c45599f667b4dc3604d69e43722d4ace6b770

$address->getPrivateKey();
// 33eb576d927573cff6ae50a9e09fc60b672a8dafdfbe3045c7f62955fc55ccb4

$address->getPublicKey();
// 20876c03fff2b09ea01861f3b3789ada54a20a8c5e90170618364cbb02d8e6408401e120158f489376a1db3f8cde24f9432976d2f89aeb193fb5becc094a28b9
```

## License

MIT

## Crypto

[![Ethereum](https://user-images.githubusercontent.com/725986/61891022-0d0c7f00-af09-11e9-829f-096c039bbbfa.png) 0x9c7b7a00972121fb843af7af74526d7eb585b171][Ethereum]

[Ethereum]: https://etherscan.io/address/0x9c7b7a00972121fb843af7af74526d7eb585b171 "Donate with Ethereum"
