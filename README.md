# Aplicação galeria de fotos

Trata-se de uma aplicação que pega as fotos que estão no firebase e mostra em formato de
card. Também é possível adicionar um novo arquivo de foto no firebase através da aplicação.


## Instalação desta Aplicação
### `npm install`

## Para rodar a aplicação
### `npm start`


## Configurando o firebase
passo 1: Acesse o firebase com login de uma conta Google
         No menu superior clique em 'Ir para o console'.

passo 2: Crie um projeto e o nomeie ex: 'reactGallery123'
         Ativar o analytics é opcional, clique em 'criar projeto'.

passo 3: Continuando... Escolha a opção 'web' em 'Adicione um app para começar'.

passo 4: Criando um app dentro do projeto no firebase:
         Escolha um nome para registrar o app, ex: 'reactGallery123'.

passo 5: Clique em registrar app, será gerado uma serie de códigos atrelada ao que já
         criamos anteriormente. Copie o trecho que contém o seguinte código:

         `const firebaseConfig = {
            apiKey: "",
            authDomain: "",
            projectId: "",
            storageBucket: "",
            messagingSenderId: "",
            appId: ""
        };`

passo 6: Altere o arquivo '.env.example' com os valores atribuidos pelo firebase 
        ao objeto 'firebaseConfig', observe que as variaveis de ambiente nao deveram possuir
        'aspas' ex: REACT_API_FIREBASE_APIKEY=XXXXXXXXXXXXXXXXXXXXX. 
        Renomeie o arquivo '.env.example' para '.env'.
        Este passo pode também ser realizado depois do passo a passo das configurações do firebase.

passo 7: No firebase clique em 'continuar no console'

passo 8: No menu lateral do firebase clique em 'storage', clique em 'primeiros passos',
         clique em 'próxima', clique em 'concluir'.

passo 9: No menu superior clique em 'rules', 'editar regras', na linha 5 do código mostrado,
         altere as regras, então a linha 5 deverá ficar assim: 'allow read, write;'.
         Obs: Nota que permitiremos leitura e escrita, em uma aplicação que ficará 
         no ar não deverá alterar este trecho.

passo 10: no menu superior clique em 'files', crie uma pasta chamada 'images', clicando
        ao lado de '...'. Se o nome da pasta não for 'images', deve não funcionar porque faz
        referência no código.

Abra [http://localhost:3000] no seu navegador.
