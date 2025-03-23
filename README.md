<h1 align="center"> Generative Pre-Trained Transformers - Trabalho Final </h1> <br>

Este projeto utiliza o framework Unsloth para realizar *Continual Pretraining* (CPT) em modelos de linguagem, adaptando-os a dados específicos, como os de comunidades extremistas. A técnica de Low-Rank Adaptation (LoRA) é aplicada para ajustar eficientemente modelos de grande escala, como Mistral e Llama, utilizando memória da GPU de forma otimizada.

O objetivo é explorar como modelos pré-treinados podem ser adaptados a domínios específicos, com foco na análise de viés e manipulação de dados sensíveis, enquanto mantém a eficiência computacional.

## Tecnologias 
* **Pandas** para pré-processamentos dados de treinamento
* **Unsloth** para treinamento eficiente de modelos
* **LoRA** para adaptação de modelos com baixo custo computacional
* **PyTorch** para operações de deep learning
* **CUDA** para aceleração via GPU


## Instruções para Execução do Código
Para executar o código deste projeto, siga as etapas abaixo:

1. **Criar um Ambiente Virtual** <br>
Primeiramente, é necessário criar um ambiente virtual para garantir que as dependências do projeto não entrem em conflito com outras instalações no seu sistema. Para isso, use o seguinte comando:

```bash
python -m venv venv
```

2. **Ativar o Ambiente Virtual**<br>
Em seguida, ative o ambiente virtual:

No Windows:

```cmd
.\venv\Scripts\activate
```

No macOS/Linux:
```bash
source venv/bin/activate
```

3. **Instalar as Dependências**<br>
Instale todas as bibliotecas necessárias utilizando o arquivo ``requirements.txt`` presente no repositório. Execute o seguinte comando:

```bash
pip install -r requirements.txt
```

4. **Rodar o Notebook**<br>
Após instalar as dependências, o código pode ser executado diretamente no Jupyter Notebook. 

**Observação:** O pré-processamento foi ajustado para o dataset específico utilizado neste projeto. Se você for utilizar outro conjunto de dados, será necessário ajustar as etapas de pré-processamento para atender às suas necessidades. Além disso, os prompts utilizados para gerar os outputs neutros e enviesados podem ser ajustados conforme a necessidade.
