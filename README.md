# Análise de Similaridade de Textos - Jaccard e Cosseno

Este repositório contém notebooks e uma base de dados voltados para a análise de similaridade de textos utilizando as métricas de **Similaridade Cosseno** e **Similaridade de Jaccard**.

## Conteúdo do Repositório

- `Cosseno.ipynb`: Notebook contendo a implementação da Similaridade de Cosseno aplicada à análise de feedbacks de clientes.
- `Jaccard.ipynb`: Notebook contendo a implementação da Similaridade de Jaccard para comparação de textos, com foco em categorizar as reclamações de clientes.
- `Base - FeedBacks Clientes.xlsx`: Conjunto de dados com feedbacks coletados de clientes, utilizado para as análises de similaridade nos notebooks.

## Requisitos

Para executar os notebooks, você precisará dos seguintes pacotes Python:

- `pandas`
- `numpy`
- `nltk`
- `sklearn`
- `matplotlib`
- `seaborn`
  
Você pode instalar os pacotes necessários rodando:

```bash
pip install pandas numpy nltk scikit-learn matplotlib seaborn
```

## Estrutura dos Dados

O arquivo `Base - FeedBacks Clientes.xlsx` contém dados de feedbacks de clientes, que são classificados em seis categorias principais. Cada linha representa um feedback textual associado a uma das seguintes categorias, com a seguinte distribuição no conjunto de dados:

| Categoria            | Contagem |
|----------------------|----------|
| Não necessário        | 731      |
| Comercial             | 337      |
| Gestão de Terceiros   | 220      |
| Implantação           | 119      |
| Estratégia            | 50       |
| Marketing             | 26       |

### Explicação das Categorias:

- **Comercial**: Refere-se a questões comerciais, como o seguinte exemplo:
  
  > "O correspondente informa que o movimento na loja caiu, mas pretende continuar operando. Ele está entrando em contato com seus clientes, oferecendo e informando sobre os benefícios. O correspondente já tem acesso ao site e solicita o aumento do limite de recebimentos para pagamentos de boletos, pois tem essa demanda. O valor atual permitido é insuficiente."

- **Gestão de Terceiros**: Focado em questões de recebimento de equipamento e treinamento, como:

  > "O correspondente informa que recebeu o treinamento técnico, mas ficou com dúvidas. A instalação foi feita, mas o treinamento foi muito rápido e ele precisaria de outro contato."

- **Implantação**: Engloba problemas técnicos com o equipamento ou falta de serviços, como:

  > "O correspondente informou que a maquininha está travada, pedindo uma atualização que ele não consegue realizar. Já abriu um chamado na van, mas não foi dado um prazo para solução, e ele está aguardando."

- **Marketing**: Relaciona-se à falta de materiais de divulgação para os correspondentes, como:

  > "O correspondente informa que não opera, pois as pessoas não se interessam. Disseram que só instalaram o aparelho e foram embora, deixando a necessidade de banners e mais acessórios para identificar a operação. Ele também sente a falta de acompanhamento de alguém."

- **Estratégia**: Trata de informações pontuais e comerciais que podem ser resolvidas sem a necessidade do time comercial, como:

  > "O correspondente informou que tudo ocorreu bem, mas não foi informado sobre o acelerador ou a campanha. O treinamento foi realizado sem deixar dúvidas."

- **Não necessário**: Frases que não representam uma dor ou necessidade do cliente e, portanto, não requerem ação por parte da equipe, como:

  > "A implantação foi um sucesso e finalizada está operando normalmente"

# Análises Incluídas
## Similaridade de Cosseno
O notebook `Cosseno.ipynb` implementa a métrica de Similaridade Cosseno, que é amplamente usada para medir a similaridade entre dois textos com base no ângulo entre seus vetores de palavras obtidos através da técnica TF-IDF.

## Similaridade de Jaccard
O notebook `Jaccard.ipynb` aplica a métrica de Similaridade de Jaccard, que calcula a similaridade baseada no tamanho da interseção e da união de dois conjuntos de palavras.

## Considerações Finais

Este projeto tem como objetivo fornecer uma solução prática para análise de similaridade de textos aplicando as métricas de Similaridade de Jaccard e Similaridade de Cosseno, utilizando feedbacks reais de clientes. Ele serve tanto para fins de estudo como para aplicação prática em cenários de categorização automática de textos. 

## Autores

- **Igor da Silva Alencar** - _Trabalho Inicial_ - [Seu Perfil no GitHub](https://github.com/seu-usuario)
