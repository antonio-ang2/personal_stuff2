---
title: Inserindo dados na tabela
sidebar_position: 3
---

# <img src={require('/img/autoestudo.png').default} width='35vw'/> Setup de ferramentas de desenvolvimento


## 1. Nessa aula vamos adicionar registros na tabela com SQL

Para criar comandos na tabela criada, basta exexutar o seguinte comando sql:

```bash
use cadastro;
insert INTO pessoas(id, nome, nascimento, sexo, peso, altura, nacionalidade)
values('3' , 'antonio', '1999-01-02', 'f', '63.5', '1.62',default);
```
Nesse sentido, aqui vão algumas dicas:

- Devo colocar auto increment para não precisar informar o id, não basta apenas informar que é chave primária
- Se eu colocar as informações na ordem que são declaradas no banco, posso excluir a declaração de valores e somente enviar
- Por fim, para adicionar mais de um registro ao mesmo tempo, basta passar mais de uma linha de values - separados por vírgula até a última.



<div style={{ textAlign: 'center' }}>
    <iframe 
        style={{
            display: 'block',
            margin: 'auto',
            width: '100%',
            height: '50vh',
        }}
        src="https://www.youtube.com/embed/NCG9niOlm40?si=cd9Ui4DNQqPVSUuk"
        frameborder="0" 
        allowFullScreen>
    </iframe>
</div>

