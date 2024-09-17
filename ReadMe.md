Em nosso projeto utilizaremos 


1 - Abra "visual studio" e Clone esse repositório no diretório de sua preferencia

2 - Criar tabelas:
	Utilizando o banco de dados de sua preferencia use o scrit no arquivo CreateDLL.sql para criar as tabelas que
	usaremo em nosso projeto

3 - Criar uma WebApp

	3.1 Entre no portal azure e entre na aba "Serviços de Aplicativos" >> "Criar" >> "Aplicativo Web".
	
	3.2 Preencha os proximos espaçõs em branco com informações à sua escolha
		* Assinatura
		* Grupo de recursos (clique em "criar novo" caso não aja opções de outros grupos de recursos)
		* Nome
		* Região (recomenda-se a região mais proxima de sua localização presente, para esse teste uslizaremos "brazil south")
		* Plano do Linux (escolha um nome para seu plano)
		* Plano de preços (para nossa demonstração utilizamos Básico B1)

	3.3 Escolha as proximas opções obrigatóriamente
		* Publicar (escolha "codigo")
		* Pilha de runtime (.NET 8 (LTS))
	
	3.4 Clique em Avançar:Implantação
		* A "implantação continua" pode ficar desabilitada
		* A "Autenticação básica" deve ficar habilitada
	3.5 Clique no botão "Revisar + criar"

4 - baixe o perfil de publicação
	entre no seu Web App criado e clique "Baixar perfil de publicação" e salve no diretório de sua escolha

5 - Abrir o projeto no Sisual Studio
	No Visual Studio abra a aba "arquivo" >> "abrir" >>  "Projeto/Solução" e abra o projeto "ApplicationCP2.csproj"
	

6 - Realizar o deploy de sua aplicação
	* no "Gerenciador de Soluções" clique com o botão direito em "ApllicationCP2" >> "Publicar"
	* na janela "publicar" escolha a opção "importa perfil" e clique em "próximo"
	* clique em "Procurar" e abra o arquivo do perfil de publicação que foi baixado no "passo 4"
	* aguarde o carregamento e clique em publicar.

A pagina do navegador do projeto deve abrir em seguida, caso não abra realise a proxima etapa

7 - Abrir o WebApp
	No portal azure abra seu web app clique em iniciar, espere o carregamento de seu WebApp
	e clique em "Domínio Padrão"

(IMPORTANTE) o WebApp não funcionará se a variavel de ambiente não estiver habilitada em modo de desenvolvimento
caso isso aconteça siga o proximo passo 

8 - habilitando variaveis de ambiente
	No portal azure abra seu WebApp criado.
	A aba de configuração clique em "Variaveis de ambiente"
	Em "variaveis de ambiente" clique em "Adicionar" e copie e cole "Development Mode" no espaço "Nome"
	e "Development" no espaço "Valor"

9 - reinie sua WebApp
	
 




 