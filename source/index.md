# Finance

## Get merchant transactions from billing.invoice table

> Request

``` http
GET /merchant/merchants/{merchant_id}/finance/transactions/registry.{format}?datetime_from=2014-09-21&datetime_to=2014-09-22&limit=1&offset=1&in_transfer_currency=xsolla&show_total=xsolla HTTP/1.1
User-Agent: xsolla-api-client/1.0
Host: api.xsolla.com
Accept: application/json
Authorization: Basic ZGVtb0B4c29sbGEuY29tOmRlbW8=
Content-Type: application/json
```

``` shell
$ curl -v 'https://api.xsolla.com/merchant/merchants/{merchant_id}/finance/transactions/registry.{format}?datetime_from=2014-09-21&datetime_to=2014-09-22&limit=1&offset=1&in_transfer_currency=xsolla&show_total=xsolla' \
-X GET \
-u user_id:api_key
```


> Response

``` http
HTTP/1.1 200
Content-Type: application/json

[
    {
        "IdProject": "1",
        "NameProject": "1. Demo Project",
        "TransferDateFormat": "21.09.2014 17:02",
        "IdInvoice": "16575",
        "ReqInGame": "xso test4",
        "CodeInstance": "389. Paybyme (ARS)",
        "PaymentSum": "10 ARS",
        "CommissionXsolla": "0 ARS (5.00%)",
        "CommissionPs": "0 ARS (60.00%)",
        "PayoutSum": "0 ARS (78.80%)",
        "UserCommission": "2.12 ARS (21.20%)",
        "CommissionAgentReal": "0 ARS (65.00%)",
        "NominalSum": 0,
        "RefundReason": "",
        "NameStatus": "xsollaRefundFailed",
        "IsoCountry": "TR",
        "Phone": "905414468107",
        "Email": "",
        "TestProject": "0",
        "ExternalCommission": "0%",
        "OutProject": 0
    },
    {
        "IdProject": "1",
        "NameProject": "1. Demo Project",
        "TransferDateFormat": "21.09.2014 13:23",
        "IdInvoice": "86854",
        "ReqInGame": "test76 2",
        "CodeInstance": "16. QIWI (RUB)",
        "PaymentSum": "3 RUB",
        "CommissionXsolla": "0.17 RUB (5.00%)",
        "CommissionPs": "0.17 RUB (5.00%)",
        "PayoutSum": "3 RUB (100.00%)",
        "UserCommission": "0 RUB (0.00%)",
        "CommissionAgentReal": "0 RUB (10.00%)",
        "NominalSum": 3,
        "RefundReason": "",
        "NameStatus": "done",
        "IsoCountry": "RU",
        "Phone": "79638581817",
        "Email": "",
        "TestProject": "0",
        "ExternalCommission": "0%",
        "OutProject": 3
    },
    {
        "IdProject": "1",
        "NameProject": "1. Demo Project",
        "TransferDateFormat": "21.09.2014 09:55",
        "IdInvoice": "63415",
        "ReqInGame": "demo 1",
        "CodeInstance": "27. Yandex.Money (RUB)",
        "PaymentSum": "1 RUB",
        "CommissionXsolla": "0 RUB (5.00%)",
        "CommissionPs": "0 RUB (5.00%)",
        "PayoutSum": "0 RUB (100.00%)",
        "UserCommission": "0 RUB (0.00%)",
        "CommissionAgentReal": "0 RUB (10.00%)",
        "NominalSum": 0,
        "RefundReason": "",
        "NameStatus": "xsollaRefundFailed",
        "IsoCountry": "RU",
        "Phone": "",
        "Email": "",
        "TestProject": "0",
        "ExternalCommission": "0%",
        "OutProject": 0
    },
    {
        "IdProject": "1",
        "NameProject": "1. Demo Project",
        "TransferDateFormat": "21.09.2014 09:33",
        "IdInvoice": "1634",
        "ReqInGame": "demo 1",
        "CodeInstance": "27. Yandex.Money (RUB)",
        "PaymentSum": "1 RUB",
        "CommissionXsolla": "0.06 RUB (5.00%)",
        "CommissionPs": "0.06 RUB (5.00%)",
        "PayoutSum": "1 RUB (100.00%)",
        "UserCommission": "0 RUB (0.00%)",
        "CommissionAgentReal": "0 RUB (10.00%)",
        "NominalSum": 1,
        "RefundReason": "",
        "NameStatus": "done",
        "IsoCountry": "RU",
        "Phone": "",
        "Email": "",
        "TestProject": "0",
        "ExternalCommission": "0%",
        "OutProject": 1
    },
    {
        "IdProject": "1",
        "NameProject": "1. Demo Project",
        "TransferDateFormat": "21.09.2014 09:12",
        "IdInvoice": "60025",
        "ReqInGame": "demo 1",
        "CodeInstance": "27. Yandex.Money (RUB)",
        "PaymentSum": "1 RUB",
        "CommissionXsolla": "0.06 RUB (5.00%)",
        "CommissionPs": "0.06 RUB (5.00%)",
        "PayoutSum": "1 RUB (100.00%)",
        "UserCommission": "0 RUB (0.00%)",
        "CommissionAgentReal": "0 RUB (10.00%)",
        "NominalSum": 1,
        "RefundReason": "",
        "NameStatus": "done",
        "IsoCountry": "RU",
        "Phone": "",
        "Email": "",
        "TestProject": "0",
        "ExternalCommission": "0%",
        "OutProject": 1
    }
]

```

