Para este CTF é necessário utilizar o `find` com comando específicos de termos que o exercício fornece, foi utilizado o seguinte comando

`find / -user bandit7 -group bandit6 -size 33c 2>/dev/null`

**`find /`** inicia a busca no diretório raiz do servidor

**`-user bandit7`** especifica que o arquivo pertence ao usuário bandit7

**`-group bandit6`** especifica que o arquivo pertence ao grupo bandi6

**`size 33c`** especifica que o tamanho do arquivo é de 33 bytes, **c** indica o tamanho do arquivo em bytes, **k** seria em quilobytes e **m** em megabytes


**`2>dev/null`** redireciona qualquer mensagem de erro (2) para o diretório **/dev/null**, que é como um buraco negro no sistema, isso significa que todo os arquivos com mensagem de erro ou de permissão negada serão ignorados na busca. 

Abaixo tem o significado dos números que são usados antes do sinal de redirecionamento (`>`, `>>`, `<`, `<<`)

- `0`: Entrada padrão (stdin)
- `1`: Saída padrão (stdout)
- `2`: Saída de erro padrão (stderr)

Flag: z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S