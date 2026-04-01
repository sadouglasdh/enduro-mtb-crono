# 🚵 Enduro MTB — Sistema de Cronometragem

Sistema de cronometragem profissional para competições de Enduro MTB.
Dois apps separados para tablet de Largada e tablet de Chegada.

## 🌐 Acesso Online

- **Página inicial:** `https://SEU-USUARIO.github.io/enduro-mtb-crono/`
- **Largada:** `https://SEU-USUARIO.github.io/enduro-mtb-crono/largada.html`
- **Chegada:** `https://SEU-USUARIO.github.io/enduro-mtb-crono/chegada.html`

## 📁 Arquivos

| Arquivo | Descrição |
|---|---|
| `index.html` | Página inicial com links para os dois apps |
| `largada.html` | App do tablet de Largada |
| `chegada.html` | App do tablet de Chegada |

## 🚀 Como publicar no GitHub Pages

1. Crie o repositório `enduro-mtb-crono` no GitHub
2. Faça upload dos 3 arquivos HTML
3. Vá em **Settings → Pages → Source → Deploy from branch → main**
4. Aguarde 1-2 minutos e acesse a URL gerada

## 📱 Como transformar em APK

1. Acesse **webintoapp.com**
2. Cole a URL do app (largada ou chegada)
3. Configure nome, ícone e cor
4. Baixe o `.apk` e instale no tablet Android
5. https://www.webintoapp.com/author/apps/1233584/edit

## 📋 Formato da Startlist CSV

```
numero,nome,categoria,genero,especial,ordem,hora_largada
1,Carlos Ferreira,Elite,M,Especial 1,1,09:00:00
1,Carlos Ferreira,Elite,M,Especial 2,1,10:00:00
2,Ana Paula Gomes,Elite,F,Especial 1,2,09:01:00
```

## 🔄 Fluxo do Evento

1. **Ambos os tablets** importam a mesma Startlist CSV
2. **Largada:** registra pilotos → encerra especial → gera `largada_Especial1.json`
3. **Chegada:** registra chegadas → encerra especial → gera `chegada_Especial1.json`
4. **Resultado Final** (aba no app de Largada): importa largada + chegada por especial → calcula → exporta PDF
