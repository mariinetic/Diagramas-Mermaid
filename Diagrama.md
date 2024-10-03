# Fluxograma de Avaliação de Sprint

```mermaid
graph TD;
    A["Tela de Login (Autenticação)"] --> B{"Tipo de Usuário"};
    B -->|Aluno| C["Menu Aluno"];
    B -->|Professor| D["Menu Professor"];
    
    C --> E["Avaliação de Sprint"];
    E --> E1["Avaliar todos os membros da equipe"];
    E --> E2["Verificar Sprint atual"];
    E --> E3["Limitar a uma avaliação por Sprint"];
    
    C --> F["Painel Geral"];
    F --> F1["Ver avaliações realizadas"];
    
    D --> G["Extrair Relatório"];
    G --> G1["Relatório de nota média por aluno por critério"];
    G --> G2["Relatório de nota média de grupo por Sprint"];
    
    D --> H["Gerenciar Grupos"];
    H --> H1["Carregar arquivo com informações dos grupos"];
    H --> H2["Adicionar/Remover membros dos grupos"];
    
    D --> I["Gerenciar Critérios de Avaliação"];
    I --> I1["Incluir critérios"];
    I --> I2["Alterar critérios"];
    I --> I3["Desativar critérios"];
    
    D --> J["Cadastrar Calendário de Sprints"];
    J --> J1["Definir datas das Sprints por semestre"];
    J --> J2["Associação automática da Sprint atual"];
