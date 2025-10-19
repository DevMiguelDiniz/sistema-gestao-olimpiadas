# Sistema de Gestão de Olimpíadas

## Descrição do Projeto

Com a chegada das Olimpíadas, um novo sistema de gestão é necessário para coordenar os diferentes aspectos do evento. Este sistema deve permitir o gerenciamento de competições, inscrições de atletas, alocação de locais para as provas, e controle de resultados.

## Funcionalidades Principais

### 1. Cadastro de Competições
- O sistema permite o cadastro de competições, incluindo:
  - Nome da modalidade
  - Data e horário
  - Local de realização
  - Lista de atletas inscritos

### 2. Inscrição de Atletas
- Atletas de diferentes países podem se inscrever em competições específicas
- Cada atleta pode participar de várias competições
- Um atleta só pode representar um país por modalidade

### 3. Alocação de Locais
- Os locais para as competições são alocados evitando conflitos de horário
- Um local só pode abrigar uma competição por vez

### 4. Controle de Resultados
- Após a realização das competições, os resultados são registrados
- Sistema determina o atleta vencedor e os classificados em segundo e terceiro lugares

### 5. Relatórios de Medalhas
- O sistema gera relatórios de medalhas por país
- Mostra o desempenho baseado nas medalhas de ouro, prata e bronze conquistadas

## Arquitetura do Sistema

### Diagrama de Casos de Uso
Este diagrama ilustra as principais interações entre os usuários do sistema e as funcionalidades disponíveis.

![Diagrama de Casos de Uso](imagens/diagrama-de-casos-de-uso.jpeg)

### Diagrama de Classes e Pacotes
Este diagrama apresenta a estrutura interna do sistema, mostrando as classes, pacotes e seus relacionamentos.

![Diagrama de Classes e Pacotes](imagens/diagrama-de-classes-e-pacotes.png)

### Diagrama de Componentes
Este diagrama mostra a arquitetura de componentes do sistema e como eles se relacionam.

![Diagrama de Componentes](imagens/diagrama-de-componentes.jpeg)

### Diagrama de Implantação
Este diagrama representa como o sistema será implantado em ambiente de produção.

![Diagrama de Implantação](imagens/diagrama-de-implantação.png)

## Estrutura de Pacotes

O sistema está organizado nos seguintes pacotes principais:

- **Controller**: Responsável pela camada de apresentação e controle das requisições
- **Service**: Contém a lógica de negócio do sistema
- **Repository**: Interface para acesso aos dados
- **Model**: Entidades do domínio
- **DTO**: Objetos de transferência de dados

## Entidades Principais

### Competição
- Representa uma modalidade esportiva específica
- Contém informações sobre data, horário, local e atletas inscritos

### Atleta
- Representa um competidor
- Possui nome e país de origem

### País
- Representa as nações participantes
- Contém nome e código do país

### Local
- Representa os locais onde as competições ocorrem
- Possui nome e capacidade

### Resultado
- Registra os resultados de uma competição
- Define atletas vencedores (ouro, prata, bronze)

## Regras de Negócio

1. **Cadastro de competições**: Sistema deve permitir cadastro completo com validações de data e local
2. **Inscrição de atletas**: Validação de que cada atleta representa apenas um país por modalidade
3. **Alocação de locais**: Prevenção de conflitos de horário entre competições
4. **Controle de resultados**: Registro obrigatório de posições dos atletas
5. **Relatórios de medalhas**: Geração automática de estatísticas por país

## Tecnologias Utilizadas

- **PlantUML**: Para modelagem dos diagramas
- **Arquitetura em Camadas**: Separação clara de responsabilidades
- **LucidChart**: Para modelagem do diagrama de implantação 

## Contribuição

Este projeto foi desenvolvido como parte de um trabalho acadêmico sobre modelagem de sistemas. Para contribuições, entre em contato com os desenvolvedores.

## Licença

Este projeto está sob licença acadêmica. Consulte o arquivo de licença para mais detalhes.

---

**Desenvolvido para o Sistema de Gestão de Olimpíadas**