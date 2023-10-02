 aula_css
primeira aula de css

#!/bin/bash

sudo apt update
sudo apt upgrade -y

sudo apt install openjdk-17-jre -y

DIR_PC="./Documents"
GIT_URL="https://github.com/icaro-bezerra/teste-shell.git"
JAR="nome-do-seu-arquivo.jar"


git clone "$GIT_URL" "$DIR_PC"

if [ $? -eq 0 ]; then
    echo "Repositório Git clonado com sucesso."

    cd "$DIR_PC"

   # java -jar "$JAR"
    cat a.txt
else
    echo "Falha ao clonar o repositório Git."
    exit 1
fi

