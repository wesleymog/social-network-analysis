# Análise de Redes Sociais: Evolução do Discurso no Instagram

Este repositório contém o artigo científico **"Analisando a Evolução Do Discurso No Instagram: Revelando O Papel Das Redes Sociais Na Invasão de Brasília Em 8 de Janeiro de 2023"** e todo o material de pesquisa relacionado.

## 📋 Sobre o Artigo

### Resumo

Este estudo analisa a evolução do discurso no Instagram de indivíduos envolvidos na tentativa de golpe ocorrida em 8 de janeiro de 2023, em Brasília. A pesquisa examina dois grupos distintos: pessoas verificadas associadas ao ex-presidente Jair Bolsonaro e indivíduos presentes durante o ataque aos prédios do Congresso Nacional, Palácio do Planalto e Supremo Tribunal Federal.

### Objetivos

- Analisar mudanças no discurso antes e depois do evento de 8 de janeiro
- Identificar padrões de sentimento e frequência de postagens
- Examinar a evolução das menções e palavras-chave utilizadas
- Compreender o papel das redes sociais na disseminação de discursos antidemocráticos

### Metodologia

- **Coleta de dados**: Utilização da ferramenta CrowdTangle para monitorar postagens do Instagram
- **Análise de sentimentos**: Implementação do VADER (Valence Aware Dictionary and Sentiment Reasoner)
- **Visualização**: Geração de nuvens de palavras e gráficos temporais
- **Período de análise**: 30/10/2022 a 10/04/2023 (antes e depois do evento)

## 📁 Estrutura do Repositório

### Arquivos Principais

- `artigo_ars.tex` - Artigo principal em LaTeX (formato ACM)
- `artigo_ars.pdf` - Versão final do artigo em PDF
- `referencias.bib` - Base de dados bibliográfica
- `README.md` - Este arquivo

### Scripts de Análise

- `gerar_figuras_reais.py` - Script principal para geração de gráficos e análises
- `gerar_nuvens_palavras.py` - Script específico para criação de nuvens de palavras
- `Colab_Redes_Sociais.ipynb` - Notebook do Google Colab com análises interativas

### Dados

- `CSV - Bases de Dados/` - Diretório contendo os datasets utilizados:
  - `df_publicas_before.csv` - Postagens de pessoas verificadas (antes do evento)
  - `df_publicas_after.csv` - Postagens de pessoas verificadas (depois do evento)
  - `df_presentes_before.csv` - Postagens de presentes no ato (antes do evento)
  - `df_presente_after.csv` - Postagens de presentes no ato (depois do evento)

### Figuras Geradas

- **Análise de Sentimentos** (figuras 1-8): Gráficos diários e mensais de sentimentos
- **Nuvens de Menções** (figuras 13-16): Visualização das menções mais frequentes
- **Nuvens de Palavras** (figuras 17-24): Palavras-chave mais utilizadas
- **Frequência de Postagens** (figuras 25-28): Análise temporal de atividade

### Template e Formatação

- `ACM_Journals_Primary_Article_Template/` - Template ACM para formatação acadêmica

## 🔬 Principais Descobertas

### Análise de Sentimentos

- **Turbulência emocional**: Variação significativa nos sentimentos expressos
- **Mudança temporal**: Tendência a sentimentos mais negativos após o evento
- **Diferenças entre grupos**: Padrões distintos entre pessoas verificadas e presentes no ato

### Análise de Conteúdo

- **Centralidade de figuras políticas**: Foco em Jair Bolsonaro e Lula
- **Evolução das menções**: Redução nas menções ao ex-presidente após o evento
- **Mudança de foco**: Transição de temas políticos para outros assuntos

### Frequência de Postagens

- **Pessoas verificadas**: Aumento na frequência de postagens após o evento
- **Presentes no ato**: Redução drástica na atividade nas redes sociais
- **Padrão temporal**: Mudanças significativas nos meses seguintes ao evento

## 🛠️ Como Executar as Análises

### Pré-requisitos

```bash
pip install pandas matplotlib seaborn wordcloud nltk vaderSentiment
```

### Executar Análises

```bash
python gerar_figuras_reais.py
```

### Compilar o Artigo

```bash
pdflatex artigo_ars.tex
bibtex artigo_ars
pdflatex artigo_ars.tex
pdflatex artigo_ars.tex
```

## 📊 Resultados Principais

1. **Mudança Significativa no Discurso**: Evidências claras de alteração nos padrões de comunicação
2. **Impacto do Evento**: Redução na atividade e mudança no tom das postagens
3. **Polarização Política**: Manutenção de temas políticos centrais
4. **Evolução Temporal**: Padrões distintos antes e depois do evento

## 🎯 Contribuições

Este trabalho contribui para:

- Compreensão do papel das redes sociais em eventos políticos
- Metodologia para análise de sentimentos em português
- Estudos sobre desinformação e polarização política
- Análise de comportamento em redes sociais durante crises

## 📚 Referências

O artigo cita trabalhos fundamentais em:

- Análise de sentimentos em redes sociais
- Estudos sobre desinformação política
- Metodologias de análise de dados sociais
- Pesquisas sobre eventos similares (ex: ataque ao Capitólio dos EUA)

## 👥 Autores

- **Lucas da Silva Farias** (lukz@ic.ufrj.br)
- **Wesley Mota de Oliveira Gomes** (wesleymota@ic.ufrj.br)
- **Marcelo Drummond Fonseca** (marcelodrummondfonseca@gmail.com)

**Instituição**: Instituto de Computação - Universidade Federal do Rio de Janeiro (UFRJ)

## 📄 Licença

Este projeto está sob licença acadêmica. Os dados utilizados seguem as diretrizes éticas de pesquisa em redes sociais.

## 🤝 Agradecimentos

Agradecimentos especiais ao Silas pela colaboração na obtenção de dados e à Prof.ª Jonice pela orientação e disponibilização das ferramentas necessárias para a pesquisa.

---

_Este repositório contém material de pesquisa acadêmica. Para uso comercial ou redistribuição, entre em contato com os autores._
