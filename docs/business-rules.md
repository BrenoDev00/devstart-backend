# DevStart - plataforma de vagas para desenvolvedores iniciantes

## Objetivo do sistema

- permitir que desenvolvedores iniciantes encontrem oportunidades de trabalho, como:
- primeiro emprego;
- estágio;
- trainee;
- vagas júnior;
- a plataforma também permite que empresas publiquem vagas voltadas para iniciantes.

## Tipos de usuários

### Candidato

- usuário que busca vagas para se candidatar.
- pode:
- criar conta;
- cadastrar perfil profissional;
- buscar vagas;
- candidatar-se a vagas;
- descandidatar-se a vagas.

### Empresa

- usuário que publica vagas.
- pode:
- criar conta;
- cadastrar perfil da empresa;
- publicar vagas;
- visualizar candidatos com base na vaga cadastrada;
- fechar vagas.

### Administrador

- usuário responsável por moderar o sistema.
- pode:
- manter usuários;
- manter empresas;
- manter vagas;
- moderar conteúdo quando for necessário.

## Regras de negócio específicas de Candidato

- o usuário pode se candidatar informando:
  nome,
  e-mail,
  senha,
  tecnologias,
  nível (podendo ser júnior, estagiário ou trainee),
  github (opcional),
  linkedin (opcional),
  disponibilidade (remoto, presencial ou híbrido),
  foto (verificar possibilidade de implementar no projeto);
- e-mail deve ser único;
- senha deve ter 6 caracteres, incluindo 1 letra maiúscula, números e 1 caractere especial;
- não pode se candidatar 2 vezes na mesma vaga.

## Regras de negócio específicas de Empresa

- a empresa pode se candidatar informando:
  nome da empresa,
  e-mail,
  senha,
  linkedin (opcional),
  descrição,
  tamanho da empresa (opcional),
  site(opcional),
  foto (verificar possibilidade de implementar no projeto);
- e-mail deve ser único;
- senha deve ter 6 caracteres, incluindo 1 letra maiúscula, números e 1 caractere especial.

## Regras de negócio sobre Vagas

- empresa pode publicar vagas com os campos:
  título da vaga,
  descrição,
  tecnologias,
  tipo de vaga (CLT ou PJ),
  nível da vaga (podendo ser júnior, estagiário ou trainee),
  disponibilidade (remoto, presencial ou híbrido) e salário (opcional);
- nenhuma vaga pode exigir experiência;
- uma vaga pode ter status: aberta (status definido por padrão), fechada e pausada;
- candidatos só podem aplicar em vagas abertas.

## Regras de negócio sobre Candidaturas

- quando um candidato aplica em uma vaga, o sistema deve salvar:
  candidato, vaga e data de candidatura;

## Regras gerais

- todos os usuários podem visualizar vagas;
- somente usuários logados podem aplicar em vagas.
