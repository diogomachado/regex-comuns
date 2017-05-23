# Expressões regulares
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

## CNPJ (com ponto e traço opcional)
```
([0-9]{2}[\.][0-9]{3}[\.][0-9]{3}[\/][0-9]{4}[-][0-9]{2})
```

## CPF (com ponto e traço obrigatório)
!["Representação do regex"](https://lh3.googleusercontent.com/iKKppqlQRiUX9YsVL7UQkply7UzfyjgZ2b2bYb-HK5pwPTCe_Bgv4q3n5cZDO2nrO2xAdosYVqHCWkGSiZDpAw1pOpw3hz4LKfPHrQk0Gs0oPK8LBjKmIvsQdBYf-UGnnnYlbfyrjj7XUPC7UjR3CS6pksppcVK_Po6v5kYmLHVbBDi2HJUBFVAXJ3PZdQaynQ0cy_IibXoZx8qfQGn_HzfloB9oY7FKbC9YOPM_EmZNK7C0FDSJBN2z07ha2r-QCWrVSZrxnAbLbCZM6bMLHgwcYF4vgAPifSZu6Fb05q1DjRADWek_KZo4fO4Oz04rqxJx33wqyFPiLTXxd7ue3rG2GTbFBPcoXYMlOJUJvLHjqda_fqmaF10lsfoOCQ2GbMaOI_m2p3gnFgzBBFVUeQ293uAoz3o-EJJ5jsvYd82l_iDfIfIB3Jy0CRut-5fB19sVuvm5poHKTXZEbu5Ykwh2UmgzaBWg3ccwvYkjXhCP2ON4exQG0aNHnEIyu2Dku4UVuiz46aXkEHC8RRiKuzaq-zXHFY1JD46pDnFIi__MQfO9GwK1Vs51COxuri3Qbbl8oaY1=w1547-h761)

```
([0-9]{3}[\.][0-9]{3}[\.][0-9]{3}[-][0-9]{2})
```
