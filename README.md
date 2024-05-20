create database universidadedb; use universidadedb;

CREATE TABLE cursos ( id INTEGER PRIMARY KEY AUTO_INCREMENT, nome VARCHAR(100) );

INSERT INTO cursos (nome) VALUES ('Matemática'), ('História'), ('Biologia'), ('Literatura'), ('Física'), ('Química'), ('Geografia'), ('Inglês'), ('Artes');

CREATE TABLE alunos ( RA INTEGER PRIMARY KEY AUTO_INCREMENT, nome VARCHAR(60), sobrenome VARCHAR(60), curso aluno INTEGER, universidade INTEGER 

);




INSERT INTO alunos (nome, sobrenome, curso aluno, universidade) VALUES ('João ', 'silva', 1, 1),

('Maria ', 'ferreira', 2, 2),

('Vinicius', 'santos silva', 3, 3),

('Ana', 'laura', 4, 4),

('Carlos', 'pontes', 5, 5),

('Luana', 'pereira', 6, 6),

('Mariana', 'Camargo', 7, 2),

('José', 'santos', 8, 1),

('Andreia', 'lima', 9, 3);



INSERT INTO professor (nome, email, curso professor, universidade) VALUES ('Carlos Oliveira', 'carlos@gmail.com', 1, 2),

('Bruno Rodrigues', 'Bruno01@gmail.com', 2, 3),

('Pedro Xavier', 'pedroxavi@gmail.com', 3, 4),

('Mariana Camargo', 'marianaC@gmail.com', 4, 5),

('Luana Gonçalves', 'luanagonçaves@gmail.com', 5, 6),

('José De Oliveira', 'joseoliveira@gmail.com', 6, 3),

('Amanda Leite', 'amandaL2003@gmail.com', 7, 4),

('Francielly Acosta', 'Francielly.acosta02@gmail.com', 8, 5),

('Rafael Santos', 'rafael@gmail.com', 9, 2),

('Daniel Ohata', 'Daniel.ohata@facens.com', 1, 1);



CREATE TABLE universidade ( id INTEGER PRIMARY KEY AUTO_INCREMENT, nome VARCHAR(100), endereco VARCHAR(255)
);

INSERT INTO universidade (nome, endereco) VALUES ('FACENS', 'Rodovia Senador José Ermírio de Moraes, 1425 - Alto da Boa Vista, Sorocaba, SP'),

('Universidade Federal do Rio de Janeiro', 'Av. Pedro Calmon, 550 - Cidade Universitária, Rio de Janeiro, RJ'),

('Universidade de São Paulo', 'Av. Prof. Mello Moraes, 65 - Butantã, São Paulo, SP'),

('Universidade Federal de Minas Gerais', 'Av. Antônio Carlos, 6627 - Pampulha, Belo Horizonte, MG'),

('Universidade Estadual de Campinas', 'Av. Érico Veríssimo, 2500 - Cidade Universitária, Campinas, SP'),

('Universidade Federal do Rio Grande do Sul', 'Av. Paulo Gama, 110 - Farroupilha, Porto Alegre, RS');

create table EmailsAlunos( id int primary key auto_increment, email varchar(255) );

DELIMITER //


CREATE PROCEDURE criar_email_aluno(IN nomeprocedure VARCHAR(100),IN sobreprocedure varchar(100),IN uniprocedure varchar(100)) BEGIN DECLARE email1 VARCHAR(255);

END; //

DELIMITER ;

call criar_email_aluno('Viniciues','santos silva','FACENS'); select * from EmailsAlunos;
