# ✝ Desafio Católico Diário

Página web simples, pensada para celular, que sorteia um **desafio católico por dia**: rezar um terço, fazer uma boa ação, ler o Evangelho, visitar o Santíssimo e muitos outros.

🔗 **Acesse:** https://SEU-USUARIO.github.io/desafio-catolico/

## Funcionalidades

- **Desafio do dia:** todos recebem o mesmo desafio no mesmo dia, e ele muda à meia-noite.
- **Parabéns ao cumprir:** ao marcar o desafio como cumprido, aparece uma mensagem de parabéns.
- **Novo desafio:** depois de cumprir, a pessoa pode pedir outro desafio, se quiser ir além.
- **Sequência e total:** mostra quantos dias seguidos a pessoa cumpriu e quantos desafios fez no total. Esses dados ficam salvos só no navegador de cada pessoa.
- **Copiar desafio:** copia o texto para compartilhar no WhatsApp ou nas redes.
- **Mais de 130 desafios** em 8 categorias: Oração, Palavra de Deus, Caridade, Sacrifício, Sacramentos e Igreja, Maria e os santos, Família e gratidão, e Virtude.
- **Tema claro e escuro**, que segue a configuração do celular.

## Estrutura

```
desafio-catolico/
├── index.html   # a página inteira (HTML, CSS e JavaScript)
└── README.md    # este arquivo
```

O projeto não depende de nada além do navegador e não tem build nem dependências.

## Como publicar no GitHub Pages

1. Crie um repositório **público** no GitHub, por exemplo `desafio-catolico`.
2. Envie o `index.html` e este `README.md` (**Add file → Upload files → Commit changes**).
3. Vá em **Settings → Pages**.
4. Em *Source*, escolha **Deploy from a branch**, depois a branch **main** e a pasta **/ (root)**, e clique em **Save**.
5. Em 1 a 2 minutos, o site estará no ar em `https://SEU-USUARIO.github.io/desafio-catolico/`.

## Como atualizar

**Pelo site:** envie o novo `index.html` com o mesmo nome em **Add file → Upload files**. Ele substitui o antigo.

**Pelo terminal:**

```bash
git add index.html README.md
git commit -m "Descrição da mudança"
git push
```

O site atualiza sozinho em poucos minutos. Se não mudar, recarregue a página no celular.

## Como adicionar novos desafios

No `index.html`, procure a lista `const D=[` e acrescente uma linha no formato:

```js
["o","Texto do novo desafio."],
```

A primeira letra indica a categoria:

| Letra | Categoria            |
|-------|----------------------|
| `o`   | Oração               |
| `p`   | Palavra de Deus      |
| `c`   | Caridade             |
| `s`   | Sacrifício           |
| `i`   | Sacramentos e Igreja |
| `m`   | Maria e os santos    |
| `f`   | Família e gratidão   |
| `v`   | Virtude              |

Não esqueça a vírgula no final de cada linha.

---

*Ad maiorem Dei gloriam*, tudo para a maior glória de Deus.
