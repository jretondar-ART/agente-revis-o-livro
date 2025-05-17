# agente-revisão-livro autor: José Carlos da Costa Retondar projeto para as aulas da IMERSÃO AI terceira edição da ALURA
## Manual de Utilização do Agente de Revisão e Marketing de Livros (Para Usuários no GitHub)

Este manual explica como utilizar o agente de IA para revisar livros e gerar resumos para marketing, disponibilizado no GitHub. Este agente foi desenvolvido utilizando o Google colab e com auxilio do google Gemini e é executado no ambiente Google Colaboratory.

**Pré-requisitos:**

  * **Conta Google:** Necessária para acessar e executar o projeto no Google Colaboratory.
  * **Acesso ao GitHub:** Você precisará de uma conta GitHub para acessar o repositório do projeto.
  * **Arquivo do Livro:** O arquivo do seu livro deve estar em formato de texto simples (`.txt`) ou em formato PDF (`.pdf`).

**Passo a Passo:**

1.  **Acessando o Projeto no Google Colaboratory:**

      * No GitHub, navegue até o repositório onde o projeto `revisor_de_livros_e_ebook.ipynb` está hospedado.
      * Procure por um botão ou link que diga algo como "Open in Colab" ou "View in Colab". Clique neste link. Isso abrirá o notebook diretamente no seu Google Colaboratory.

2.  **Configurando o Ambiente (Chave de API):**

      * **Importante:** Para que o agente funcione, você precisará fornecer sua própria chave de API do Google AI Studio. Se você ainda não tem uma, siga estas instruções:
          * Abra o Google AI Studio no seu navegador: [https://makersuite.google.com/app/apikey](https://makersuite.google.com/app/apikey)
          * Crie uma nova chave de API, se necessário.
          * Copie a chave gerada. **Mantenha essa chave em segurança e não a compartilhe publicamente no GitHub.**
      * No notebook Colab aberto, localize a célula de código onde a chave de API é configurada (geralmente marcada com um comentário como `# Insira sua chave de API aqui`).
      * Substitua o texto placeholder (como `"SUA_CHAVE_DE_API"`) pela sua chave de API real, **mantendo as aspas**.
      * Execute esta célula de código (clique no "play" ou pressione `Shift + Enter`).

3.  **Executando as Funções do Agente:**

      * O notebook Colab conterá várias células de código definindo as funções do agente (para leitura de arquivos, revisão, marketing e o chatbot).
      * Execute cada uma dessas células de código na ordem em que aparecem no notebook. Isso garante que todas as funções necessárias estejam carregadas na memória do Colab.

4.  **Utilizando o Chatbot:**

      * Procure pela célula de código que inicia o chatbot (geralmente com a chamada da função `chatbot_ebook()` e sem o `#` na frente).
      * Execute esta célula. O chatbot será iniciado e exibirá uma mensagem solicitando o caminho do arquivo do seu livro.

5.  **Fornecendo o Caminho do Arquivo do Livro:**

      * O chatbot pedirá o caminho do arquivo do seu livro (`.txt` ou `.pdf`). Você tem duas opções principais para disponibilizar o arquivo para o Colab:

          * **Utilizando arquivos do Google Drive:**
              * Faça o upload do seu arquivo de livro para o seu Google Drive, se ainda não estiver lá.
              * Para obter o caminho correto: clique com o botão direito no arquivo no Google Drive, selecione "Detalhes" e copie o "Local". O caminho completo geralmente começa com `/content/drive/MyDrive/` seguido pela estrutura de pastas até o seu arquivo (ex: `/content/drive/MyDrive/Meus Livros/meu_livro.txt` ou `/content/drive/MyDrive/Ebooks/meu_ebook.pdf`).
              * Cole este caminho completo no chatbot e pressione Enter.

          * **Fazendo o Upload Direto para o Colab (para arquivos menores):**
              * No painel esquerdo do Colab, clique no ícone de pasta ("Arquivos").
              * Clique no ícone de "upload" (seta para cima) e selecione o arquivo do seu computador para fazer o upload.
              * Após o upload, o arquivo estará na raiz do ambiente Colab. O caminho que você deverá digitar no chatbot será simplesmente o nome do arquivo (ex: `meu_livro.txt` ou `meu_ebook.pdf`).

6.  **Interagindo com o Chatbot:**

      * Após fornecer o caminho do arquivo, o chatbot perguntará o que você gostaria de fazer: `revisar`, `marketing` ou `sair`. Digite a ação desejada e pressione Enter.

      * **Para Revisar:**
          * Digite `revisar` e pressione Enter.
          * O chatbot perguntará se você tem algum pedido específico para a revisão (ex: "Verificar erros de digitação e gramática avançada"). Digite seu pedido ou apenas pressione Enter para a revisão padrão.
          * O agente processará o texto e exibirá o relatório de revisão.

      * **Para Marketing:**
          * Digite `marketing` e pressione Enter.
          * O chatbot perguntará que tipo de resumo de marketing você gostaria (ex: "Criar um resumo curto para redes sociais"). Digite seu pedido ou apenas pressione Enter para um resumo padrão.
          * O agente processará o texto e exibirá o resumo de marketing.

      * **Para Sair:**
          * Digite `sair` e pressione Enter para encerrar o chatbot.

7.  **Repetindo o Processo:**

      * Você pode continuar interagindo com o chatbot para realizar diferentes ações com o mesmo arquivo ou fornecer o caminho de um novo arquivo para análise.

**Observações Importantes para Usuários:**

  * **Chave de API:** Sua chave de API é pessoal e deve ser mantida em segredo. Não a compartilhe publicamente.
  * **Caminhos de Arquivo:** Certifique-se de que o caminho do arquivo fornecido ao chatbot esteja correto.
  * **Codificação de Arquivos `.txt`:** Para arquivos de texto, utilize a codificação UTF-8 para melhor suporte a caracteres especiais.
  * **Tamanho do Arquivo:** Arquivos muito grandes podem levar mais tempo para serem processados e podem atingir as limitações do modelo de linguagem. Considere testar com partes menores se necessário.
  * **Pedidos Específicos:** Seja claro e específico ao fazer seus pedidos de revisão e marketing para obter os melhores resultados.
  * **Ambiente Colab:** Lembre-se que o ambiente do Google Colab é temporário. Se você fechar a aba ou ficar inativo por um tempo, o ambiente será resetado e você precisará executar as células novamente (mas sua chave de API permanecerá na célula, a menos que você a remova).

Esperamos que este manual ajude você a utilizar o agente de revisão e marketing de livros com sucesso\! Em caso de dúvidas ou problemas, consulte a documentação do projeto no GitHub ou entre em contato com o mantenedor do repositório.
