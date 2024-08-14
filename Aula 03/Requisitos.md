#### Regras de Negócio
- *RN 01:* No caso de ser informado um documento, identificar se é um CPF ou CNPJ, e então se ele é válido;
- *RN 02:* No caso de ser informado um documento, o dropdown de transportadora deixa de ser opcional, e passa a ser um campo obrigatório;
- *RN 03:* No caso de ser informado o código e selecionado uma transportadora, pular etapa de identificação do emissor do código e buscar direto na transportadora informada;
- *RN 04:* No caso de ser informado apenas o código, fazer uma análise do input para identificar o possível emissor;
- *RN 05:* No caso de não ser possível identificar o emissor, solicitar ao usuário que informe a transportadora de origem do código.

#### Requisitos Funcionais
- *RF 01:* Campo de texto para informar o código de rastreio ou documento para busca (CPF / CNPJ);
- *RF 02:* Dropdown para selecionar a transportadora, funcionando como um "filtro" (opcional para código e obrigatório para documento);
- *RF 03:* Botão "Buscar" para iniciar a busca do pacote;
- *RF 04:* Ao completar a busca, abrir uma aba no navegador com a relação de movimentação do pacote.

#### Requisitos Não Funcionais
- *RNF 01:* Identificação do input do usuário, se é um documento ou um código de rastreio;
- *RNF 02:* Bloqueio da busca caso usuário informe um documento e não selecione uma transportadora;
- *RNF 03:* Identificação do emissor do código para direcionamento da busca;
- RNF 04: Se não identificar o emissor do código, solicitar ao usuário que informe a transportadora.

[< Anterior](Hipóteses)