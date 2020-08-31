Usage Example
$message = 'Ready your ammunition; we attack at dawn.';
$key = hex2bin('000102030405060708090a0b0c0d0e0f101112131415161718191a1b1c1d1e1f');

$encrypted = SaferCrypto::encrypt($message, $key);
$decrypted = SaferCrypto::decrypt($encrypted, $key);

var_dump($encrypted, $decrypted);
