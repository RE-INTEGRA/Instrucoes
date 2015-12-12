#Passos para utilizar o Git

## Como mandar arquivos para nuvem.

 1. Passo para adicionar arquivos. Este comando adiciona todos os arquivos à base de dados do git.


    git add *

 2. Guarde a versão de código e escreva uma mensagem que descreva o que foi realizado.


    git commit -m "mensagem"

 3.  Enviar arquivos para nuvem


    git push

 4. insira no "Username" - Nome do usuário
 5. Insira "Password" - Insira senha.


## Trabalhar em ambiente colaborativo

No trabalho em equipa tem de se ter em atenção que o seu código pode quebrar o código do seu colega. Usando o git é possível criar ramos de desenvolvimento. Normalmente têm-se o ramo *master*, que é o ramo que tem todo o código funcional e que está em produção, e o ramo *development*, que é ramo que está em desenvolvimento, e ramos filhos de "development" em que cada membro da equipa trabalha numa funcionalidade do programa.

Os seguintes comandos ajudam no desenvolvimento em equipe.

Este comando cria um ramo chamado funcionalidade e muda a localização do git para trabalhar nele:


    git checkout -b funcionalidade

Você trabalhou no seu ramo e agora quer guardar as alteração. Use o comando commit para guardar as suas alterações, mas antes não se esqueça de adicionar os arquivos:

    git add *
    git commit -m "mensagem"

Terminou o seu trabalho e quer juntar com o ramo "master". Você terá de se mover para o ramo master e juntar com a sua funcionalidade, usando os seguintes comandos:

Move para o ramo master:

    git checkout master

Junta o ramo funcionalidade com o master:

    git merge funcionalidade

Depois do trabalho realizado, testado e funcionando, é hora de apagar o ramo em que já não trabalha:

    git branch -d funcionalidade
