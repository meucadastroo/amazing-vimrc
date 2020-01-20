# init.vim para neovim

**Instalacao do neovim em sistemas debian-like:**

`$ sudo apt install neovim`

**Instalacao do init.vim:**

`$ git clone https://github.com/foxx3r/amazing-vimrc`

**Configurando o ambiente:**

`$ mkdir ~/.config/nvim -p`

E por ultimo:

`$ mv amazing-vimrc/* ~/.config/nvim/`

Para instalar os plugins necessarios, voce precisa das seguintes ferramentas instaladas:

```
curl
git
wget
```

# Features:

**1. Compilação automática**

Para salvar e executar/compilar seu projeto aperte `CTRL + G`

**2. REPL integrada**

Para rodar a REPL, use `CTRL + a`

**3. Log de última modificação**

Para adicionar o log de última modificação no seu VIM, adicione `ultima modificação: ` e `Last Change: ` nas 5 primeiras linhas do seu projeto. 

Atenção:

1 - Os seus projetos devem conter os dois comentários, obrigatoriamente, caso contrário, não funcionará.

2 - Eles também devem ter um espaço após o ":".

3 - Fique atento ao "ção", "L" e "C", eles são obrigatórios.

Exemplo:

```rust
// ultima modificação: 
// Last Change: 
fn main() {
    println!("Hello, World!");
}
```

Após isso, salve-o.

**4. Fechamento automático em HTML**

...

**5. Destaque de IP**

...

**6. Changelog automático**

No modo normal do VIM, chame `:call InsertChangelog()` ou `:call InsertHeadBash()` para scripts em bash.

Perceba que ao fazer isso, o nome do Autor será o meu, você poderá mudá-lo no `~/.vimrc` ou `~/.config/nvim/init.vim`, ou então mudá-lo toda vez que executar a função.

**7. Rolar janela alternativa de forma mais amigável**

Após usar `Ctrl-w-n` ou `:split`, você poderá rolar a janela abaixo com `ALT + teclas (up, down)`.

Obs: Ainda não disponivel com `:vsplit`, não suportado com mais de 2 janelas.

**8. Backup de arquivos**

Suponha que você tenha sem querer desligado o computador (ou acabou a luz na cidade inteira) ou então executou sem querer um `kill` no PID do VIM, então você terá o arquivo .script.swap no seu diretório atual com todas as suas alterações salvas.

# Plugins:

**delimitMate** - Auto-fechamento de delimitadores

**ag.vim** - Está deprecated, vou atualizar e colocar o ack.vim, mas simplesmente extende a capacidade do VIM buscar fazendo regex e dar split na tela

**ctrlp.vim** - É um fuzzy de path e buffer bstante leve

**nerdcommenter** - Auto comment

**vim-polyglot** - Um plugin com vários outros plugins e inclui suporte a 200 linguagens na qual o VIM/neovim não tem suporte (ficando 700 no total)

**syntastic** - Analisador sintático completo

**nerdtree** - Um tree path

**vim-numbertoggle** - Um number navigation

**AutoComplPop** - Auto complete

**vim-editorconfig** - Extende as possibilidades de configuração do VIM

**molokai** - Tema de background
