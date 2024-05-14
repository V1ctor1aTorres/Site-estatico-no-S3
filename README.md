# Hospedando um site estático no Amazon S3 com proteção de dados e ciclo de vida de dados
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)

## Hospedando um site estático:
- Criar o bucket "bucket-website".
  <img src="https://github.com/V1ctor1aTorres/Site-estatico-no-S3/blob/main/images/bucket%20criado.png">
- Desativar "Bloquear todo o acesso público".
- Habilitar a hospedagem de site estático no bucket.
  <img src="https://github.com/V1ctor1aTorres/Site-estatico-no-S3/blob/main/images/hospedagem%20de%20site%20estatico.png">
- Fazer upload dos arquivos do site para o bucket do S3.
  <img src="https://github.com/V1ctor1aTorres/Site-estatico-no-S3/blob/main/images/upload%20dos%20arquivos.png">
- Criar uma política de bucket "permissão somente leitura a usuários anônimos públicos".
  <img src="https://github.com/V1ctor1aTorres/Site-estatico-no-S3/blob/main/images/politica.png">

## Implementando um método de proteção de dados:
- Habilitar o versionamento no bucket do S3.
  <img src="https://github.com/V1ctor1aTorres/Site-estatico-no-S3/blob/main/images/versionamento%20ativado.png">
- Testar o versionamento fazendo upload dos arquivos atualizados.
  
## Implementando uma estratégia de ciclo de vida dos dados:
- Criar regras para economizar custos.
- Mover-versoes-anteriores: regra de ciclo de vida para mover as versões anteriores de todos os objetos do bucket de origem para o S3 Standard-IA após 30 dias.
- Excluir-versoes-anteriores: regra de ciclo de vida para excluir as versões anteriores dos objetos após 365 dias.
  <img src="https://github.com/V1ctor1aTorres/Site-estatico-no-S3/blob/main/images/regras%20de%20ciclo%20de%20vida.png">
  
## Site hospedado:
  <img src="https://github.com/V1ctor1aTorres/Site-estatico-no-S3/blob/main/images/site%20hospedado.png">
