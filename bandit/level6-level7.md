utilizar o comando cd para acessar o diretório inhere

`cd inhere`

utilizar o comando ls -a para listar os arquivos do diretório

utilizar o comando abaixo para listar todos os arquivos dentro do diretório atual, que tenham o tamanho de 1033 bytes e que não sejam executáveis, dessa forma há um grande afunilamento que resulta no diretório e arquivo que contém a flag

`find . -type f -size 1033c ! -executable`

**`size 1033c`** especifica que o tamanho do arquivo é de 1033 bytes, **c** indica o tamanho do arquivo em bytes, **k** seria em quilobytes e **m** em megabytes

Flag: P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU