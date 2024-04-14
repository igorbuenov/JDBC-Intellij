# JDBC-Intellij

## Passo a passo para utilizar MySQL no Intellij

### MySQL:
Antes de qualquer configuração, devemos installar o MySQL e uma interface gráfica para a utilização da mesma.
- MySQL Installer: https://dev.mysql.com/downloads/installer/
- MySQL Workbench (interface gráfica): https://dev.mysql.com/downloads/workbench/

Bônus:

- Vídeo de instalação e configuração: https://www.youtube.com/watch?v=gffMzD8IsRk&t=66s

Obs: A depender do momento que você está assistindo a esse vídeo, alguma coisa pode ter mudado, então como um bom desenvolvedor, utilize as habilidades para pesquisar por materiais mais recentes que possam te auxiliar.

### JDBC:
Com ambos instalados, chegou a hora de baixar e instalar o JDBC que é uma API padrão do JAVA que da o auxilio para a conexão com os bancos de dados, fazendo a conversão do código JAVA para o código nativo para o acesso do mesmo.

- MySQL JAVA connector: https://dev.mysql.com/downloads/connector/j/ 

Selecione a opção "Plataform Independent", baixe o arquivo ZIP e extraia para uma pasta de preferência que fique suas bibliotecas externas ou funcionalidades para JAVA, sendo assim de fácil localização.

- Abra o Intellij clique em File -> Project Structure:

![image](https://github.com/igorbuenov/JDBC-Intellij/assets/98808773/9b00bfaa-c640-4ec1-86c3-c0399897cbf4)


- Na aba lateral clique em Modules -> Dependencies:

![image](https://github.com/igorbuenov/JDBC-Intellij/assets/98808773/c39dc071-f7b7-44fc-bfb3-6091b111b3a6)


- Clique no símbolo de "+", escolha a opção "JAR or Directories" para adicionar uma nova dependencia e navegue até a pasta onde você extraiu o JDBC Connector:

![image](https://github.com/igorbuenov/JDBC-Intellij/assets/98808773/d62d1c02-f067-4060-8450-dfdbf2b0d521)


- Após selecionado, clique em ok, dê um Apply e ok novamente!

### Teste de conexão

Para fins de testes, no Workbench crie um banco com uma tabela e insira alguns dados para poder testar o retorno das informações.

![image](https://github.com/igorbuenov/JDBC-Intellij/assets/98808773/7c39c78c-a5f3-4342-bcd5-54d245c211f8)


No Intellij crie uma classe para testes e insira os códigos abaixo, lembrando de trocar os dados de conexão (url, user e password) com os seus :

![image](https://github.com/igorbuenov/JDBC-Intellij/assets/98808773/1bbb62f6-7807-46a1-94e5-0cbac7107fec)


Com a query executada o resultado retornado foi:

![image](https://github.com/igorbuenov/JDBC-Intellij/assets/98808773/484e468c-200a-487d-9382-f7cd1d2758b7)


O Intellij está pronto e configurado para trabalhar com banco de dados e MySQL no seu projeto.

### Observações finais:

Esse passo a passo foi feito para estudo próprio mas com a intenção de ajudar a todo aquele iniciante que possa encontrar um pouco de dificuldade
em alguma parte do seu estudo. Mudanças podem acontecer com o decorrer do tempo, e assim que possível será corrigido. Espero poder ter ajudado!
