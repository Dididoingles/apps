# [US] digital

Uma iniciativa digital gratuita que concentra ferramentas criadas pela professora Diandra para ajudar as pessoas a aprenderem Inglês de graça.

## Sobre o projeto

O [US] digital nasceu do desejo de ensinar Inglês para quem não tinha acesso. Tudo começou com aulas gratuitas aos fins de semana para alunos carentes. Com o tempo, a iniciativa cresceu e se transformou em uma plataforma digital com ferramentas interativas, práticas e gratuitas para o aprendizado de Inglês.

## Funcionalidades

O projeto conta com uma página principal com a vitrine de ferramentas, uma página de conversação com o robô Mars, uma página de conversa livre com avaliação de pronúncia e gramática, e uma página sobre a história do projeto.

Na página de conversação, o usuário escolhe um tópico, o Mars fala o texto (via Web Speech API), o aluno repete usando o microfone (via SpeechRecognition), e o sistema avalia a semelhança entre o que foi dito e o que era esperado, gerando uma porcentagem de acerto.

Na página de conversa livre, o Mars sorteia uma pergunta de um banco de dados. O aluno responde o que quiser. O sistema avalia a resposta com base na quantidade de palavras, variedade de vocabulário, ritmo e, opcionalmente, na checagem gramatical real feita pela API da LanguageTool.

## Estrutura de pastas


usdigital/
├── assets/
├── conversas/
│   ├── aleatorio.txt
│   ├── amigo.txt
│   ├── comidafavorita.txt
│   ├── index.json
│   ├── intro.txt
│   ├── pet.txt
│   └── viagem.txt
├── outros/
│   ├── carrousel.isolado.html
│   └── info.txt
├── roleplay/
│   ├── index.html
│   └── livre.html
├── tools/
│   └── index.html
├── usdigital/
│   └── index.html
├── favicon.png
├── index.html
└── README.md

Como rodar localmente
Como o projeto usa a API de fetch para carregar arquivos .txt e .json, não é possível abrir os arquivos HTML diretamente com duplo clique (file://). É necessário rodar um servidor local simples.

Com Python instalado, navegue até a pasta do projeto e execute:

bash
python3 -m http.server 8000
Depois, acesse http://localhost:8000 no navegador.

Tecnologias utilizadas
HTML5, CSS3 e JavaScript puro (Vanilla). Não há dependências de frameworks, bibliotecas externas ou processo de build.

A voz do Mars é gerada pela Web Speech API (SpeechSynthesis). O reconhecimento da voz do aluno é feito pela Web Speech API (SpeechRecognition), que tem melhor suporte no Chrome e no Edge. A avaliação gramatical opcional usa a API pública da LanguageTool.

Navegadores compatíveis
O recurso de reconhecimento de voz funciona melhor no Google Chrome e no Microsoft Edge (desktop e Android). O Safari tem suporte limitado, e o Firefox não suporta SpeechRecognition nativamente. A página exibe um aviso caso o navegador não ofereça suporte.

Aviso sobre a avaliação
A avaliação das respostas combina uma heurística local (quantidade de palavras, variedade, ritmo) com a API da LanguageTool. Nenhuma das duas é 100% precisa. A ferramenta é um apoio ao estudo e não substitui a correção de um professor.

Licença
Este projeto é de uso gratuito, mas a comercialização, a cópia e a adaptação são expressamente proibidas sem autorização prévia por escrito da autora.

Você pode usar, estudar e praticar com o material. Você não pode vender, redistribuir como seu, ou modificar o código para outros fins sem permissão.

Para autorizações, entre em contato pelo Instagram: @dicarvalho.prof

Desenvolvido por professora Diandra de Inglês.
Instagram: @dicarvalho.prof
