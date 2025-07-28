# Conversão do Artigo ARS para LaTeX ACM

Este repositório contém a conversão do artigo "Analisando a Evolução Do Discurso No Instagram: Revelando O Papel Das Redes Sociais Na Invasão de Brasília Em 8 de Janeiro de 2023" do formato Markdown para LaTeX usando o template ACM.

## Arquivos

- `artigo_ars.tex` - Arquivo principal em LaTeX
- `referencias.bib` - Arquivo com as referências bibliográficas
- `ACM_Journals_Primary_Article_Template/` - Pasta com o template ACM

## Como compilar

### Pré-requisitos

Você precisa ter um compilador LaTeX instalado (como TeX Live, MiKTeX, ou Overleaf).

### Compilação

1. **Compilação básica:**

   ```bash
   pdflatex artigo_ars.tex
   bibtex artigo_ars
   pdflatex artigo_ars.tex
   pdflatex artigo_ars.tex
   ```

2. **Ou usando latexmk (recomendado):**
   ```bash
   latexmk -pdf artigo_ars.tex
   ```

### Estrutura do documento

O documento LaTeX inclui:

- **Cabeçalho ACM**: Configurado para revista com informações dos autores
- **Abstract**: Em inglês conforme padrão ACM
- **CCS Concepts**: Classificação ACM Computing Classification System
- **Keywords**: Palavras-chave em português
- **Seções principais**:
  - Introdução
  - Revisão da Literatura
  - Materiais e Métodos
  - Resultados
  - Avaliação e Discussão
  - Conclusão
  - Agradecimentos
  - Referências

### Notas importantes

1. **Figuras**: O documento contém comentários indicando onde as figuras devem ser inseridas. Para adicionar as figuras:

   - Salve as imagens na mesma pasta
   - Descomente as linhas `\begin{figure}` e `\end{figure}`
   - Ajuste o caminho das imagens conforme necessário

2. **Referências**: Todas as referências estão no arquivo `referencias.bib` e são citadas no texto usando `\cite{chave}`.

3. **Template**: O documento usa o template ACM `acmart.cls` que está na pasta `ACM_Journals_Primary_Article_Template/`.

### Personalizações feitas

- Configuração para revista ACM
- Abstract em inglês
- CCS Concepts apropriados para análise de redes sociais
- Estrutura de seções e subseções mantida do original
- Citações e referências formatadas conforme padrão ACM
- Footnotes para URLs e informações adicionais

### Problemas comuns

1. **Erro de compilação**: Certifique-se de que o template ACM está acessível
2. **Referências não aparecem**: Execute `bibtex` após a primeira compilação
3. **Figuras não carregam**: Verifique se os arquivos de imagem existem no caminho especificado

## Estrutura das referências

As referências incluem:

- Livros acadêmicos
- Artigos de conferência
- Dissertações
- Artigos online
- Materiais diversos (misc)

Todas seguem o formato ACM-Reference-Format.
