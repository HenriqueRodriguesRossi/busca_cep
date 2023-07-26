API busca_cep: 

Essa é uma API construída com Node.js, Express.js, Mongoose e Axios para consultar informações de CEP utilizando a API do ViaCEP.

Instalação
Certifique-se de ter o Node.js instalado em sua máquina. Em seguida, siga os passos abaixo:

Clone este repositório para o seu computador:
git clone https://github.com/seu-usuario/busca_cep.git

Acesse a pasta do projeto:
cd busca_cep

Instale as dependências:
npm install

Executando a aplicação:

Para executar a API, utilize o seguinte comando:
npm run dev

Rotas
GET /buscaCep
Essa rota permite realizar a consulta de informações de um CEP através do método GET.

Parâmetros da URL
cep (obrigatório): O CEP a ser consultado. Deve conter apenas números e ter o tamanho de 8 dígitos.

Exemplo de Requisição
GET http://localhost:8080/buscaCep?cep=01001000

Exemplo de Resposta (CEP encontrado): 

Status: 200 OK
{
  "cep": "01001-000",
  "logradouro": "Praça da Sé",
  "bairro": "Sé",
  "localidade": "São Paulo",
  "uf": "SP"
}

Exemplo de Resposta (CEP não encontrado):
Status: 404 Not Found
{
  "mensagem": "CEP não encontrado!"
}

Considerações Finais
Esta API foi desenvolvida com o intuito de realizar consultas de CEP de forma simples e rápida, utilizando as tecnologias Node.js, 
Express.js, Mongoose e Axios. Sinta-se à vontade para contribuir com melhorias e novas funcionalidades.

Agradecemos o uso da API busca_cep! Em caso de dúvidas ou sugestões, entre em contato com nossa equipe.
