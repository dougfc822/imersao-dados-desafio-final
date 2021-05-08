
# Desafio Final Imersão Dados
![image](https://github.com/dougfc822/imersao-dados-desafio-final/blob/main/Header.jpg?raw=true)
Photo by National Cancer Institute on Unsplash
# Projeto Final Drug Discovery Alura 2021

Autor: Douglas Chicaroni<br>
Linkedin: https://www.linkedin.com/in/douglas-chicaroni/<br>
e-mail: douglaschicaroni@gmail.com<br>
Projeto elaborado durante imersão Alura de 03/05/2021 até 07/05/2021<br>
**Última atualização feita em 08/05/2021**

# Sumário do Projeto
## Este projeto está dividido nas seguintes partes:
* Finalidade do Projeto
* Fases do Projeto
* Importação dos Dados
* Exploração da Estrutura dos Dados
* Análise dos Dados
* Preparação do Modelo de Machine Learning
* Machine Learning
* Conclusão do Projeto
* Bibliografia
* Sobre

## Finalidade do Projeto
Encontrar um modo de prever se ocorreu erro humano durante o processo de classificação do tipo de amostra no tratamento sendo ele erroneamento colocado como "controle" enquanto o mesmo deveria ser "com droga"

## Conclusão de Estrutura de Dados Experimentos
Através da análise temos a seguinte estrutura dos dados:
* id - coluna id seria a chave primária de cada teste, valor único definindo o teste em si.
* tratamento - dois tipos de grupos de tratamento, temos um grupo que foi testado com o componente e um outro grupo de controle para verificar a real eficácia do mesmo.
* tempo - neste campo estão os dados de tempo que a célula foi submetida pelo composto, neste caso temos 3 opções, 24, 48 e 72 horas.
* dose - que foi a dose a que esta célula foi submetida, temos neste caso D1 e D2, dois tipos de opções
* droga - a identificação de cada composto que foi utilizado no teste. O mesmo foi anonimizado para evitar qualquer conflito ou viés.
* g-0 ao g-771 - Os genomas estudados em cada experimento
* c-0 ao c-99 - É referente a linhagem celular e os valores são a viabilidade delas

## Conclusões da Análise de tratamento com controle e com droga
* Temos um total de 23.814 testes
* Um total de 3289 compostos sendo testados, sendo que um deles é um placebo, sendo 3288 compostos especificos e 1 para controle
* Temos um equilibrio nos testes.
* O grupo de controle possui uma proporção de 11,71 em relação ao grupo de droga, acredito que o pesquisador tenha usado isto para otimizar o experimento.
* Através da análise encontramos que o placebo é identificado como cacb2b860

## Estrutura de Dados Resultados
Tabela que apresenta os resultados dos experimentos e suas reações
* Coluna "id" - Apresenta a mesma chave primária dos dados experimentos, demostrando uma ligação com os dados relacionados ao compostos testados.<br>

Demais Colunas são apresentações de inibidores, agonistas e antagonistas que são ativados ou não durante o teste. No caso ativados é 1 e não ativado é 0.

Para se aprofundar no tema de mecanismos de ação coloco aqui um artigo<br> https://en.wikipedia.org/wiki/Mechanism_of_action#:~:text=In%20pharmacology%2C%20the%20term%20mechanism,as%20an%20enzyme%20or%20receptor.

##Conclusão

Com os dados apresentados e modelo de Regressão Logística utilizado, foi possível concluir a utilidade de um modelo de Machine Learning com a finalidade de se mitigar riscos de erros de classificação de amostras de controle.

### Notas importantes
Este projeto foi criado através de conhecimento adquirido durante 1 semana de Imersão por uma pessoa que não tinha conhecimento prévio de programação, estrutura de pesquisa e muito menos sobre biologia, leva em conta principalmente a necessidade do autor em se aprofundar no assunto podendo ter muitas falhas de interpretação e ajustes para serem feitos.

### Agradecimentos
Agradeço imensamente a equipe Alura pela oportunidade de aprender um assunto tão complexo, espero ter a oportunidade de participar em outros eventos.
