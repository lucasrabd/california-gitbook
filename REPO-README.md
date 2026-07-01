# 📖 California Roleplay — GitBook

Repositório de documentação oficial do servidor **California Roleplay** (FiveM, heavy roleplay), sincronizado com o GitBook via **GitHub Sync**.

---

## 🗂️ Estrutura

```
california-gitbook-main/
├── README.md                                  # Página inicial do GitBook ("Bem vindo(a)")
├── SUMMARY.md                                    # Índice / árvore de navegação do GitBook
├── regras/
│   ├── README.md                                  # Seção "Regras" (overview)
│   └── regras-gerais.md                             # Regras gerais do servidor
├── legal-faction/
│   ├── README.md                                  # Seção "Legal Faction" (overview)
│   └── informacoes-legal-faction.md                 # Diretrizes de RP para facções legais (LSPD, etc.)
├── ilegal-faction/
│   ├── README.md                                  # Seção "Ilegal Faction" (overview)
│   └── informacoes-de-faccoes-ilegais.md             # Regras para criação/gestão de facções ilegais
└── .gitbook/assets/                              # Imagens e covers usados nas páginas
```

---

## 📚 Conteúdo documentado

| Seção | Descrição |
|---|---|
| **Bem vindo(a)** | Lore, proposta e ambientação do servidor (Califórnia sobre o mapa do GTA V) |
| **Regras** | Regras gerais de convivência e conduta da comunidade |
| **Legal Faction** | Diretrizes de roleplay para instituições oficiais (polícia, órgãos públicos) — foco em procedimento, investigação e realismo |
| **Ilegal Faction** | Regras para criação e gestão de facções ilegais (requisitos mínimos de membros, território, fornecedores, IFM) |

A navegação completa entre as páginas é definida em [`SUMMARY.md`](SUMMARY.md).

---

## ✍️ Convenções de edição

Cada página GitBook usa **YAML front matter** no topo do arquivo para metadados de exibição:

```yaml
---
description: Texto curto exibido abaixo do título
icon: nome-do-icone       # ícone do GitBook (ex: scroll, gun, scale-balanced)
cover: .gitbook/assets/arquivo.png   # imagem de capa (opcional)
coverY: 36.14                          # posição vertical da capa
layout:
  width: default
  cover: { visible: true, size: full }
  tableOfContents: { visible: true }
---
```

Blocos de destaque usam a sintaxe própria do GitBook:

```
{% hint style="info" icon="cloud-check" %}
Conteúdo do aviso.
{% endhint %}
```

Imagens usam a tag `<figure>`:

```html
<figure><img src="../.gitbook/assets/arquivo.png" alt=""><figcaption></figcaption></figure>
```

---

## 🔄 Workflow

1. Editar os arquivos `.md` diretamente neste repositório (ou pelo editor do GitBook, que sincroniza de volta via GitHub Sync).
2. Ao criar uma nova página, adicionar a entrada correspondente em `SUMMARY.md` para que ela apareça na navegação.
3. Imagens novas vão em `.gitbook/assets/` e são referenciadas com caminho relativo (`../.gitbook/assets/nome.png`).
4. Commits na branch sincronizada disparam a atualização automática do site GitBook.

---

## 🔗 Compliance

Documentação sob pesquisa de conformidade quanto ao uso de marcas e referências do mundo real, no contexto da **Cfx.re Platform License Agreement (PLA)** aplicável a servidores FiveM.
