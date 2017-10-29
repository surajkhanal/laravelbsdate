# A Laravel Nepali Date.

[![Latest Stable Version](https://poser.pugx.org/shankhadev/bsdate/v/stable)](https://packagist.org/packages/shankhadev/bsdate)
[![License](https://img.shields.io/github/license/shankhadevpadam/laravelbsdate.svg?style=flat-square)](https://packagist.org/packages/shankhadev/bsdate)
[![Total Downloads](https://img.shields.io/github/downloads/shankhadevpadam/laravelbsdate/total.svg?style=flat-square)](https://packagist.org/packages/shankhadev/bsdate)
[![StyleCI](https://styleci.io/repos/102555089/shield?branch=master)](https://styleci.io/repos/102555089)

A laravel date package which convert AD to BS and viceversa.

#Installation
1) In order to install Laravel 5 Laravelbsdate, just add the following to your composer.json in require. Then run composer update:

```json
"shankhadev/bsdate": "master-dev"
```

2) Open your `config/app.php` and add the following to the `providers` array:

```php
Shankhadev\Bsdate\BsdateServiceProvider::class,
```

3) In the same `config/app.php` and add the following to the `aliases ` array: 

```php
'Bsdate' => Shankhadev\Bsdate\BsdateFacade::class,
```

## Usage

```php
Bsdate::eng_to_nep(2016,12,31); //For converting AD TO BS
Bsdate::nep_to_eng(2073,09,16); //For converting BS TO AD
// output 
Array
(
    [year] => २०७३
    [month] => ९
    [date] => १६
    [day] => शनिबार
    [nmonth] => पुष
    [num_day] => ७
)
```
