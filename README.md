# client-server-api
Desafio Pós GoExpert Client-server-api

Para executar o projeto:
$ cd \client-server-api\server
$ go run main.go

$ cd \client-server-api\client
$ go run main.go

Prováveis mensagens de erro caso o ambiente não estiver configurado:

Erro: Binary was compiled with 'CGO_ENABLED=0', go-sqlite3 requires cgo to work.
Resolução: go env -w CGO_ENABLED=1

Caso não tenha instalado o compilador GCC para embutir o sqlite é necessário instala-lo:
https://jmeubank.github.io/tdm-gcc/articles/2021-05/10.3.0-release
MinGW-w64 based

Desabilite firewall ou configura firewall de saída, se não ocorrerá o erro abaixo:
ERROR could not get quotation at awesomeapi url=https://economia.awesomeapi.com.br/json/last/USD-BRL error="Get \"https://economia.awesomeapi.com.br/json/last/USD-BRL\": context deadline exceeded"
exit status 0xc000013a

