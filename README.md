# 🎵 Kauan Music - Desafio de Desenvolvimento Web

## 🎯 Contexto do Projeto

**Você foi contratado pela Mateus Music**, uma empresa inovadora no segmento de streaming musical, para desenvolver uma plataforma web moderna que exiba o catálogo musical completo da empresa. 

A Mateus Music possui um acervo impressionante de **mais de 20.000 músicas** e precisa de uma interface elegante e funcional para apresentar esse conteúdo aos usuários.

## 📊 Sobre a Base de Dados

### Características Principais:
- **+20.000 músicas** no catálogo completo
- Dados de **Streams do Spotify** e **Views do YouTube**
- **Links dos vídeos** do YouTube para cada música
- **Metadados completos** dos artistas e faixas

### Estrutura da Base (exemplo):
```csv
Artist,Track,Stream,Views,Url_youtube
Artist Name,Song Title,150000000,50000000,https://youtube.com/...
```

## 🎨 Requisitos do Site

### 1. **Layout Principal**
- Título atrativo: "DJ Mateus 🎧 - As mais tocadas no Spotify e YouTube"
- Subtítulo explicativo sobre a rádio do DJ Mateuszão
- Layout responsivo e moderno

### 2. **Sistema de Filtros (Sidebar)**
- ✅ Seletor de artistas com todas as opções disponíveis
- ✅ Logo da empresa visível
- ✅ Filtros intuitivos e de fácil uso

### 3. **Apresentação das Músicas**
Cada música deve ser exibida com:

#### **Informações Principais:**
- 🎶 **Nome da Música** em destaque
- 🎵 **Número de Streams** no Spotify (formatado)
- 📺 **Número de Views** no YouTube (formatado)
- 🎬 **Player de Vídeo** integrado

#### **Requisitos Visuais:**
- ✅ Uso de **st.markdown** para estilização avançada
- ✅ **Containers estilizados** para cada música
- ✅ **Cores temáticas** (Spotify verde, YouTube vermelho)
- ✅ **Layout em colunas** para métricas
- ✅ **Separadores visuais** entre as músicas
- ✅ **Design responsivo** e profissional

### 4. **Estatísticas do Artista**
- 📊 Contagem total de músicas do artista
- 🎵 Soma total de streams no Spotify
- 📺 Soma total de views no YouTube

## 💻 Tecnologias Utilizadas

- **Streamlit** - Framework principal
- **Pandas** - Manipulação de dados
- **HTML/CSS** via st.markdown - Estilização
- **YouTube Player** integrado

## 🚀 Exemplo de Implementação Esperada

### Estrutura Básica do Código:
```python
import streamlit as st
import pandas as pd

# Configuração da página
st.set_page_config(page_title="DJ Mateus 🎧", layout="wide")

# Carregamento dos dados
df = pd.read_csv('Dados_Artistas.csv')

# Sidebar com filtros
# → Implementar seletor de artistas
# → Adicionar logo

# Header principal
# → Título e descrição

# Estatísticas do artista selecionado
# → Calcular totais

# Loop através das músicas do artista
for index, row in df_artista.iterrows():
    # → Container estilizado para cada música
    # → Métricas em colunas
    # → Player de vídeo
```

## 🎯 Critérios de Avaliação

### **Obrigatórios:**
1. ✅ Carregamento correto da base de dados
2. ✅ Sistema de filtro por artista funcional
3. ✅ Exibição de todas as informações das músicas
4. ✅ Integração com vídeos do YouTube
5. ✅ Uso de st.markdown para estilização

### **Diferenciais:**
1. 🎨 Design criativo e profissional
2. 📱 Layout responsivo
3. 🔢 Formatação adequada de números (1.000.000)
4. 🏷️ Organização visual clara
5. ⚡ Performance com base grande de dados

## 📝 Notas Importantes

### **Desafio Técnico:**
- A base possui **+20.000 registros** - otimização é crucial
- Garantir que a aplicação rode smooth mesmo com grande volume de dados

### **Expectativa da Empresa:**
A Mateus Music espera uma plataforma que:
- Seja visualmente atraente para engajar usuários
- Apresente dados de forma clara e organizada
- Ofereça boa experiência de navegação
- Destaque o vasto catálogo musical da empresa

## 🎼 Mensagem Final

"**Curta a playlist e aproveite a vibe! 🎶**"

---

**Boa sorte no desenvolvimento!** A Mateus Music conta com você para criar uma experiência musical excepcional! 🎧✨
