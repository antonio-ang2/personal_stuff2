---
title: Meu primeiro banco de dados
sidebar_position: 2
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# <img src={require('/img/autoestudo.png').default} width='35vw'/> Meu primeiro banco de dados

## 1. MEU PRIMEIRO DB



## 2. TIPOS PRIMITIVOS SQL
No MySQL, os tipos de dados primitivos mais comuns incluem:

1. **INTEGER**: Armazena números inteiros, geralmente com tamanho fixo, como INT, TINYINT, SMALLINT, MEDIUMINT, BIGINT.
2. **FLOAT**: Armazena números de ponto flutuante com precisão simples.
3. **DOUBLE**: Armazena números de ponto flutuante com precisão dupla.
4. **DECIMAL**: Armazena números decimais de ponto fixo.
5. **CHAR**: Armazena strings de tamanho fixo.
6. **VARCHAR**: Armazena strings de tamanho variável.
7. **DATE**: Armazena datas no formato 'YYYY-MM-DD'.
8. **TIME**: Armazena horas no formato 'HH:MM:SS'.
9. **DATETIME**: Armazena datas e horas no formato 'YYYY-MM-DD HH:MM:SS'.
10. **TIMESTAMP**: Armazena datas e horas, mas é convertido do fuso horário atual para o UTC para armazenamento e convertido de volta para o fuso horário atual quando recuperado.
11. **BOOLEAN**: Armazena valores de verdadeiro ou falso, geralmente representados como 0 (falso) ou 1 (verdadeiro).

Esses são os tipos de dados primitivos básicos no MySQL, mas existem variações e tipos adicionais que podem ser usados dependendo das necessidades específicas de um banco de dados. Nesse sentido, ao modelar um banco de dados, o tamanho dos valores que eu almejo guardar devem ser levados em conta.

## 3. PRIMEIROS COMANDOS SQL

Para interagir com a linguagem SQL e vê-la funcionando, basta abrir alguma interface que execute essa linguagem, mysql wrkbench por exemplo e usar alguns comandos.

- CRIAR DATABASE:
```bash
CREATE DATABASE NOME DA DATABASE
```

- CRIAR TABELA: Porém, para esse comando, deve-se escolher a database que irei utilizar, isso pode ser feito com o comando Use.
```bash
USE NOME DA DATABASE;
CREATE TABLE NOME DA TABELA(
    ATRIBUTO1 TIPAGEM(),
    ATRIBUTO2 TIPAGEM(),
    ATRIBUTO3 TIPAGEM(),
);
```


## 4. Melhorando a Estrutura do Banco de Dados
Para melhor consulta dentro de um banco de dados e otimização do poder computacional, deve-se levar em conta a forma de construção do mesmo, a fim de que esse seja o mais otimizado possível. Dessa forma, vamos melhorar o que foi aprendido na última aula da seguinte forma:

Criando tabelas com algumas regras chamadas de constraints.

```bash
create database cadastro
default character set utf8
default collate utf8_general_ci;
```
Dessa forma, a database será criada com base na linguagem portuguesa, levando em conta suas acentuações e afins.


Agora, a fim de criar uma tabela bem otimizada quanto aos tipos, devemos fazer a seguinte declaração de tipagem:
```bash
create table pessoas(
	id int primary key,
	nome varchar(30) not null,
    nascimento date,
    sexo enum('m', 'f'),
    peso decimal(5,2), 
    altura decimal(3,2),
    nacionalidade varchar(20) default 'brasileiro'
)default charset = utf8;
```
Como pode ser visto, além disso, entra aqui o índice, responsável por gerar a indexação dentro da database e melhora das consultas.


Use este comando quando quiser visualizar uma tabela específica
```bash
describe pessoas;
```

O comando describer pode ser escrito como desc; 

Use para quando quiser excluir uma database.

```bash
DROP DATABASE cadastro;
```

## 5. Meu primeiro banco de dados

<div style={{ textAlign: 'center' }}>
    <iframe 
        style={{
            display: 'block',
            margin: 'auto',
            width: '100%',
            height: '50vh',
        }}
        src="https://www.youtube.com/embed/m9YPlX0fcJk?si=17hLuJntWoxg8pAh" 
        frameborder="0" 
        allowFullScreen>
    </iframe>
</div>

## 6. Melhorando a Estrutura do Banco de Dados
<div style={{ textAlign: 'center' }}>
    <iframe 
        style={{
            display: 'block',
            margin: 'auto',
            width: '100%',
            height: '50vh',
        }}
        src="https://www.youtube.com/embed/cHLKtALWDos?si=n4J7RINoBvpDflQ0" 
        frameborder="0" 
        allowFullScreen>
    </iframe>
</div>


