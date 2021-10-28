# Atividade 5A04

Essa é uma fake api criada para a atividade 5A04 da Kenzie Academy Brasil

## Endpoints

Nesta api voce tera acesso a 4 Endpoits
<ol>
<li>Cadastro</li>
<li>Login</li>
<li>Hobies</li>
<li>Sites Favoritos</li>

</ol>

### Cadastro
O cadastro pode ser feito atravez da requisição com:

POST /register <br/>
e no corpo da requisição deve ser desta maneira:

{

	"email":"larissa@emailcom,

	"password":"123456",

	"name":"larissa",

	"age":24

}

### Login
O login pode ser feito atravez dessa requisição:

POST /login <br/>

e no corpo da requisição deve ser desta maneira :

{

	"email":"larissa@email.com",
	"password":"123456"

}
### Hobbie
Os hobbie podem ser lidos ou escritos somente pelo usuario logado, a leitura pode ser atravez da requisição:

GET /hobbie

essa requisição nao precisa de um corpo mas precisa de um token  que é obitdo quando logado:

{

    headers:
                {
                 authorization: Bearer 
                 eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNjM0NjUxMjQwLCJqdGkiOiIzNTQxMmM0NGM0NjI0ZjZhOTU3NTIzNGJlNzJiMmQ0ZSIsInVzZXJfaWQiOjE5fQ.kFFi1u2rRMG49LUeVOln18ViRtG_XioJKa2-H-ZNi3c

                }

}

ja escrita devera ser feita atravez da requisição :

POST /hobbie
essa requisição necessita de um corpo que deve ser assim :


{
	"Nickname":"Daniel",
	"hobbie_name":"Jogar online",
	"description":"Eu gosto de jogar nas horas vagas tanto no camputador ou em consoles"
	
}
e deve ter um token:


{

    headers:
                {
                 authorization: Bearer 
                 eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNjM0NjUxMjQwLCJqdGkiOiIzNTQxMmM0NGM0NjI0ZjZhOTU3NTIzNGJlNzJiMmQ0ZSIsInVzZXJfaWQiOjE5fQ.kFFi1u2rRMG49LUeVOln18ViRtG_XioJKa2-H-ZNi3c

                }

}
### Sites Favoritos

Os Sites favoritos podem ser lidos ou escritos porem a leitura pode ser feita sem a necessidade de um token ja a escrita necessita do token, a leitura pode ser feita atravez da requisição:

GET /favsites

esse requisição nao necessita de um corpo
ja a leitura pode ser feita atravez da requisição 

POST /favsites
essa requisição necessita de um corpo que deve ser assim :

{

	"nickname":"larissa",
	"name":"youtube",
	"link":"https://www.youtube.com/"
}
e deve ter um token:

{

    headers:
                {
                 authorization: Bearer 
                 eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNjM0NjUxMjQwLCJqdGkiOiIzNTQxMmM0NGM0NjI0ZjZhOTU3NTIzNGJlNzJiMmQ0ZSIsInVzZXJfaWQiOjE5fQ.kFFi1u2rRMG49LUeVOln18ViRtG_XioJKa2-H-ZNi3c

                }

}

