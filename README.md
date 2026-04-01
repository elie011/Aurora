```markdown
# Análise de Telemetria e Lançamento de Foguetes 🚀

Este repositório contém um script em Python desenvolvido para analisar dados de telemetria de foguetes e determinar se eles estão seguros para o lançamento. O script lê um conjunto de dados, seleciona uma amostra aleatória (representando os dados de um dia/momento específico) e realiza uma série de verificações de segurança estruturais, de temperatura e de energia.

## 📋 Funcionalidades

O script avalia as seguintes condições do foguete:
- **Temperatura:** Verifica se as temperaturas internas e externas estão dentro das margens de segurança.
- **Integridade Estrutural:** Analisa os sensores de integridade do chassi do foguete.
- **Pressão do Tanque:** Confirma se a pressão dos tanques de combustível está estável.
- **Módulos Críticos:** Checa o status dos módulos principais e o link de telemetria.
- **Análise Energética:** Calcula a porcentagem de kWh usados e estima o consumo de energia necessário para a decolagem.
- **Validação de Lançamento:** Uma verificação final rigorosa que define se o foguete tem ou não permissão para decolar (Go/No-Go).

## 🛠️ Pré-requisitos

Para executar este código, você precisará do **Python 3.x** instalado em sua máquina, além da biblioteca `pandas` para manipulação de dados.

Você pode instalar as dependências necessárias executando o seguinte comando no seu terminal:

```bash
pip install pandas
```

## 📂 Estrutura de Arquivos Necessária

Para que o script funcione corretamente, é obrigatório ter o arquivo de dados de telemetria no mesmo diretório do script:


## 🚀 Como Executar

1. Clone este repositório para a sua máquina local:
   ```bash
   git clone [https://github.com/elie011/Aurora.git](https://github.com/elie011/Aurora.git)
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd seu-repositorio
   ```
3. Execute o script do arquivo "datase.ipynb" para criar o dataset `telemetry_anomalies_dataset.csv` na pasta.
4. Execute o script Python:
   ```bash
   python pre-decolagem.ipynb
   ```

## 📊 Exemplo de Saída (Output)

Ao executar o script, você verá um relatório no terminal semelhante a este:

```text
A linha 42 está sendo analisada agora, este é o dia 2023-10-25 14:30:00 
Temperaturas estão Ok
A integridade estrutural está OK
A pressão do tanque está Ok
O status dos módulos críticos estão OK
Capacidade energetica total: 150.5Kw
Porcentagem de Kwh usados: 45.23%
Consumo de energia estimado na decolagem: 120.5Kwh
Perda energetica: 2.5%
O foguete 42 está pronto para lançamento
```
