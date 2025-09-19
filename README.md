<div style="text-align: justify;">

## Análise de Sentimentos com Dragon Ball Z

## 🛠️ Ferramentas utilizadas

![Azure Speech Studio](https://img.shields.io/badge/Azure%20Speech%20Studio-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white) 
![Azure Language Studio](https://img.shields.io/badge/Azure%20Language%20Studio-0089D6?style=for-the-badge&logo=azuredevops&logoColor=white) 

Azure Speech Studio – transcrição de fala para texto.  
Azure Language Studio – análise de sentimentos.  

## 🎯 Objetivo

Este projeto demonstra o uso de IA da Azure (Speech Studio + Language Studio) para analisar sentimentos em falas icônicas do anime Dragon Ball Z.  
Foi utilizada a fala do Android 16 para Gohan como exemplo, transformando a transcrição em uma análise de sentimentos.

<p align="center">
  <img src="gohan3.jpg" width="500" alt="Dragon Ball Z - Saga Cell">
  <br>
  <em>Figura 1 - Dragon Ball Z - Saga dos Androids & Saga Cell</em>
</p>

</div>

## 1️⃣ Transcrição da fala com Azure Speech Studio

Depois de criar a conta no Azure e o recurso necessário, acesse o Azure Speech Studio e escolha a função utilizada; nesse caso, será a etapa de **conversão de voz para texto**:

<p align="center">
  <img src="gohan4.gif" width="500" alt="Azure Speech Studio">
  <br>
  <em>Figura 2 — Azure Speech Studio</em>
</p>

Após acessar a aba de conversão de voz para texto, realize o upload do áudio e aguarde o resultado da transcrição. Observa-se que o texto é apresentado com a acentuação e a estrutura gramatical que a IA interpreta como corretas:

<p align="center">
  <img src="gohan5.gif" width="500" alt="Transcrição do Azure Speech Studio">
  <br>
  <em>Figura 3 — Transcrição do Azure Speech Studio</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/a08a19a3-3972-4921-bc49-9436a1f05f87" width="1210" height="302" alt="Transcrição do Azure Speech Studio">
  <br>
  <em>Figura 4 — Transcrição do Azure Speech Studio</em>
</p>

Percebe-se que a IA, ao receber o áudio, interpreta algumas frases do Android 16 como perguntas:

- "Gohan, vê se você me escuta?"  
- "Pense, existem inimigos que não são convencidos com palavras?"  
- "E as plantas desse mundo?"

No episódio, percebemos que ele **não está realmente perguntando nada**. Ele apenas chama a atenção de Gohan durante a luta e faz seu discurso antes de morrer. Essa diferença ocorre porque a IA interpreta o áudio de forma diferente da percepção humana da cena.

<p align="center">
  <img src="gohan6.gif" width="500" alt="Morte de Android 16">
  <br>
  <em>Figura 5 — Morte de Android 16</em>
</p>

## 2️⃣ Análise de Sentimentos com Azure Language Studio

Depois de criar a conta no Azure e o recurso necessário, acesse o **Azure Language Studio** e importe o texto gerado no Speech Studio para realizar a análise de sentimentos:

<p align="center">
  <img src="gohan7.gif" width="500" alt="Análise de Sentimentos">
  <br>
  <em>Figura 6 — Análise de Sentimentos</em>
</p>

<div style="text-align: justify;">

Se seguirmos o mesmo texto que foi gerado na ferramenta anterior e utilizarmos na nossa análise, teremos o seguinte resultado:

<p align="center">
  <img src="https://github.com/user-attachments/assets/63d7ee14-bd5f-4023-99ec-b047f1d34c71" width="223" height="151" alt="Realização da análise de Sentimentos">
  <br>
  <em>Figura 7 - Realização da análise de Sentimentos</em>
  <!-- Insira aqui o texto explicativo da Figura 7 -->
</p>

O modelo quebra o texto em sentenças para explicar o resultado do gráfico e realiza a busca por palavras-chave para avaliar o conteúdo. Aqui, ele buscou palavras como "plantas" e "amei":

<p align="center">
  <img src="https://github.com/user-attachments/assets/14d07950-adb2-4b47-a9b2-ba2c07890e4d" width="826" height="475" alt="Gráfico gerado com o resultado final da análise">
  <br>
  <em>Figura 8 - Gráfico gerado com o resultado final da análise</em>
  <!-- Insira aqui o texto explicativo da Figura 8 -->
</p>

Segundo a imagem, o texto foi interpretado como algo positivo. Logo, o discurso feito pelo Android 16 foi de grande ajuda para que Gohan desbloqueasse todo o seu poder oculto e enfrentasse Cell.



Agora, será que há diferença nesse resultado ao utilizar o texto **corrigido gramaticalmente**? Após a correção e nova análise na ferramenta, temos:

<p align="center">
  <img src="https://github.com/user-attachments/assets/62e10951-5f8f-4f74-9d0f-4dcb2d48f785" width="1214" height="648" alt="Nova análise com correção ortográfica">
  <br>
  <em>Figura 9 - Nova análise com correção ortográfica</em>
  <!-- Insira aqui o texto explicativo da Figura 9 -->
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/a9f01561-768f-462a-9b8b-fa2ec46bf0ee" width="266" height="193" alt="Resultado das sentenças">
  <br>
  <em>Figura 10 - Resultado das sentenças</em>
  <!-- Insira aqui o texto explicativo da Figura 10 -->
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/ce0cfc66-fd47-4657-ac51-c98433b636b6" width="528" height="347" alt="Resultados das sentenças">
  <br>
  <em>Figura 11 - Resultados das sentenças</em>
  <!-- Insira aqui o texto explicativo da Figura 11 -->
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/3acb4eb2-2d12-4b7a-8318-cfadeb077fa6" width="611" height="292" alt="Resultados das sentenças">
  <br>
  <em>Figura 12 - Resultados das sentenças</em>
  <!-- Insira aqui o texto explicativo da Figura 12 -->
</p>

Percebe-se que o resultado foi alterado. Antes, o modelo interpretava a maioria do texto como positiva, mas após a correção gramatical, o modelo apresenta avaliações negativas.  
Esse resultado mostra  como a **correção gramatical influencia diretamente** o resultado final da análise de sentimentos, mostrando que ajustes no texto podem alterar a interpretação da IA.

</div>
