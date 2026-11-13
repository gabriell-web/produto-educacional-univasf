# Produto Educacional · PROFMAT / UNIVASF

Site estático em HTML e CSS com página inicial, página de atividades e visual responsivo em azul e amarelo. Não exige Node.js nem instalação de pacotes.

## Arquivos
| Arquivo | O que editar |
| --- | --- |
| index.html | Textos e cartões da página inicial |
| atividades.html | Atividades, títulos e links |
| style.css | Cores, tamanhos, espaçamento e layout |
| favicon.svg | Ícone da aba (símbolo matemático, não logotipo oficial) |
| pdfs/ | Seus materiais PDF |
| netlify.toml | Pasta publicada pelo Netlify |

Abra index.html no navegador para visualizar. No VS Code, também é possível usar a extensão Live Server.

## Clonar no computador
```sh
git clone https://github.com/gabriell-web/produto-educacional-univasf.git
cd produto-educacional-univasf
code .
```

## Atualizar pelo Git
Antes de começar, com sua pasta sem alterações pendentes:
```sh
git pull --ff-only
```
Edite e salve seus arquivos. Confira e envie:
```sh
git status
git diff
git add index.html atividades.html style.css favicon.svg pdfs
git commit -m "Atualiza materiais e visual do site"
git push
```
Se alterar outros arquivos, inclua seus caminhos no git add. Revise sempre o git status antes do commit.

## Trabalhar em uma alteração separada
```sh
git switch -c melhoria-site
```
Após editar e fazer commit:
```sh
git push -u origin melhoria-site
```
No GitHub, abra um Pull Request para main. Depois de mesclar:
```sh
git switch main
git pull --ff-only
```

## Adicionar materiais
Leia pdfs/README.md. Os PDFs ainda não estão incluídos; os links funcionarão quando você os adicionar com os nomes indicados. Para criar uma quinta atividade, copie um cartão em atividades.html, altere seu título e href para pdfs/atividade05.pdf e atualize a contagem de materiais.

## Netlify
O repositório está preparado para publicação estática: pasta de publicação "." e sem comando de build.
Conecte este repositório ao seu projeto Netlify e escolha a branch main. Depois de conectado, os novos pushes poderão gerar publicações automáticas.
A conexão ao Netlify não é feita apenas pela presença do netlify.toml.

## Identidade Git
Use seu próprio nome e e-mail configurados no Git. O repositório não contém senhas ou tokens.

