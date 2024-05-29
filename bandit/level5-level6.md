utilizar o comando cd para acessar o diretório inhere

`cd inhere`

utilizar o comando ls -a para listar os arquivos do diretório

utilizar o comando file para determinar o tipo dos arquivos, geralmente os arquivos legíveis para humanos são classificados como "ASCII text" ou "UTF-8 text", para este CTF foi utilizado o seguinte comando 

`find . -type f -exec file "{}" \;`

Isso porque existem vários arquivos dentro do diretório e este comando faz o seguinte

 **`find`**: É um comando que permite buscar arquivos e diretórios
    
**`.`**: Representa o diretório atual a partir do qual o `find` deve começar a busca. 
    
**`-type f`**: É uma opção do `find` que especifica que estamos interessados apenas em arquivos regulares (não diretórios, links simbólicos, etc.).
    
**`-exec file "{}" \;`**: Esta parte do comando executa o comando `file` para cada arquivo encontrado. O `{}` é uma espécie de espaço reservado que é substituído pelo nome de cada arquivo encontrado pelo `find`. O `\;` indica o final do comando a ser executado para cada arquivo.

utilizar o comando `cat` para encontrar a flag no arquivo legível para humanos

`cat -- -file07`
sendo o -- utilizado para evitar que o hífen em -file07 seja interpretado de forma errada

Flag: lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR