---
title: Alterar estrutura de uma tabela
sidebar_position: 4
---
import Admonition from '@theme/Admonition';

# <img src={require('/img/autoestudo.png').default} width='35vw'/> Alterando a estrutura de uma tabela


## 1.1 ADICIONANDO ATRIBUTAS A UMA TABELA
A tabela criada nas aulas anteiores foi pensada para um sistema específico. Porém, imagine que essa estrutura precise mudar. Por exemplo, você precise adicionar a profissão do usuário nessa tabela. Você pode fazer isso com esse comando:

```bash
use cadastro;
alter table nome_da_tabela
add column nome_atributo varchar(10);
```

Com esse comando, o atributo profissao foi adicionado à tabela cadastro. Além disso, a fim de adicionar essa coluna em uma posição específica, você pode ultizar o camando AFTER NOME_DA_COLUNA. Da mesma forma, se quiser que o atributo seja o primeiro, basta colocar FIRST.

Por outro lado, se o caso for exlusão de uma coluna, posso fazer usando o seguinte comando:

```bash
use cadastro;
alter table nome_da_tabela
drop column nome_do_campo;
```

## 1.2 ALTERANDO PROPRIEDADE DO CAMPO

Vamos supor, por exemplo, que você queira alterar o tipo de um atributo contido na sua tabela, você pode fazer isso por meio do comando:

```bash
use cadastro;
alter table noema_da_tabela
modify column nome_da_coluna atributo_a_ser_alterado;
```
Com esse comando, pode-se mudar constrainsts e propriedades do campo, mas não seu nome.

## 1.3 RENOMEANDO CAMPO
Para renomear um campo de uma tabela, use o comando:
```bash
use database;
alter table noema_da_tabela
change column nome_da_coluna_antiga nome_novo_coluna;
```
Um porém, deve-se usar o change e reforçar todas as propriedades da coluna, se não, se perdem.

## RENOMEANDO TABELA
```bash
use database;
alter table noema_da_tabela
rename to nome_novo_tabela;
```





<Admonition 
    type="info" 
    icon=<img src={require('/img/autoestudo.png').default} width='20vw' />
    title="Autoestudo">
    <div style={{ textAlign: 'center' }}>
    <iframe 
        style={{
            display: 'block',
            margin: 'auto',
            width: '100%',
            height: '50vh',
        }}
        src="https://www.youtube.com/embed/To9qUcEMuY0?si=40_lsTh0ny3Exajn" 
        frameborder="0" 
        allowFullScreen>
    </iframe>
</div>
</Admonition>
