# weather_forecast
Aplicação de Crawling em uma Página Web com Scrapy e Python 3.

* Site utilizado para extração de dados: https://www.climatempo.com.br/previsao-do-tempo/agora/cidade/558/saopaulo-sp


## Criando Ambiente Virtual para depedências.
-- Criando Ambiente: py -m venv weather_forecast_venv.   
-- Ativando Ambiente: .\weather_forecast_venv\scripts\activate.

### Instalando Depedências.
-- Instalando o scrapy: pip install scrapy.

#### Criando Configurações do Gerenciador de depedências.
-- Criando arquivo de configurações: pip freeze > requirements.txt	

#### Criando Estruturas de dados.
Mongodb
db.weather.insert(
{
    id: "", 
    cidade: "",
    temperatura: "",
    previsao: "",
    sensacao: "",
    umidade: "",
    pressao: "",
    vento:  "",
    horario: ""
}

PostgreSQL ou outro BD Relacional SQL.

CREATE TABLE [IF NOT EXISTS] weather (
    weather_id int serial PRIMARY KEY,
	cidade VARCHAR ( 100 ) UNIQUE NOT NULL,
    temperatura VARCHAR ( 4 ) UNIQUE NOT NULL,
    previsao VARCHAR ( 30) UNIQUE NOT NULL,
    sensacao VARCHAR ( 4 ) UNIQUE NOT NULL,
    umidade VARCHAR ( 4 ) UNIQUE NOT NULL,
    pressao VARCHAR ( 10 ) UNIQUE NOT NULL,
    vento VARCHAR ( 10 ) UNIQUE NOT NULL,
	horario_created_on TIMESTAMP NOT NULL,
    
);







