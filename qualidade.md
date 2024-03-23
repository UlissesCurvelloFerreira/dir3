# Relatório Atividade Trainee Semana 1 - Qualidade

## Introdução
Neste relatório, abordarei algumas das dificuldades encontradas durante a construção do deploy e os problemas enfrentados. Ele será dividido em duas partes: a primeira descreverá como encontrei a documentação da atividade, e na segunda explorarei mais a fundo a questão do deploy.

## Parte 1:
Na primeira parte, recebi o projeto por e-mail. Em seguida, realizei o login no servidor. Iniciei a busca pela atividade utilizando alguns comandos básicos de terminal. Curiosamente, ou não, foi somente no último arquivo que consegui encontrar a atividade. Com a atividade encontrada, parti para o deploy do projeto.

## Parte 2:
Na segunda parte, comecei a entender o que a atividade solicitava. Logo, instalei o nginx usando o terminal, pois estou utilizando o Linux. Em seguida, precisei escolher um jogo e optei pelo 2048, pois é o que tenho mais familiaridade.

### Erros de configuração:
Com o jogo e seus arquivos baixados no meu computador, dei início à configuração do nginx. Primeiramente, movi os arquivos relacionados ao jogo para a pasta de arquivos HTML do nginx ("/var/www/html"). Como o jogo estava lá, era necessário configurar o arquivo de servidor do Nginx. Neste ponto, tive um pouco de dificuldade por não conhecer os padrões e qual porta usar para acesso HTTP. Após uma rápida pesquisa, descobri que seria a porta 80. Assim, o primeiro problema foi solucionado.

### Erros de acesso:
Com a porta configurada, meu problema agora era outro. Sabia que o server_name deveria ser "localhost", já que a aplicação deveria ser usada apenas localmente, como especificado no trabalho. A configuração do root também foi rápida de encontrar na internet, seguindo alguns tutoriais. No entanto, o principal problema foi a variável "index". Esta variável me deu um pouco de trabalho, pois eu a apontei para uma pasta acima daquela onde estava o diretório do arquivo index.html. Isso gerou alguns erros e perdi um pouco de tempo para entender como resolver tal problema. Finalmente, após alguns instantes, achei o erro e a variável foi configurada adequadamente.

Outra dificuldade foi acessar a aplicação de dispositivos móveis, mas esse erro foi rapidamente resolvido com conversas e trocas de dúvidas.

- Quando uso o comando:

Isso funciona em dispositivos móveis conectados ao mesmo IP da minha rede
- http://192.168.1.107/2048-master/
ou posso usar também
- http://localhost/2048-master/.

## Conclusão:
Durante o desenvolvimento do projeto, enfrentei alguns desafios e dificuldades. No entanto, com um pouco de pesquisa e tempo, consegui encontrar a solução adequada para cada um. Essas resoluções foram ótimas oportunidades de aprendizado e desenvolvimento das minhas habilidades.
