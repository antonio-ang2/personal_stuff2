---
title: Curso MYSQL
sidebar_position: 1
---

# <img src={require('/img/autoestudo.png').default} width='35vw'/> Origem e definição de banco de dados

## 1. Origem de banco de dados

Um banco de dados é um sistema organizado para armazenar, gerenciar e recuperar informações de forma eficiente. Ele é composto por uma coleção estruturada de dados, geralmente organizados em tabelas, que podem ser facilmente acessados, gerenciados e atualizados. Os bancos de dados são amplamente utilizados em diferentes áreas, desde aplicativos empresariais até sites e sistemas de gerenciamento de conteúdo. Eles oferecem uma maneira eficaz de armazenar grandes volumes de dados e facilitam a realização de consultas complexas para recuperar informações específicas quando necessário.


Um banco de dados é um sistema organizado para coletar, armazenar e gerenciar dados de forma estruturada, permitindo acesso rápido e eficiente, além de garantir integridade e segurança dos dados. 

A história dos bancos de dados remonta ao surgimento dos primeiros sistemas de computação na década de 1960. Nessa época, os dados eram armazenados em arquivos simples e o acesso a eles era limitado. Com o aumento da complexidade das aplicações e a necessidade de gerenciar grandes volumes de dados, surgiram os primeiros sistemas de gerenciamento de banco de dados (SGBDs). O modelo relacional, proposto por Edgar F. Codd em 1970, foi um marco importante no desenvolvimento de SGBDs modernos.

O gerenciamento de um banco de dados envolve várias atividades, incluindo:

1. **Modelagem de dados:** Definir a estrutura dos dados a serem armazenados no banco de dados, incluindo tabelas, campos e relacionamentos.

2. **Projeto do banco de dados:** Projetar o esquema físico e lógico do banco de dados com base nos requisitos da aplicação.

3. **Implementação:** Criar o banco de dados e carregar os dados iniciais, utilizando linguagens como SQL (Structured Query Language) para definir esquemas, tabelas, índices, etc.

4. **Administração:** Monitorar e manter o desempenho do banco de dados, realizar backups e recuperação de dados, gerenciar usuários e permissões de acesso, entre outras tarefas.

5. **Otimização de desempenho:** Identificar e resolver problemas de desempenho, como consultas lentas, índices ausentes ou mal projetados, e ajustar a configuração do banco de dados conforme necessário.

6. **Segurança:** Implementar medidas de segurança para proteger os dados contra acesso não autorizado, como criptografia, controle de acesso baseado em papéis e auditoria de atividades.

Existem vários tipos de bancos de dados, incluindo bancos de dados relacionais (como MySQL, PostgreSQL, Oracle), bancos de dados NoSQL (como MongoDB, Cassandra), bancos de dados de grafos (como Neo4j) e outros. Cada tipo tem suas próprias características e é adequado para diferentes tipos de aplicações e necessidades de negócios.

O que é SQL?
- SQL stands for Structured Query Language
- SQL lets you access and manipulate databases
- SQL became a standard of the American National Standards Institute (ANSI) in 1986, and of the International Organization for Standardization (ISO) in 1987

# <img src={require('/img/propriedades_db.png').default} width='35vw'/> Configurações do ROS

![](/img/ros2_overlay.webp)

<div style={{ textAlign: 'center' }}>
    <iframe 
        style={{
            display: 'block',
            margin: 'auto',
            width: '100%',
            height: '50vh',
        }}
        src="https://www.youtube.com/embed/Ofktsne-utM?si=tUN7rvlnIIgbyVtD"
        frameborder="0" 
        allowFullScreen>
    </iframe>
</div>


Assim como no vídeo, citado no vídeo, o foco do curso será a linguagem de  exploração, Structured Query Language. Consiste em uma linguagem de consulta, dar comandos e esperar o retorno de uma solicitação. A ideia era se ter uma linguagem SQL só, mas as empresas adequaram a linguagem para seu próprio contexto, surgindo uma para cada empresa.



Um banco de dados é uma coleção organizada de informações - ou dados - estruturadas, normalmente armazenadas eletronicamente em um sistema de computador. Um banco de dados é geralmente controlado por um sistema de gerenciamento de banco de dados (DBMS). Juntos, os dados e o DBMS, juntamente com os aplicativos associados a eles, são chamados de sistema de banco de dados, geralmente abreviados para apenas banco de dados.

Os dados nos tipos mais comuns de bancos de dados em operação atualmente são modelados em linhas e colunas em uma série de tabelas para tornar o processamento e a consulta de dados eficientes. Os dados podem ser facilmente acessados, gerenciados, modificados, atualizados, controlados e organizados. A maioria dos bancos de dados usa a linguagem de consulta estruturada (SQL) para escrever e consultar dados.


SQL é uma linguagem de programação usada por quase todos os bancos de dados relacionais para consultar, manipular e definir dados e fornecer controle de acesso. O SQL foi desenvolvido pela primeira vez na IBM nos anos 1970, com a Oracle como principal contribuinte, o que levou à implementação do padrão SQL ANSI; o SQL estimulou muitas extensões de empresas como IBM, Oracle e Microsoft. Embora o SQL ainda seja amplamente usado hoje em dia, novas linguagens de programação estão começando a aparecer.


A foto é o dado, enquanto a galeria do seu celular onde a foto ficou armazenada é o banco de dados.

Banco de dados é um um local onde dados são armazenados e gerenciados. A palavra “relacional” significa que os dados armazenados estão organizados em tabelas.