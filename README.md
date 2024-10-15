# nvim

## Install

En caso de fallo de los plugins de nvim, buscar en github o en google el nombre del plugins y coger la config correcta

1) Instalar neovim
2) Instalar  to [Vim-Plug](https://github.com/junegunn/vim-plug#neovim) to neovim
3) Copiar fichero init.vim (donde se van poner los plugins y las configuraciones)
   en /home/$USER/.config/nvim/init.vim
4) Abre `nvim` y escribe `:PlugUpdate`  para instalar y actualizar los plugins, y `:PlugUpgrade` para actualizar el propio gestor `vim-plug`
5) Instalar [zsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)
6) Instalar [ohmyzsh](https://ohmyz.sh/#install)
7) Instalar [fzf search](https://github.com/joshskidmore/zsh-fzf-history-search)
8) Instalar esta [fuente](https://github.com/romkatv/powerlevel10k#manual-font-installation)
9) Pegar el fichero `init.vim` en _.config/nvim/init.vim_
10) Instala [bat](https://github.com/sharkdp/bat)
11) Install `zoxide`
12) Install `the_silver_searcher`
13) [Install](https://releases.hashicorp.com/terraform-ls/) [terraform-ls](https://github.com/hashicorp/terraform-ls/blob/main/docs/installation.md) only download de binary and put in `/usr/local/bin/`. And execute in nvim `:CocConfig`  and       paste the [next](https://github.com/hashicorp/terraform-ls/blob/main/docs/USAGE.md#vim--neovim):

```bash
{
	"languageserver": {
		"terraform": {
			"command": "terraform-ls",
			"args": ["serve"],
			"filetypes": [
				"terraform",
				"tf"
			],
			"initializationOptions": {},
			"settings": {}
		}
	}
}
```
14) Instalar yarn
15) Create folder "~/.local/share/nvim/site/autoload/airline/themes" and paste the file "tokyonight.vim"

## Shortcuts and tricks

Color Html (night): `#1A1B26`/32" # Ip's de cliente pedidas por Antonio

### Comentar
Para comentar y descomentar una linea  `gcc`
Para comentar y descomentar un bloque  `gc`

### NerdTree
    t: Open the selected file in a new tab
    i: Open the selected file in a horizontal split window
    s: Open the selected file in a vertical split window
    I: Toggle hidden files
    m: Show the NERD Tree menu
    R: Refresh the tree, useful if files change outside of Vim
    ?: Toggle NERD Tree's quick help

### fzf.vim
`Ctrl + p`  -> Buscar nombre de fichero.
`Ctrl + f`  -> Buscar dentro de los ficheros.

**Ctrl+T**, **Ctrl+X**, or **Ctrl+V** to open the file in a new tab, split, or vertical split,

### Coc + Terraform
```
Ctrl + space = mostrar propiedades de un recurso.
gd = ir a la declaración del recurso.
```

### Cambiar entre pestañas de vim

```
Next tab: gt
Prior tab: gT
Numbered tab: _nnn_gt
```

### Atajos Fn's
`F2` -> NerdTree
`F3` -> Sacar/Ocultar numeros laterales
`F4` -> MarkdowPreview
`F5` -> Mostrar diff
`F12` -> Sacar shell delante de Vim
