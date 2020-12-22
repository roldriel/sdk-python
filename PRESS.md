<div align="right"><font color=#4682B4 size=3>

![logo](/img/lts_logo_mini.png)
<b>Demo SDK V2 | Q4 2020 | 23/12/2020</b></font>

</div>

<div align="center">
<font color=#4169E1 size=6>

<b>PY<font color=#FF8C00>THON</font> <font color=#4682B4>+</font> <font color=#800080>RUBY</b></font></font></div>

<b>Referências</b>

- PLAYERS | ideias de implementação: Stripe e Square
- ARQUITETURA | baseada em .Net Core: Danilo Elias

>mercadopago/
>>config/
>>>config .py
`[configurações estáticas]`
>>>request_options.py
`[configurações de chamadas onde qualquer Dev pode sobrescrever chamadas e/ou módulos conforme a sua necessidade]`

>mercadopago/
>>core/
>>>mp_base.py
`[une os módulos em resources e http_client.py com regras de validação básicas para evitar erros nas chamadas criadas]`

>mercadopago/
>>http/
>>>http_client.py
`[chamadas REST]
[max_retries possui regra para o GET]`

>mercadopago/
>>resources/ 
`[a lista foi construída com base nas SDKs em PHP e Java]
[módulos para chamar as APIs]`
>>>advanced_payment.py
>>>card_token.py
>>>card .py
>>>customer .py
>>>disbursement_payment.py
>>>identification_type.py
>>>merchant_order.py
>>>payment_methods.py
>>>payment .py
>>>preference .py
>>>refund .py
>>>user .py

>mercadopago/
>>SDK

>tests
`[testes de integração]`
>>test_advanced_payment.py
>>test_card_token.py
>>test_card.py
>>test_customer.py
>>test_identification_type.py
>>test_merchant_order.py
>>test_payment_methods.py
>>test_payment.py
>>test_preference.py
>>test_user.py
>>test .py

###Pydoc
`/sdk-python/docs/mercadopago/index.html`

###GitHub Actions
>github
>>workflows
>>>mercado-pago-package.yml
`[configurado para os testes na branch de desenvolvimento refactor]`