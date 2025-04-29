### **Objetivo**

Este sistema foi desenvolvido para automatizar o cálculo de folha de pagamento, permitindo o processamento de salários líquidos com base em horas trabalhadas, horas extras, atrasos, descontos (INSS, FGTS, vale alimentação/refeição) e bonificações. Inicialmente implementado em **C**, o código foi posteriormente convertido para **Python** para facilitar sua execução em diferentes ambientes.

### **Funcionamento**

O programa realiza os seguintes cálculos e operações:

1. **Entrada de Dados:**
    - Salário base.
    - Horas e minutos trabalhados.
    - Horas e minutos de atraso.
    - Horas e minutos extras.
    - Taxa de adicional de horas extras (entre 50% e 100%).
    - Alíquota do INSS (%).
    - Bonificação (opcional).
    - Verificação de benefício de vale alimentação/refeição (VA/VR) e cálculo do desconto (20% do valor).
2. **Cálculos Realizados:**
    - **Valor da hora trabalhada:** **`Salário / Horas trabalhadas`**.
    - **Valor das horas extras:** **`(Horas extras × Valor da hora) + Adicional (taxa definida)`**.
    - **Desconto por atrasos:** **`Valor da hora × Tempo de atraso`**.
    - **Desconto do INSS:** **`Salário × Alíquota do INSS`**.
    - **FGTS (8% do salário):** **`Salário × 0.08`**.
    - **Desconto MAX de VA/VR (se aplicável):** **`20% do valor do benefício`**.
    - **Salário líquido:** CopyDownload
        
        ```
        (Salário + Horas extras + Bonificação) - (INSS + Atrasos + VA/VR)
        ```
        
3. **Saída de Resultados:**
    - Exibe detalhadamente:
        - Valor da hora trabalhada.
        - Acréscimos (horas extras e bonificação).
        - Descontos (atrasos, INSS, FGTS, VA/VR).
        - Salário líquido final.
4. **Repetição do Processo:**
    - Permite que o usuário realize novos cálculos sem reiniciar o programa.

### **Características Técnicas**

- **Linguagem Original:** C (posteriormente convertido para Python).
- **Interatividade:** Interface de linha de comando (CLI) com entrada e saída de dados.
- **Validação de Dados:** Garante que a taxa de horas extras esteja entre 50% e 100%.
- **Flexibilidade:** Aceita ajustes como bonificações e benefícios opcionais (VA/VR).

### **Aplicação**

Ideal para pequenas empresas ou departamentos de RH que necessitam de um sistema simples e eficiente para cálculos de folha de pagamento, garantindo precisão nos descontos e facilidade de uso.

(Segue anexo código em C, ZIP e modo de uso)
