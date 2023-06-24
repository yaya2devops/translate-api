# Develop and Secure Translate APIs

The project demonstrates the process of developing, [securing](policies) and creating a product-ready API for translation.

To access the translation API, you can use the following endpoint
```sh
https://api.gtranslater.com/translate/v1?lang=
```

To specify the desired language, append the lang code parameter at the end of the URL e.g. add `lang=de` to the API endpoint for german translation.



## API Usage

Discover how our API can accurately translate text from English to German. 


Experience the convenience of our service with this example request
```sh
IP@apigeex-vm:~$ curl -i -k -X POST "https://api.gtranslater.com/translate/v1?lang=de" \
>     -H "Content-Type:application/json" \
>     -H "Key: $KEY" \
>     -d '{ "text": "Hey, Im Yahya a DevOps Consultant" }'
```

Unlock further seamless language translation with our German Translation API. 


```JSON
HTTP/2 200 
content-type: application/json
x-request-id: 98af2e9c-a33e-468b-9aa0-b09b2e76ca0a
content-length: 57
date: Sat, 24 Jun 2023 15:47:05 GMT
via: 1.1 google
alt-svc: h3=":443"; ma=2592000,h3-29=":443"; ma=2592000

{"translated":"Hallo, ich bin Yahya, ein DevOps-Berater"}
```

Curious about my profession more? Witness the power of our translation API in action



```sh
IP@apigeex-vm:~$ curl -i -k -X POST "https://api.gtranslater.com/translate/v1?lang=de" \
>     -H "Content-Type:application/json" \
>     -H "Key: $KEY" \
>     -d '{ "text": "I work in the cloud to provide value" }'
```


Transform text from English to German effortlessly

```JSON
HTTP/2 200 
content-type: application/json
x-request-id: 6e535c4c-2f63-4771-b99c-7497ab5a9cdb
content-length: 66
date: Sat, 24 Jun 2023 15:48:41 GMT
via: 1.1 google
alt-svc: h3=":443"; ma=2592000,h3-29=":443"; ma=2592000

{"translated":"Ich arbeite in der Cloud, um Mehrwert zu schaffen"}
```

The API allows you to translate in wide range of languages. Consult [supported languages.](https://cloud.google.com/translate/docs/languages)




## License

Distributed under the MIT License. See [LICENSE](LICENSE) for more information.

