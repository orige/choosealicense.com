# Choose a License Web Site - Brazilian Portuguese

This is a portuguese translated  unofficial version of Choosealicense project by GitHub.
The License and the contributors will be kept.

Access the official repository through [this link](https://github.com/github/choosealicense.com).

# Choose a License Web Site

Como um site de Escolha Sua Própria Aventura, porém menos interessante.

# Introdução

Muitos dos repositórios no GitHub.com não tem uma licença. O GitHub fornece um seletor de licenças, mas se você não sabe nada sobre elas, como você poderia tomar a decisão mais inteligente?

ChooseALicense.com foi projetado para ajudar pessoas a fazer uma decisão esclarecida sobre licenças.

# Metas imediatas

* Sem políticas legais - Não vamos entrar nisso.

* Bem projetado, mas isso não precisa ser dito.

* A página inicial deve ter apenas o suficiente para ajudar 99% das pessoas a tomar uma decisão.  

* Para o 1%, o site irá conter uma lista de licenças comuns para situações e comunidades específicas.

* Não ser abrangente. Parece um objetivo estranho, mas há um "zilhão" (eu contei) de licenças mundo afora. Nós vamos ter que filtra-las e coloca-las em uma pequena lista das que importam.

# Rode Na Sua Máquina

1. `git clone https://github.com/github/choosealicense.com`
2. `cd choosealicense.com`
3. `script/bootstrap`
4. `script/server`
5. Abra [localhost:4000](http://localhost:4000) em seu navegador favorito

# Adicionando uma licença

As licenças estão no diretório `/licenses` como arquivos markdown (`.md`). Cada licença tem uma parte em YAML descrevendo suas propriedades. O corpo do arquivo markdown deve ser o texto da licença. Os campos metadata disponíveis são:

* `title` - O nome da licença
* `layout` - Isto **deve ser** `license`
* `permalink` - A URL absoluta para a licença, começando com `/licenses/`
* `source` - URL para o texto de origem da licença
* `note` - O campo de observação na barra lateral (opcional)
* `how` - Como utilizar a licença, também na barra lateral
* `required`, `permitted`, `forbidden` - uma lista de regradas aplicadas à licença (veja abaixo)
* `filename` - O nome do arquivo a ser criado no GitHub.com quando um repositório for iniciado com esta licença.

As licenças no choosealicense.com são regularmente importadas para o GitHub.com para serem utilizadas como uma lista de licenças disponíveis ao criar um repositório. Quando criamos um repositório, vamos substituir certas strings na licença por variáveis a partir do repositório. Isso pode ser utilizado para criar avisos de direitos autorais mais precisos. As variáveis disponíveis são:

* `[fullname]` - O nome completo ou nome de usuário do dono do repositório

* `[login]` - O nome do proprietário do repositório

* `[email]` - O endereço de email principal do dono do repositório 

* `[project]` - O nome do repositório

* `[description]` - A descrição do repositório

* `[year]` - O ano atual

# Regras 

* Rules (the license's properties) are stored as a bulleted list within the licenses YAML front matter. A full list of rules can be found in the repository's `_config.yml` file. Each rule has a name e.g., `include-copyright`, a human-readable label, e.g., `Copyright inclusion`, and a description `Include the original copyright with the code`. To add a new rule, simply add it to config.yml and reference it in the appropriate license. 

* Regras (as propriedas das licenças) são armazenadas como uma lista de marcadores na parte do YAML. Uma lista com todas essas regras pode ser encontrada no arquivo `_config.yml` no repositório. Cada regra tem um nome, por exemplo: `include-copyright`, uma breve descrição legível, exemplo: `Inclusão de direitos autorais`, e uma descrição `Inclua os direitos autorais originais com o código`. Para adicionar uma nova regra, simplesmente coloque-a no arquivo config.yml e referenci-a na licença conveniente.

# Licença

O conteúdo deste projeto em si está licenciado sob a [Creative Commons Attribution 3.0 license](http://creativecommons.org/licenses/by/3.0/us/deed.en_US), e o código fonte utilizado para formatar e mostrar o conteúdo esta licenciado sob a [licença MIT](http://opensource.org/licenses/mit-license.php). 