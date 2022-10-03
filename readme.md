//Comando para gerar chave ssh
~ eval "$(ssh-agent -s)"

//Comando para consultar chave ssh
~ cat ./.ssh/id_rsa.pub

//Se você criou sua chave com um nome diferente ou se estiver adicionando uma chave existente que tenha outro nome, substitua id_ed25519 no comando //pelo nome do arquivo de chave privada.
~ ssh-add ~/.ssh/id_rsa.pub

//Comando para criar um arquivo readme com o conteúdo que está entre aspas
~ echo "# andersoncpinheiro" >> README.md

//Comando para criar o repositório local
~ git init

//Comando para subir para antes do commit
~ git add README.md

//Comando para comitar com observação entre aspas
~ git commit -m "first commit"

//Comando para ver o repositório remoto
~ git remote -v

//Comando para criar uma branch Main
~ git branch -M main

//Comando para criar conexão entre o repositório local e o remoto via ssh
~ git remote add origin git@github.com:andersoncpinheiro/andersoncpinheiro.git

//Comando para enviar as alterações para o respositório remoto
~ git push -u origin main

Criar respositório via linha de comando
echo "# criarconexoesgit" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:andersoncpinheiro/criarconexoesgit.git
git push -u origin main
