1 - Buscar o nome e ano dos filmes

SELECT Nome, Ano
FROM Filmes

2 - Buscar o nome e ano dos filmes, ordenados por ordem crescente pelo ano 

SELECT Nome, Ano
FROM Filmes
ORDER BY Ano ASC;

3 - Buscar pelo filme de volta para o futuro, trazendo o nome, ano e a duração

SELECT Nome, Ano, Duracao
FROM filmes
WHERE Nome = 'De Volta para o Futuro';

4 - Buscar os filmes lançados em 1997

SELECT Nome, Ano
FROM filmes
WHERE Ano = 1997;

5 - Buscar os filmes lançados APÓS o ano 2000

SELECT nome, ano
FROM filmes
WHERE ano > 2000;

6 - Buscar os filmes com a duracao maior que 100 e menor que 150, ordenando pela duracao em ordem crescente

SELECT Nome, Duracao
FROM filmes
WHERE Duracao > 100 AND Duracao < 150
ORDER BY Duracao ASC;

7 - Buscar a quantidade de filmes lançadas no ano, agrupando por ano, ordenando pela duracao em ordem decrescente

SELECT Ano, COUNT(*) AS Quantidade_filmes
FROM filmes
GROUP BY Ano
ORDER BY Quantidade_filmes DESC;

8 - Buscar os Atores do gênero masculino, retornando o PrimeiroNome, UltimoNome

SELECT PrimeiroNome, UltimoNome ,Genero
FROM atores
WHERE Genero = 'M';

9 - Buscar os Atores do gênero feminino, retornando o PrimeiroNome, UltimoNome, e ordenando pelo PrimeiroNome

SELECT PrimeiroNome, UltimoNome , Genero
FROM atores
WHERE Genero = 'F'
ORDER BY PrimeiroNome;

10 - Buscar o nome do filme e o gênero

SELECT Nome, Genero
FROM filmes
Join FilmesGenero ON IdFilme = Filmes.Id
Join Generos ON IdGenero = Generos.Id

11 - Buscar o nome do filme e o gênero do tipo "Mistério"

SELECT Nome, Genero
FROM filmes
Join FilmesGenero ON IdFilme = Filmes.Id
Join Generos ON IdGenero = Generos.Id
WHERE Generos.Genero = 'Mistério';

12 - Buscar o nome do filme e os atores, trazendo o PrimeiroNome, UltimoNome e seu Papel

SELECT Nome, PrimeiroNome, UltimoNome, Papel 
FROM filmes
Join ElencoFilme ON IdFilme = Filmes.Id
Join Atores ON IdAtor = Atores.Id
