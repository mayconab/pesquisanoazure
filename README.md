<h1>
    <a href="https://www.dio.me/">
     <img align="center" width="40px" src="https://hermes.digitalinnovation.one/assets/diome/logo-minimized.png"></a>
    <span> Pesquisas com IA Azure</span>
</h1>

## Sobre o Projeto
Página desenvolvida para fins didáticos para o curso *Microsoft - AZURE AI-900** da [Digital Innovation One](https://www.dio.me/). O projeto é um estudo sobre a criação de AI na plataforma Azure Microsoft. Adicionei legendas em uma imagem de hambúrguer que foi trago os seguintes resultados:


## Descrição

Este projeto tem como objetivo demonstrar a análise de uma sentença utilizando IA. A sentença fornecida descreve uma experiência negativa em um restaurante, especificamente no Mc'Donald's. A análise será feita para identificar os pontos negativos mencionados na sentença e fornecer o resultado sobre a experiência do cliente.

A pasta `inputs` contém o arquivo `sentencas.txt`, que possui a sentença que será analisada pela IA.

**Conteúdo da pasta `pesquisa`**:

## Passo a Passo para Configurar uma Pesquisa no Azure

### 1. Configuração do Ambiente

Antes de começar, certifique-se de que você tem:
- Uma conta no Azure.
- O Azure Portal acessível.
- Um workspace do Azure criado.

### 2. Criar um Serviço de Pesquisa Cognitiva do Azure

1. **Acesse o Azure Portal**:
   - Vá para o [Azure Portal](https://portal.azure.com/).

2. **Criar um Serviço de Pesquisa Cognitiva**:
   - No menu lateral, clique em "Criar um recurso".
   - Pesquise por "Azure Cognitive Search" e selecione-o.
   - Clique em "Criar".
   - Preencha os detalhes necessários, como nome do serviço, assinatura, grupo de recursos e localização.
   - Escolha o tipo de preço (recomendado: Free ou Basic para testes).
   - Clique em "Revisar + criar" e depois em "Criar".

3. **Aguardar a Implantação**:
   - Aguarde até que o serviço seja implantado. Isso pode levar alguns minutos.

### 3. Configurar o Índice de Pesquisa

1. **Acesse o Serviço de Pesquisa**:
   - No Azure Portal, vá para o serviço de pesquisa que você acabou de criar.

2. **Criar um Índice**:
   - No painel do serviço de pesquisa, clique em "Índices".
   - Clique em "Adicionar índice".
   - Dê um nome ao índice e defina os campos que ele deve conter. Por exemplo:
     - `id` (Edm.String) - Chave
     - `title` (Edm.String) - Título
     - `content` (Edm.String) - Conteúdo
   - Clique em "Criar".

### 4. Carregar Dados no Índice

1. **Preparar os Dados**:
   - Prepare um conjunto de dados que você deseja indexar. Pode ser um arquivo CSV, JSON, ou outro formato.

2. **Carregar Dados**:
   - No Azure Portal, você pode usar a interface gráfica para carregar os dados no índice.

### 5. Testar a Pesquisa

1. **Usar o Azure Portal**:
   - No painel do serviço de pesquisa, clique em "Índices".
   - Selecione o índice que você criou.
   - Clique em "Pesquisar" para testar consultas.

---
