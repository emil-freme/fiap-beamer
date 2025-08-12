# Template Beamer FIAP

Este template foi desenvolvido para uso com **Pandoc**, permitindo converter
documentos Markdown (`.md`) em apresentações PDF no formato **Beamer**.

## Requisitos

* **Pandoc** (versão mínima: 3.4)
* Alguma distribuição **LaTeX** (ex.: MiKTeX 24.4 ou TeX Live)

## Uso simples

Para uso básico:

1. Baixe este repositório.
2. Coloque o seu arquivo `.md` na mesma pasta do template.
3. Utilize o comando de conversão (ver seção abaixo).

## Instalação (Linux e outros sistemas não Windows)

> **Atenção:** Esta primeira versão foi criada para distribuições baseadas no
> **TeX Live**. Futuras versões buscarão ser agnósticas em relação à
> distribuição LaTeX utilizada.

1. Clone o repositório.
2. Execute o script de instalação:

```bash sudo python3 install.py ```

Esse script irá copiar os arquivos necessários para a pasta `beamer` da sua
distribuição LaTeX.

3. Atualize o **filename database** do LaTeX:

```bash sudo texhash ```

4. Use o arquivo `exemplo.md` como base para criar sua apresentação.

## Gerando o PDF

Para gerar o PDF a partir do Markdown:

```bash pandoc -t beamer apresentacao.md -o apresentacao.pdf --defaults
defaults.yaml ```

