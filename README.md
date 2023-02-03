thousands-separator
Script for switching English numbers to Persian/Arabic numbers and separates them by thousands (with commas).

it is created as a Django template filter but you can just use the function anywhere you need.

filter example :

{% load thousands("or your custom template filters file name") %}

{{ produc.price|separator:"fa" }}

{{ produc.price|separator:"ar" }}

the function takes 2 arguments:

num: input number

lang (str): target language ('fa' for Persian, 'ar' for Arabic, None for just returning the input number separated by thousands).

Returns: str: a string of the input number separated by thousands and translated to target language.