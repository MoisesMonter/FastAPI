
# Aula 001

Primeiros passos com FastApi


## Referências

- [Documentação FastAPI](https://devdocs.io/fastapi/)


## Instalação/Dependências

1. Crie Primeiamente seu ambiente virtual **python -m venv venv**
    - Rodando Windows
        ```bash 
            venv/Scripts/activate
        ```
    - Rodando Linux
        ```bash
        venv/bin/activate
        ```



2. Instale as dependências com **pip**


```bash
  $ pip install fastapi
  $ pip install "uvicorn[standard]"
```


## Rodando Projeto

Para roda o pojeto, irá usar função **uvicorn** na **main** do projeto

```bash
$  uvicorn main:app --reload
```

### Ambiente de teste

```bash
    INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
```
## Documentação da API

#### Local para ver toda Documentação


```htpp
localhost:8000/docs/
```

#### API deste projeto


```http
  GET /
```

| Key   | Value       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `hello` | `world` | ------------ |

#### Retorna um item

```http
  GET /api/item/${id}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `id`      | `int` | None |

#### add(num1, num2)

Recebe dois números e retorna a sua soma.

