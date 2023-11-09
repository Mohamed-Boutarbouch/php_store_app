# Setting up postgres:

## Change password to Postgres user:

```sql
ALTER USER postgres WITH PASSWORD 'postgrespostgres';
```

## Connect (use) to database:

```sql
\c store
```

## Create table:

```sql
CREATE TABLE products (
    id SERIAL PRIMARY KEY,
    title VARCHAR(255) NOT NULL,
    description TEXT NOT NULL,
    price DECIMAL(10,2) NOT NULL,
    image VARCHAR(255),
    create_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

## List all tables in a database:

```sql
\dt+
```

# Run PHP server:

```bash
php -S localhost:8000 -t public/
```

# Fix:

Code fix is [link](https://gist.github.com/Mohamed-Boutarbouch/f14e82e816b7be6d12c7450bbbd08808)

# Example Test:

Code test example [link](https://gist.github.com/Mohamed-Boutarbouch/12bbe7e7b10970c4904a7238a24acd41)
