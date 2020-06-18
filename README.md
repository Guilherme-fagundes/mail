# Mail

#### Instalation

```bash
composer require coffeebreaks/mail
```


##### Example

```php

$mail = new \coffeebreaks\Mail();
$mail->config('smtp.your-host.com', 'your-user',
    'you-pass', port);
$mail->add('suport@exemple.com', 'Suport',
    'your-mail@domain.com', 'Test classe Mail',
    "This is a email with <b>PhpMailer</b> and generic class <i>Mail</i>");

if ($mail->getResult()){
    echo "Success :)";
}

```