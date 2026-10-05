# API REST — Tutorial 4

CRUD com Node.js, Express e MySQL usando:

Route → Controller → Repository → MySQL

## Instalação

```bash
npm install
```

Copie `.env.example` para `.env`.

## Banco com Docker

```bash
docker compose up -d
```

Depois, execute o SQL de `database/init.sql` dentro do MySQL.

## Executar

```bash
npm run dev
```

API:
- GET /
- POST /alunos
- GET /alunos
- GET /alunos/:id
- PUT /alunos/:id
- DELETE /alunos/:id

## Exemplos

### POST /alunos

```json
{
  "nome": "Pedro",
  "curso": "ADS"
}
```

### PUT /alunos/1

```json
{
  "nome": "Pedro Silva",
  "curso": "Sistemas de Informação"
}
```

O Repository cuida do SQL/persistência. O Controller cuida de HTTP. As Routes fazem o mapeamento entre endpoint e Controller.
