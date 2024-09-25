# analise_sentimentos_linkedin
Análise de sentimentos dos comentários sobre o app do LinkedIn no Google Play

## Sumário

> [Introdução](https://github.com/marioluciofjr/analise_sentimentos_linkedin/tree/main#introdu%C3%A7%C3%A3o)\
> [Como utilizar](https://github.com/marioluciofjr/analise_sentimentos_linkedin/tree/main#como-utilizar)\
> [Estrutura do projeto](https://github.com/marioluciofjr/analise_sentimentos_linkedin/tree/main#estrutura-do-projeto)\
> [Links úteis](https://github.com/marioluciofjr/analise_sentimentos_linkedin/tree/main#links-%C3%BAteis)\
> [Resultados](https://github.com/marioluciofjr/analise_sentimentos_linkedin/tree/main#resultados)\
> [Contribuições](https://github.com/marioluciofjr/analise_sentimentos_linkedin/tree/main#contribui%C3%A7%C3%B5es)\
> [Licença](https://github.com/marioluciofjr/analise_sentimentos_linkedin/tree/main#licen%C3%A7a)\
> [Contato](https://github.com/marioluciofjr/analise_sentimentos_linkedin/tree/main#contato)

## Introdução

Este projeto realiza a extração e análise de resenhas do aplicativo LinkedIn na Google Play Store, focando na análise de sentimentos e visualização de dados. Também gera nuvens de palavras para os sentimentos positivos e negativos.

## Como Utilizar

1. Clique na badge [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/marioluciofjr/analise_sentimentos_linkedin/blob/main/sentimentos_linkedin.ipynb)
2. Execute o código no Google Colab

Certifique-se de ter os seguintes pacotes instalados no ambiente de execução (Google Colab ou localmente):

- `google-play-scraper`
- `pysentimiento`
- `pandas`
- `nltk`
- `wordcloud`
- `plotly`
- `matplotlib`

### Instalação dos Pacotes Necessários

No Google Colab, as dependências podem ser instaladas automaticamente. Caso contrário, use o seguinte código para instalar manualmente:

```bash
!pip install google-play-scraper
!pip install pysentimiento
!pip install plotly
!pip install nltk
!pip install wordcloud
!pip install matplotlib
```

## Estrutura do projeto
<div>
  <img align="center" height="60" width="80" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original-wordmark.svg"/><br><br>
  sentimentos_linkedin.ipynb<br><br>
</div>

1. **Coleta de Resenhas da Google Play Store**: O código utiliza a biblioteca google-play-scraper para extrair todas as resenhas do aplicativo do LinkedIn disponível na Google Play Store. As resenhas são coletadas no idioma português do Brasil e são ordenadas por relevância.

2. **Análise de Sentimento**: Usando o pacote pysentimiento, o código realiza uma análise de sentimento das resenhas coletadas, categorizando-as como positivas (POS), negativas (NEG), ou neutras (NEU).

3. **Visualização da Distribuição de Sentimentos**: As resenhas são agrupadas com base nos sentimentos (positivo, negativo, neutro) e exibidas em um gráfico de barras interativo, utilizando a biblioteca plotly.express.

4. **Geração de Nuvens de Palavras**: O código gera nuvens de palavras com base nas resenhas positivas e negativas, removendo stopwords (palavras comuns irrelevantes), para identificar os termos mais frequentes em cada tipo de sentimento.

5. **Gravação e Leitura de Dados**: As resenhas extraídas da Google Play Store são salvas em um arquivo CSV chamado reviews.csv, que posteriormente é carregado para análise de sentimento e visualização.

## Links Úteis
Durante o projeto utilizei várias ferramentas muito úteis e deixo aqui os links e alguns comentários de como foram importantes para mim neste projeto, até mesmo para quem deseja saber melhor ou mesmo compor seus próprios trabalhos:

+ [Como salvar em uma planilha os reviews de um aplicativo da Play Store](https://tatiany-lukrafka.medium.com/como-salvar-em-uma-planilha-os-reviews-de-um-aplicativo-na-play-store-83452042a195) - artigo sobre o método de scraping dos reviews no Google Play;
+ [Pysentimiento](https://huggingface.co/pysentimiento/bertweet-pt-sentiment) - modelo pré-treinado para análise de sentimentos em língua portuguesa e publicado no Hugging Face;
+ [App do LinkedIn no Google Play](https://play.google.com/store/apps/details?id=com.linkedin.android&hl=pt_BR) - página do aplicativo do LinkedIn no Google Play;
+ [Curso Alura de Hugging Face: explorando e aplicando soluções com modelos de IA ](https://cursos.alura.com.br/course/hugging-face-explorando-aplicando-solucoes-modelos-ia) - curso Alura ministrado pela instrutora [Valquíria Alencar](https://www.linkedin.com/in/valquiria-alencar).

## Resultados

### Gráfico de análise de sentimentos

<div>
  <img align="center" src="https://github.com/marioluciofjr/analise_sentimentos_linkedin/blob/main/grafico.png"/><br><br>
</div>

### Nuvem de palavras da análise de sentimento positiva

<div>
  <img align="center" src="https://github.com/marioluciofjr/analise_sentimentos_linkedin/blob/main/sent_pos_linkedin.png"/><br><br>
</div>

### Nuvem de palavras da análise de sentimento negativa

<div>
  <img align="center" src="https://github.com/marioluciofjr/analise_sentimentos_linkedin/blob/main/sent_neg_linkedin.png"/><br><br>
</div>


## Contribuições
Contribuições são bem-vindas! Se você tem sugestões para melhorar este projeto, sinta-se à vontade para criar um fork do repositório, fazer suas alterações e enviar um pull request.

## Licença
Este projeto está sob a licença MIT. Veja o arquivo [![LICENSE](https://img.shields.io/badge/LICENSE-42ffff?style=plastic&link=https://github.com/marioluciofjr/neurotransmissores/blob/main/LICENSE)](https://github.com/marioluciofjr/neurotransmissores/blob/main/LICENSE) para mais detalhes.

## Contato
Mário Lúcio - Prazo Certo®
<div>  	
  <a href="https://www.linkedin.com/in/marioluciofjr" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a> 
  <a href = "mailto:marioluciofjr@gmail.com" target="_blank"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white"></a>
  <a href="https://prazocerto.me/contato" target="_blank"><img src="https://img.shields.io/badge/prazocerto.me/contato-230023?style=for-the-badge&logo=wordpress&logoColor=white"></a>
  
</div>

