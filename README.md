# Expressões regulares
Expressões regulares podem salvar sua vida!

## E-mail
- Regex valida se é e-mail
- Valida se tem domínio
- Valida se tem subdomínio

!["Representação do regex"](https://lh3.googleusercontent.com/otJOOQ8Ite509gVNByswS0DZqRWdsKesk0XpnpbTN5Wr68sarkstc2vB9l1Q8Eb3iEag2rTC9yc7hmdr-78e5v5mz5RjatwkeLKSprCOH0kgSq4odjDQ8PX15eaqnBn_39-5FzaW9qNJcz-USLL6VMvGoDWphsvAScCbTw_wlhebpxCXy9evJMWN7kdg5ArbOe6oTgbrmw9Mi_Pjefp5lzUGEtqf4_u5_h0GxHuHK4cPZ9iVPnqeewGDu-2NmsX2wZdx_4KfN4pZTs93Nja-7siK80WsYCG2zmfpqSg1fEyUaJe__d7E1EU13lMwEFBqNbqryuFL8sywUjZhX_w8Zl79K-al4PNBoWWkt0u71gLkdUgY2c5g6F6qghOpObM0lgOUT3LkFCa9-X1Qble6TBDFWEtDKB1Q7VShkInK-37u2ZvzG5ATn9uoBJVsER61iay6Wr8XLhSHhhiMqhsrjJ8gEIFkx8orQUCNnxQddNRkOiptE9UvdsKC1nW-Uv4BJKKTD9upt3Ajb8KLsPxPSt-2WCQoQHAk4FaqaEXQI2Dski1QEogTK81R-8Z1-ee15w_F-Xlp=w1547-h547)

```
[\w\.]+@[a-zA-Z_\-]+?\.[a-zA-Z]{2,}([\.a-zA-Z]?){3,4}
```

Exemplos válidos:
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

!["Representação do regex"](https://lh3.googleusercontent.com/eZZm3bYF9YXwDqtq8zDwQcePs650XFuMPYJbgOZxbuGFZJEmavwEMajKHmdxt83BbwvMCShRNx_QFzcrAIGNS6T5sIe_xZkMzLHs_WhPKcNzOz1hTfwbwNIqz_JHpkAB1GvK55qUCGG1Cr2M0BgPhRexXiJvx4u4RJyWEBvWFW5RBspKkhztHcHNE_MZ9Tsq5-7mJL0xyYhkiSiR5MZUaIz3S0t9piSZFb4ODSExPLRRYzz9hOzMMpwfIRK0NuF_wZIscCJDPwztZe6aq2xRs0q0nSosbY9lDfaOThk1QtKjmbGsCSC8Z3igi7R440cDNHLYLz_uFsn7IWbQcPT2NKfcsWcqBM5AcleDzn2c3YGmGk13omzGDUQhfjJa57DwtHtPlhMrDDzYtjvU4ktj34-NErg0Hhx046a1PNQwPrwczYBgzp2NgWKECsS__7EPTgHA9nq-vqn36CLRWtr3HuGoz_PZwGon-5VxE3QFsAyLQ7O2cceb8BNu4Fo_YB0lK2tugdRMnPpKxIy3LM_a4U3MA0wb5ZAY9oHYmTPho3G0zPbsFgyUSfnPyiUDrftgVeEN3cJx=w1547-h547)

```
(0[1-9]|1[0-9]|2[0-9]|3[0-1])[/](0[1-9]|1[0-2])[/](19[0-9]{2}|20[0-7]{2})
```

## CNPJ
!["Representação do regex"](https://lh3.googleusercontent.com/m1PaImssEIXNGpd_07R7f0kNUpBdY2MnF7iFI60KVYY0ZMls0RRizLi5rN37e36X-XU6SiEyR4BgsOXw6sv-k8zdbGzCamqJdykHCDfvhV4EMg-FFTfGMGizuezfWQWJyD1sUGHzs2bpr0Q_tx75ZIgDcB4EnzVk8gQ_6rLCVP1IZvA6hMElWuFHi0JhLecOh4zEziD4hL778r4E6zkiB8fHGtVKJvFJv0kcpuPUk00tHGMLMPGRHdnRGJ1301UTf1nyUkypXuxGTs66Kp4K9HjAqqvqwNtWCJaQ_ld1AptukAURySmxRE4lsIhQfIGyGnQ3LGkdIIRB4ZOPnAGFWtNwI3OE6UCLALnynNpLHXdmTJEjzY-pPFTiK-rT6bPCCkA35OunlxylaEiuO3p9MoBVpYgiT-t6jpw7j2VN5jHnCVFeVRA6bdFBJMfBIpBKQRWLdtuMrCNwopO0WBw_pAUdlpsK-Qlf_1Kx6auomez3XJg31oxsQ7bE3pqfoyb3tf2dnFsgJfKZtvoZ6w6YXStwH2lP6ugZ0mjoAj8UBqbqFwofIh21-nAGy8XNzvXBO35ip4Jv=w1547-h810)
```
([0-9]{2}[\.][0-9]{3}[\.][0-9]{3}[\/][0-9]{4}[-][0-9]{2})
```

## CPF
!["Representação do regex"](https://lh3.googleusercontent.com/iKKppqlQRiUX9YsVL7UQkply7UzfyjgZ2b2bYb-HK5pwPTCe_Bgv4q3n5cZDO2nrO2xAdosYVqHCWkGSiZDpAw1pOpw3hz4LKfPHrQk0Gs0oPK8LBjKmIvsQdBYf-UGnnnYlbfyrjj7XUPC7UjR3CS6pksppcVK_Po6v5kYmLHVbBDi2HJUBFVAXJ3PZdQaynQ0cy_IibXoZx8qfQGn_HzfloB9oY7FKbC9YOPM_EmZNK7C0FDSJBN2z07ha2r-QCWrVSZrxnAbLbCZM6bMLHgwcYF4vgAPifSZu6Fb05q1DjRADWek_KZo4fO4Oz04rqxJx33wqyFPiLTXxd7ue3rG2GTbFBPcoXYMlOJUJvLHjqda_fqmaF10lsfoOCQ2GbMaOI_m2p3gnFgzBBFVUeQ293uAoz3o-EJJ5jsvYd82l_iDfIfIB3Jy0CRut-5fB19sVuvm5poHKTXZEbu5Ykwh2UmgzaBWg3ccwvYkjXhCP2ON4exQG0aNHnEIyu2Dku4UVuiz46aXkEHC8RRiKuzaq-zXHFY1JD46pDnFIi__MQfO9GwK1Vs51COxuri3Qbbl8oaY1=w1547-h761)

```
([0-9]{3}[\.][0-9]{3}[\.][0-9]{3}[-][0-9]{2})
```

> **Testes**
>
> Teste as expressões no site http://www.regexpal.com/