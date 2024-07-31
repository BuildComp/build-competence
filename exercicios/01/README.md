# Exercício: Programa Gerador de Ingressos

Crie um programa gerador de ingressos que atenda aos seguintes requisitos:

1. **Geração de Ingressos Únicos**: Cada ingresso deve ser único e conter letras e números, totalizando 30 caracteres.
2. **Quantidade Definida de Ingressos**: O programa deve gerar uma quantidade definida de ingressos (por exemplo, 150 ingressos).
3. **Consumo de Ingressos**: Os ingressos gerados serão consumidos pelos usuários, e o programa deve atualizar o estoque de ingressos de acordo com o consumo.
4. **Reabastecimento de Estoque**: Quando o número de ingressos restantes atingir um valor mínimo (por exemplo, 100 ingressos), o programa deve repor o estoque de ingressos para garantir que sempre haja ingressos disponíveis.
5. **Delay na Reposição**: Quando repor os ingressos, o programa deve gerar novos ingressos com um delay de 10ms entre cada geração.

### Exemplo:
Se 61 pessoas consumirem ingressos, sobrariam 89 ingressos. Nesse caso, o programa deve repor os ingressos para garantir que haja pelo menos 100 ingressos disponíveis.

### Como você implementaria esse programa?

### Requisitos Mínimos para Solução em Java:

1. **Classe `Ingresso`**:
    - **Propriedades**: código único (String de 30 caracteres).
    - **Método** para gerar um código único (letras e números).

2. **Classe `GeradorDeIngressos`**:
    - **Propriedades**: lista de ingressos, quantidade mínima e máxima de ingressos.
    - **Método** para gerar uma quantidade definida de ingressos.
    - **Método** para verificar e repor o estoque de ingressos.
    - **Método** para consumir ingressos.

3. **Função Principal (`main`)**:
    - Inicialização do gerador de ingressos com a quantidade definida.
    - Simulação do consumo de ingressos por usuários.
    - Verificação e reposição de ingressos quando necessário.
    - Utilização de `Thread.sleep` para implementar o delay de 10ms na geração dos ingressos durante a reposição.