``` shell
[
    {
        "IdProject": "1",
        "NameProject": "1. Demo Project",
        "TransferDateFormat": "21.09.2014 17:02",
        "IdInvoice": "16575",
        "ReqInGame": "xso test4",
        "CodeInstance": "389. Paybyme (ARS)",
        "PaymentSum": "10 ARS",
        "CommissionXsolla": "0 ARS (5.00%)",
        "CommissionPs": "0 ARS (60.00%)",
        "PayoutSum": "0 ARS (78.80%)",
        "UserCommission": "2.12 ARS (21.20%)",
        "CommissionAgentReal": "0 ARS (65.00%)",
        "NominalSum": 0,
        "RefundReason": "",
        "NameStatus": "xsollaRefundFailed",
        "IsoCountry": "TR",
        "Phone": "905414468107",
        "Email": "",
        "TestProject": "0",
        "ExternalCommission": "0%",
        "OutProject": 0
    },
    {
        "IdProject": "1",
        "NameProject": "1. Demo Project",
        "TransferDateFormat": "21.09.2014 13:23",
        "IdInvoice": "86854",
        "ReqInGame": "test76 2",
        "CodeInstance": "16. QIWI (RUB)",
        "PaymentSum": "3 RUB",
        "CommissionXsolla": "0.17 RUB (5.00%)",
        "CommissionPs": "0.17 RUB (5.00%)",
        "PayoutSum": "3 RUB (100.00%)",
        "UserCommission": "0 RUB (0.00%)",
        "CommissionAgentReal": "0 RUB (10.00%)",
        "NominalSum": 3,
        "RefundReason": "",
        "NameStatus": "done",
        "IsoCountry": "RU",
        "Phone": "79638581817",
        "Email": "",
        "TestProject": "0",
        "ExternalCommission": "0%",
        "OutProject": 3
    },
    {
        "IdProject": "1",
        "NameProject": "1. Demo Project",
        "TransferDateFormat": "21.09.2014 09:55",
        "IdInvoice": "63415",
        "ReqInGame": "demo 1",
        "CodeInstance": "27. Yandex.Money (RUB)",
        "PaymentSum": "1 RUB",
        "CommissionXsolla": "0 RUB (5.00%)",
        "CommissionPs": "0 RUB (5.00%)",
        "PayoutSum": "0 RUB (100.00%)",
        "UserCommission": "0 RUB (0.00%)",
        "CommissionAgentReal": "0 RUB (10.00%)",
        "NominalSum": 0,
        "RefundReason": "",
        "NameStatus": "xsollaRefundFailed",
        "IsoCountry": "RU",
        "Phone": "",
        "Email": "",
        "TestProject": "0",
        "ExternalCommission": "0%",
        "OutProject": 0
    },
    {
        "IdProject": "1",
        "NameProject": "1. Demo Project",
        "TransferDateFormat": "21.09.2014 09:33",
        "IdInvoice": "1634",
        "ReqInGame": "demo 1",
        "CodeInstance": "27. Yandex.Money (RUB)",
        "PaymentSum": "1 RUB",
        "CommissionXsolla": "0.06 RUB (5.00%)",
        "CommissionPs": "0.06 RUB (5.00%)",
        "PayoutSum": "1 RUB (100.00%)",
        "UserCommission": "0 RUB (0.00%)",
        "CommissionAgentReal": "0 RUB (10.00%)",
        "NominalSum": 1,
        "RefundReason": "",
        "NameStatus": "done",
        "IsoCountry": "RU",
        "Phone": "",
        "Email": "",
        "TestProject": "0",
        "ExternalCommission": "0%",
        "OutProject": 1
    },
    {
        "IdProject": "1",
        "NameProject": "1. Demo Project",
        "TransferDateFormat": "21.09.2014 09:12",
        "IdInvoice": "60025",
        "ReqInGame": "demo 1",
        "CodeInstance": "27. Yandex.Money (RUB)",
        "PaymentSum": "1 RUB",
        "CommissionXsolla": "0.06 RUB (5.00%)",
        "CommissionPs": "0.06 RUB (5.00%)",
        "PayoutSum": "1 RUB (100.00%)",
        "UserCommission": "0 RUB (0.00%)",
        "CommissionAgentReal": "0 RUB (10.00%)",
        "NominalSum": 1,
        "RefundReason": "",
        "NameStatus": "done",
        "IsoCountry": "RU",
        "Phone": "",
        "Email": "",
        "TestProject": "0",
        "ExternalCommission": "0%",
        "OutProject": 1
    }
]
```

Get transactions registry

### HTTP REQUEST

`GET https://api.xsolla.com/merchant/merchants/{merchant_id}/finance/transactions/registry.{format}`


Parameter | Type | Description
--------- | ---- | -----------
merchant_id | int | Merchant ID
format |  |
datetime_from | datetime |
datetime_to | datetime |
project_id (optional) | int | Project ID
show_dry_run (optional) | boolean | Show test payments
transfer_id (optional) | int |
report_id (optional) | int |
limit | int | Limit
offset | int | Offset
in_transfer_currency | string | Calculate in currency of transfer
show_total | string | Show Summary for CSV and XML data


# Error Codes

Error Code | Meaning
---------- | -------
404 | Not found
