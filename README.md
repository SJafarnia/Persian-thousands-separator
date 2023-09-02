# Thousands-separator

Script for switching English numbers to Persian/Arabic numbers and separates them by thousands (with commas).

it is created as a Django template filter but you can just use the function anywhere you need.

## filter example 

```bash
{% load thousands("or your custom template filters file name") %}

{{ product.price|separator:"fa" }}

{{ product.price|separator:"ar" }}
```

This function takes 2 arguments:

```bash 
num: input number
```
```bash
lang (str): target language ('fa' for Persian, 'ar' for Arabic, None for just returning the input number separated by thousands).
```
```bash
returns: str: a string of the input number separated by thousands and translated to target language.
```
