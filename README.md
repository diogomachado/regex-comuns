# regex-comuns
Um estudo de regex comuns

## E-mail
- Regex valida se é e-mail
- Valida se tem domínio
- Valida se tem subdomínio

```
[\w\.]+@[a-zA-Z_\-]+?\.[a-zA-Z]{2,}([\.a-zA-Z]?){3,4}
```

Exemplos:
- git@machado.com
- git@dmachado.com.br
- 21git@subdomio.diogomachado.com
- git21@subdomio.diogomachado.com
- git.21@subdomio.diogomachado.com
- git.21@diogo-machado.com

## Data de nascimento
- Esse regex valida o dia, indo de 01 até 31
- Valida o mês, de 01 até 12
- Valida o ano, de 1900 até o ano atual 2017

```
(0[1-9]|1[0-9]|2[0-9]|3[0-1])[/](0[1-9]|1[0-2])[/](19[0-9]{2}|20[0-7]{2})
```