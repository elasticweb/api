# The example query to the API with PHP

## GET

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://elasticweb.org/api/dns/entry/1');
curl_setopt($ch, CURLOPT_RETURNTRANSFER, 1);
curl_setopt($ch, CURLOPT_VERBOSE, 0);
curl_setopt($ch, CURLOPT_HEADER, 0);
curl_setopt($ch, CURLOPT_SSL_VERIFYPEER, FALSE);

curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'X-API-KEY: {YOUR_API_KEY}',
]);

$response = curl_exec($ch);
curl_close($ch);

echo $response;
```

## POST

```php
$fields = [
  'server' => '3',
  'domain' => 'test.com',
  'nginx_id' => '1',
];

$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://elasticweb.org/api/account/entry');
curl_setopt($ch, CURLOPT_RETURNTRANSFER, 1);
curl_setopt($ch, CURLOPT_VERBOSE, 0);
curl_setopt($ch, CURLOPT_HEADER, 0);
curl_setopt($ch, CURLOPT_SSL_VERIFYPEER, FALSE);
curl_setopt($ch, CURLOPT_POST, TRUE);
curl_setopt($ch, CURLOPT_POSTFIELDS, http_build_query($fields));

curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'X-API-KEY: {YOUR_API_KEY}',
]);

$response = curl_exec($ch);
curl_close($ch);

echo $response;
```

## PATCH

```php
$fields = [
  'status' => '1',
];

$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://elasticweb.org/api/account/entry/1');
curl_setopt($ch, CURLOPT_RETURNTRANSFER, 1);
curl_setopt($ch, CURLOPT_VERBOSE, 0);
curl_setopt($ch, CURLOPT_HEADER, 0);
curl_setopt($ch, CURLOPT_SSL_VERIFYPEER, FALSE);
curl_setopt($ch, CURLOPT_CUSTOMREQUEST, 'PATCH');
curl_setopt($ch, CURLOPT_POST, TRUE);
curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode($fields));

curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'X-API-KEY: {YOUR_API_KEY}',
]);

$response = curl_exec($ch);
curl_close($ch);

echo $response;
```
