# Desafio it'labs!

Desafio it'labs



# Configurar start

Ao clonar o Projeto crie um banco com o nome  **test**.
Abaixo o arquivo de configuração application.properties
> spring.datasource.url=jdbc:mysql://localhost:3306/test?useTimezone=true&serverTimezone=UTC
spring.datasource.username=root
spring.datasource.password=
spring.jpa.hibernate.ddl-auto=update

## End Point
Projeto pode ser importado para a IDE própria Spring Tool Suite. 

**Listar Todos Candidatos**
> GET /candidato/ HTTP/1.1
Host: localhost:8080

**Buscar Candidato por ID**
> GET /candidato/1 HTTP/1.1
Host: localhost:8080/

**Salvar Candidato**
> POST /candidato/save HTTP/1.1
Host: localhost:8080
Content-Type: application/json
{"nome":"Candidato 2", "idPesquisa": 2, "idCargo":2}

**Atualizar Candidato**
> PUT /candidato/2 HTTP/1.1
Host: localhost:8080
Content-Type: application/json
{
    "id": 1,
    "nome": "Candidato Atualizado",
    "idPesquisa": 1,
    "idCargo": 1
}


**Deletar Candidato**
> DELETE /candidato/1 HTTP/1.1
Host: localhost:8080


**Listar Todos Cargos**
> GET /cargo/ HTTP/1.1
Host: localhost:8080

**Buscar Cargo por ID**
> GET /cargo/1 HTTP/1.1
Host: localhost:8080/

**Salvar Cargo**
> POST /cargo/save HTTP/1.1
Host: localhost:8080
Content-Type: application/json
{"nome":"Diretor"}

**Atualizar Cargo**
> PUT /cargo/1 HTTP/1.1
Host: localhost:8080
Content-Type: application/json
{"id":1,"nome":"Diretor 1"}


**Deletar Cargo**
> DELETE /cargo/1 HTTP/1.1
Host: localhost:8080



