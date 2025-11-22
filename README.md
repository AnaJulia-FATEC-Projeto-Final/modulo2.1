# Projeto Final de Programação Multiplataforma - Módulo 2.1 - Gateway

> Projeto desenvolvido por Ana Julia Lima de Oliveira como uma API Gateway.

> Esta aplicação faz parte do módulo 2 do projeto de Programação Multiplataforma da FATEC.
> Atua em conjunto com o Login desenvolvido no módulo 2.2.

---

## Como iniciar o projeto localmente

### 1. Git clone
```bash
git clone https://github.com/AnaJulia-FATEC-Projeto-Final/modulo2.1.git

cd modulo2.1
````

> Antes de construir os containers, certifique-se de ter a imagem do Módulo 1, deste Módulo 2.1 e do Módulo 2.2 construídas localmente no seu Docker!

### 2. Construir containers e Rodar via IDE (recomendado)
```bash
docker-compose up -d

# Abra a IDE (IntelliJ recomendado) e importe o projeto
```

### 3. Você também pode rodar via Docker:
```bash
mvn clean package -DskipTests

docker build -t anajulia/modulo2.1:latest .

# Descomente a última seção do docker-compose.yml para rodar via Docker Compose
docker-compose up -d
```

> A API Gateway fica na porta 8080 do Localhost.
