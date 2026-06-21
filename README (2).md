# risco·certo — Simulado de Vestibular

App de questões de vestibular com login, dashboard de progresso, metas de estudo diárias, prática de redação, flashcards com repetição espaçada e estatísticas avançadas.

## Funcionalidades

- **Login e cadastro** próprios, com dados salvos no navegador (localStorage)
- **Banco de questões** organizado por matéria, com gabarito comentado
- **Cronômetro** de sessão, por questão e tempo total acumulado
- **Meta de estudo diária** (minutos ou número de questões)
- **Revisão de erros** — lista automática de questões erradas para refazer
- **Estatísticas avançadas**: pontos fracos por matéria, gráfico de evolução da taxa de acerto e heatmap de atividade
- **Flashcards com repetição espaçada (SRS)** — mais de 100 cartões prontos em 8 matérias, com algoritmo que prioriza o que você tem mais dificuldade
- **Prática de redação** com temas estilo ENEM ou tema livre, editor com contador de palavras/linhas e autosave
- **Foto de perfil** personalizável
- Totalmente **responsivo** (desktop e mobile)

## Como usar

🔗 **Acesse online:** `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`
*(troque pelos seus dados depois de publicar — veja o passo a passo no final deste README)*

Ou simplesmente abra o arquivo `index.html` direto no navegador, sem precisar de internet.

## ⚠️ Importante sobre os dados

Este é um app **100% estático**, sem servidor e sem banco de dados. Tudo é salvo localmente no navegador de cada pessoa (`localStorage`):

- Cada navegador/dispositivo guarda suas próprias contas e progresso
- Os dados **não são sincronizados** entre dispositivos diferentes
- Limpar os dados do navegador apaga as contas e o progresso salvo
- Não é adequado para dados sensíveis — serve para uso pessoal e prática

## Adicionando questões

As questões ficam no array `QUESTIONS`, dentro da tag `<script>` do `index.html`. Para adicionar novas, siga o formato comentado no início do array (campos `subject`, `text`, `options`, `correct`, `explanation`, etc).

## Tecnologias

HTML, CSS e JavaScript puro — sem frameworks, sem build, sem dependências de servidor.

## Como publicar no GitHub Pages

Se você baixou estes arquivos e quer publicar seu próprio link:

```bash
# dentro da pasta com index.html, README.md e .gitignore
git init
git add .
git commit -m "Primeira versão do risco·certo"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git
git push -u origin main
```

Depois, no site do GitHub:
1. Abra o repositório → **Settings**
2. No menu lateral, clique em **Pages**
3. Em "Build and deployment" → **Source**, selecione **Deploy from a branch**
4. Em "Branch", escolha **main** e a pasta **/ (root)** → clique em **Save**
5. Aguarde 1–2 minutos. O link aparece no topo dessa mesma página, no formato `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`

Pronto — qualquer pessoa com esse link já pode criar conta e usar o app.
