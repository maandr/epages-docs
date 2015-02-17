---
layout: page
title: OAuth
category: gettingstarted
---

{% callout danger maybe OAuth 2.0? %}
  maybe OAuth 2.0?
{% endcallout %}

# OAuth authentication. Why?
Your app cannot access the REST API resources without authenticating first. All API calls are authenticated according to the OAuth 1.0 protocol.

All developers have to register their application before getting started. A registered OAuth 1.0 application is assigned the following:

| Name               | Description                                                                                                                                        |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|
| Consumer key       | Identifier string generated by API for use in OAuth 1.0.                                                                                           |
| Consumer secret    | Unique token generated for use in OAuth 1.0 as an element of creating a signature. The consumer secret should not be shared.                       |
| OAuth token        | Token generated by the server upon signed request. Can be either `request_token` or `access_token` depending on which step in the flow you are on. |
| OAuth token secret | Secret generally sent with the response for a certain token. Used for exchange, signature generation, or refreshing the `access_token`.            |

Fancy more detailed information? Here you go: [OAuth 1.0 protocol](https://tools.ietf.org/html/rfc5849).

# Authorisation

1. Within your test shop backoffice, again choose the tab **Apps**.
2. Choose the field **Private Apps** and click the button **Create app**.
3. Click the button **Test authorisation**. You will be requested to enter the **Application callback URL** and **Application notification URL**.
4. Click the button **Test authorisation** again. You will be forwarded to an external page to complete the authorisation process.
5. Once the test authorisation has been finished successfully, you will be fowarded to

{% callout danger Authorisation to be described %}
  development in progress
{% endcallout %}