# Gerador de Stories da Loteria Federal

**Versão:** 1.0

Gerador automático de stories da Loteria Federal desenvolvido em **HTML**, **CSS** e **JavaScript**, com geração de imagens em **PNG** através da **Canvas API**.

O objetivo do projeto é automatizar completamente a criação de artes para divulgação dos resultados da Loteria Federal, eliminando a necessidade de edição manual em ferramentas de design e reduzindo significativamente o tempo de publicação.

---

# Motivação

A publicação dos resultados da Loteria Federal exigia a criação manual de três artes diferentes para redes sociais.

Além do tempo gasto na edição, o processo estava sujeito a erros de digitação, inconsistências entre layouts e retrabalho.

Este projeto foi desenvolvido para automatizar toda essa etapa, permitindo gerar todas as artes a partir de um único preenchimento dos resultados.

---

# Funcionalidades

* Atualização automática dos stories em tempo real
* Geração simultânea dos layouts de 5, 6 e 7 dígitos
* Exportação das artes em formato PNG
* Persistência automática dos dados utilizando LocalStorage
* Preenchimento automático da data atual
* Máscara automática para o campo de data
* Aceita apenas números nos campos dos prêmios
* Validação de campos obrigatórios
* Validação de premiações contendo exatamente cinco dígitos
* Interface simples, rápida e totalmente executada no navegador

---

# Stories gerados

O sistema gera automaticamente três arquivos:

* **5digitos.png**
* **6digitos.png**
* **7digitos.png**

Todos os arquivos são produzidos em alta resolução e prontos para publicação.

---

# Regras de geração

## Story de 5 dígitos

### Destaque dos prêmios

**1º prêmio**

* 2 primeiros dígitos em branco
* 3 últimos dígitos em laranja

**2º prêmio**

* 2 primeiros dígitos em branco
* 2 dígitos centrais em laranja
* último dígito em branco

**3º, 4º e 5º prêmio**

* totalmente em branco

### Número sorteado

Últimos 3 dígitos do 1º prêmio + 2 dígitos centrais do 2º prêmio.

---

## Story de 6 dígitos

### Destaque dos prêmios

**1º prêmio**

* 2 primeiros dígitos em branco
* 3 últimos dígitos em laranja

**2º prêmio**

* 2 primeiros dígitos em branco
* 3 últimos dígitos em laranja

**3º ao 5º prêmio**

* totalmente em branco

### Número sorteado

Últimos 3 dígitos do 1º prêmio + últimos 3 dígitos do 2º prêmio.

Formato:

```
XXX.XXX
```

---

## Story de 7 dígitos

### Destaque dos prêmios

**1º prêmio**

* 2 primeiros dígitos em branco
* 3 últimos dígitos em laranja

**2º prêmio**

* 2 primeiros dígitos em branco
* 3 últimos dígitos em laranja

**3º prêmio**

* 2 primeiros dígitos em branco
* dígito central em laranja
* 2 últimos dígitos em branco

**4º e 5º prêmio**

* totalmente em branco

### Número sorteado

Últimos 3 dígitos do 1º prêmio + últimos 3 dígitos do 2º prêmio + dígito central do 3º prêmio.

Formato:

```
X.XXX.XXX
```

---

# Tecnologias utilizadas

* HTML5
* CSS3
* JavaScript
* Canvas API
* LocalStorage

---

# Estrutura do projeto

```
gerador-stories/
│
├── index.html
├── style.css
├── script.js
└── README.md
```

Os fundos utilizados pelos stories são carregados diretamente através do GitHub Pages.

---

# Como utilizar

1. Abra o arquivo `index.html`.
2. Informe a data do sorteio.
3. Informe a extração.
4. Preencha os cinco prêmios na ordem em que são anunciados na transmissão oficial.
5. Clique em **DOWNLOAD**.
6. Os três arquivos PNG serão gerados automaticamente.

---

# Recursos implementados

* Atualização em tempo real
* Canvas API
* Download automático dos três stories
* Persistência com LocalStorage
* Data automática
* Máscara para data
* Validação dos campos
* Validação dos prêmios
* Interface limpa
* Geração totalmente offline

---

# Dependências

O projeto **não utiliza**:

* Node.js
* Electron
* Frameworks JavaScript
* Bibliotecas externas para captura de tela
* Banco de dados
* Servidor local

Basta abrir o arquivo **index.html** em um navegador moderno para utilizar a aplicação.

---

# Autor

**Matheus Rodrigues Lopes**

Analista de Tecnologia da Informação

Projeto desenvolvido para automatizar a geração de stories da Loteria Federal, reduzindo tempo operacional, eliminando tarefas repetitivas e garantindo padronização na publicação dos resultados.
