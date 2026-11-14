# SQL_BANCO_DE_DADOS_CENSO
CREATE DATABASE censo; 
 USE censo; 

 CREATE TABLE censo ( 
    regiao VARCHAR(20) NOT NULL, 
    estado VARCHAR(30) PRIMARY KEY,
    populacao Numeric(10) NOT NULL 
); 

INSERT INTO censo (regiao, estado, populacao) VALUES ('Sul', 'Paraná', 11835379); 
INSERT INTO censo (regiao, estado, populacao) VALUES ('Sul', 'Santa Catarina', 7762154); 
INSERT INTO censo (regiao, estado, populacao) VALUES ('Sul', 'Rio Grande do Sul', 11088065);
INSERT INTO censo (regiao, estado, populacao) VALUES ('Centro-Oeste', 'Mato Grosso do Sul', 2833742); 
INSERT INTO censo (regiao, estado, populacao) VALUES ('Centro-Oeste', 'Mato Grosso', 3784239); 
INSERT INTO censo (regiao, estado, populacao) VALUES ('Centro-Oeste', 'Goiás', 6950976); 
INSERT INTO censo (regiao, estado, populacao) VALUES ('Centro-Oeste', 'Distrito Federal', 2923369); 
SELECT * FROM dual; 

SELECT * FROM censo 
WHERE regiao = 'Sul'; 

SELECT * FROM censo 
WHERE regiao = 'Centro-Oeste' 
ORDER BY estado ASC; 

SELECT * FROM censo 
WHERE estado LIKE '%Sul%'; 

SELECT * FROM censo 
WHERE populacao > 5000000; 
