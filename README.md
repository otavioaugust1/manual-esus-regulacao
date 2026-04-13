# Manual e-SUS Regulação

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/otavioaugust1/manual-esus-regulacao/blob/main/LICENSE)
![Jekyll](https://img.shields.io/badge/jekyll-4.4+-red.svg)
![Just the Docs](https://img.shields.io/badge/just--the--docs-0.12.0-blue.svg)
![Status](https://img.shields.io/badge/status-Active-brightgreen.svg)

**Projeto pessoal** com o objetivo de digitalizar e publicar o manual do Sistema **e-SUS Regulação** de forma interativa e acessível.

Documentação desenvolvida com [Jekyll](https://jekyllrb.com/) e o tema [Just the Docs](https://just-the-docs.com/).

## 📖 Sobre Este Repositório

Este repositório é um **espaço colaborativo** para manter atualizado o manual do e-SUS Regulação. Se você encontrou um erro, tem uma sugestão de melhoria ou quer adicionar conteúdo, sinta-se à vontade para contribuir!

## 🚀 Como Começar

### Pré-requisitos

- Ruby >= 2.7 (instalado no seu sistema)
- Git

### 1. Clonar o Repositório

```bash
git clone https://github.com/otavioaugust1/manual-esus-regulacao.git
cd manual-esus-regulacao
```

### 2. Instalar Dependências

```bash
# Opção 1: Jekyll diretamente (mais simples)
sudo gem install jekyll just-the-docs

# Opção 2: Usando Bundler (recomendado para colaboradores)
bundle install
```

### 3. Executar Localmente

```bash
# Com Jekyll direto
jekyll serve

# Com Bundler
bundle exec jekyll serve
```

Acesse: **http://localhost:4000**

### 4. Fazer Build

```bash
jekyll build
```

Os arquivos serão gerados em `_site/`

## 📁 Estrutura do Projeto

```
├── index.md                       # Página inicial
├── _config.yml                    # Configuração do Jekyll
│
├── acesso/                        # Seção de Acesso
│   ├── index.md
│   ├── como-solicitar-acesso.md
│   └── primeiro-acesso.md
│
├── administrador/                 # Seção Administrador
│   ├── index.md
│   ├── criacao-operadores.md
│   ├── cadastro-procedimentos.md
│   └── ...outros arquivos
│
├── regulador/                     # Seção Regulador
│   ├── index.md
│   ├── fila-espera.md
│   └── ...outros arquivos
│
├── solicitante/                   # Seção Solicitante
│   ├── index.md
│   ├── agendar-consulta.md
│   └── ...outros arquivos
│
├── executante/                    # Seção Executante
│   └── index.md
│
├── LGPD/                          # Seção LGPD
│   └── index.md
│
├── imagens/                       # Imagens do manual
├── assets/                        # Estilos e scripts
└── _site/                         # Site gerado (não commitado)
```

## ✏️ Como Contribuir

### Reportar Problemas

1. Verifique se o problema já foi reportado em [Issues](https://github.com/otavioaugust1/manual-esus-regulacao/issues)
2. Abra uma nova issue descrevendo detalhadamente:
   - O que está errado
   - Onde está o problema (qual seção/página)
   - Seu navegador e sistema operacional (se relevante)

### Sugerir Melhorias

Tem uma ideia para melhorar o manual? Abra uma issue com tag de sugestão (`enhancement`)!

### Enviar Contribuições (Pull Request)

1. **Fork** este repositório
2. **Clone** seu fork: `git clone https://github.com/SEU-USUARIO/manual-esus-regulacao.git`
3. **Crie uma branch** para sua feature: `git checkout -b melhoria/sua-melhoria`
4. **Faça suas mudanças** nos arquivos `.md`
5. **Teste** localmente com `jekyll serve`
6. **Commit** suas mudanças: `git commit -m "Descrição clara da mudança"`
7. **Push** para sua branch: `git push origin melhoria/sua-melhoria`
8. **Abra um Pull Request** descrevendo suas mudanças

### Convenções de Código

Siga estas convenções para manter consistência:

| Aspecto | Convenção | Exemplo |
|---------|-----------|---------|
| **Nomes de pasta** | Minúsculas | ❌ `Solicitante/` → ✅ `solicitante/` |
| **Permalinks** | Minúsculas com `/` | ❌ `/Solicitante/` → ✅ `/solicitante/` |
| **Datas** | DD/MM/YYYY | ❌ `04/13/2026` → ✅ `13/04/2026` |
| **Arquivos** | Com hífen, minúsculas | ❌ `Como_Solicitar.md` → ✅ `como-solicitar.md` |

### Editando Conteúdo

Cada página usa YAML frontmatter no início do arquivo:

```yaml
---
layout: default
title: Seu Título
nav_order: 1
has_children: false
permalink: /seu-permalink/
last_modified_date: "13/04/2026"
---

# Seu Título

Conteúdo em Markdown...
```

## 🔧 Desenvolvimento Local

### Estrutura de um Arquivo

```markdown
---
layout: default
title: "Título da Página"
nav_order: 1                    # Ordem no menu (menor = primeiro)
parent: "Título da Seção Pai"   # Se for subpágina
has_children: false             # Se tiver subpáginas
permalink: /seu-path/           # URL da página
last_modified_date: "13/04/2026"
---

# Seu Título

Seu conteúdo aqui em Markdown...

## Subsecção

Mais conteúdo...
```

### Testando Localmente

```bash
# Terminal 1: Servir o site
jekyll serve --incremental

# Terminal 2: Fazer suas edições
# ... editar arquivos .md ...

# O navegador atualiza automaticamente!
```

### Limpando o Build

```bash
# Remove arquivos gerados
rm -rf _site .jekyll-cache
```

## 📚 Referências Úteis

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Just the Docs Theme](https://just-the-docs.com/)
- [Markdown Guide](https://www.markdownguide.org/)
- [GitHub Flavored Markdown](https://docs.github.com/en/get-started/writing-on-github)



### ✅ Dependências
- **Problema**: Gems não encontradas
- **Solução**: Instaladas globalmente (Jekyll + just-the-docs)

---

## 📄 Licença

**MIT License** — Use livremente, comercial ou pessoal. Veja [LICENSE](LICENSE).

---

## 👤 Autor & Contato

**Otávio August**
- 🌐 GitHub: [@otavioaugust1](https://github.com/otavioaugust1)
- 🇧🇷 Brasil
- 📧 Dúvidas? Abra uma [issue](https://github.com/otavioaugust1/manual-esus-regulacao/issues)!

> 📝 Informações do programa serão atualizadas continuamente. Contribuições são bem-vindas!

---

**© 2025** — Ministério da Saúde. Todos os direitos reservados.

