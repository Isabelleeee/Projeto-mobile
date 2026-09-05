# HABIT — Protótipo Mobile

![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![BEM](https://img.shields.io/badge/BEM-block%5F%5Felement----modifier-6B6B6B?style=flat-square)
![React](https://img.shields.io/badge/React-pr%C3%B3xima%20etapa-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Entrega](https://img.shields.io/badge/entrega-07%2F09%2F2026-1F7A6D?style=flat-square)

Wireframes mobile em baixa fidelidade e organização dos estilos CSS com BEM — base para a implementação em React. Disciplina de Desenvolvimento Mobile.

## Integrantes

| | Nome |
|---|---|
| ![Isa](https://img.shields.io/badge/Isa-1F7A6D?style=flat-square) | Isabelle Lopes |
| ![Murilo](https://img.shields.io/badge/Murilo-3C5FA8?style=flat-square) | Murilo Rocha |
| ![Artur](https://img.shields.io/badge/Artur-B4700F?style=flat-square) | Artur Sudre |

## Descrição da aplicação

HABIT é uma plataforma de publicação de conteúdo organizada por categorias. A área pública permite navegar por categorias, destaques e escolhas do editor, buscar postagens e assinar a newsletter. Usuários autenticados têm perfil próprio com suas postagens e comentários. A área administrativa cobre categorias, criação e revisão de postagens, escolhas do editor, usuários e moderação de comentários.

Esta etapa contém as 14 telas mobile em baixa fidelidade, a identificação dos componentes recorrentes e a estrutura inicial dos estilos CSS no padrão BEM, que servirá de base para a implementação em React.

## Telas

Protótipo no Figma: _link_

| Tela | Nome | Fluxo | Quem | Arquivo |
|---|---|---|---|---|
| tela_01 | Início | público | ![Isa](https://img.shields.io/badge/Isa-1F7A6D?style=flat-square) | [tela_01_inicio.png](projeto-mobile/wireframes/tela_01_inicio.png) |
| tela_02 | Categoria | público | ![Isa](https://img.shields.io/badge/Isa-1F7A6D?style=flat-square) | [tela_02_categoria.png](projeto-mobile/wireframes/tela_02_categoria.png) |
| tela_03 | Destaques | público | ![Isa](https://img.shields.io/badge/Isa-1F7A6D?style=flat-square) | [tela_03_destaques.png](projeto-mobile/wireframes/tela_03_destaques.png) |
| tela_04 | Assinar newsletter | público | ![Murilo](https://img.shields.io/badge/Murilo-3C5FA8?style=flat-square) | [tela_04_newsletter.png](projeto-mobile/wireframes/tela_04_newsletter.png) |
| tela_05 | Admin · Categorias | admin | ![Artur](https://img.shields.io/badge/Artur-B4700F?style=flat-square) | [tela_05_admin_categorias.png](projeto-mobile/wireframes/tela_05_admin_categorias.png) |
| tela_06 | Admin · Criar post | admin | ![Artur](https://img.shields.io/badge/Artur-B4700F?style=flat-square) | [tela_06_admin_criar_post.png](projeto-mobile/wireframes/tela_06_admin_criar_post.png) |
| tela_07 | Admin · Escolhas do editor | admin | ![Artur](https://img.shields.io/badge/Artur-B4700F?style=flat-square) | [tela_07_admin_escolhas_editor.png](projeto-mobile/wireframes/tela_07_admin_escolhas_editor.png) |
| tela_08 | Admin · Usuários | admin | ![Artur](https://img.shields.io/badge/Artur-B4700F?style=flat-square) | [tela_08_admin_usuarios.png](projeto-mobile/wireframes/tela_08_admin_usuarios.png) |
| tela_09 | Admin · Fila de revisão | admin | ![Artur](https://img.shields.io/badge/Artur-B4700F?style=flat-square) | [tela_09_admin_fila_revisao.png](projeto-mobile/wireframes/tela_09_admin_fila_revisao.png) |
| tela_10 | Admin · Fila de comentários | admin | ![Artur](https://img.shields.io/badge/Artur-B4700F?style=flat-square) | [tela_10_admin_fila_comentarios.png](projeto-mobile/wireframes/tela_10_admin_fila_comentarios.png) |
| tela_11 | Resultado da busca | público | ![Isa](https://img.shields.io/badge/Isa-1F7A6D?style=flat-square) | [tela_11_busca.png](projeto-mobile/wireframes/tela_11_busca.png) |
| tela_12 | Entrar | autenticação | ![Murilo](https://img.shields.io/badge/Murilo-3C5FA8?style=flat-square) | [tela_12_entrar.png](projeto-mobile/wireframes/tela_12_entrar.png) |
| tela_13 | Criar conta | autenticação | ![Murilo](https://img.shields.io/badge/Murilo-3C5FA8?style=flat-square) | [tela_13_criar_conta.png](projeto-mobile/wireframes/tela_13_criar_conta.png) |
| tela_14 | Perfil | autenticação | ![Murilo](https://img.shields.io/badge/Murilo-3C5FA8?style=flat-square) | [tela_14_perfil.png](projeto-mobile/wireframes/tela_14_perfil.png) |

Fluxos: público (01 → 02 / 03 / 04 / 11), autenticação (12 → 13 → 14), administrativo (05–10). Fluxo de publicação: tela_06 → tela_09 → aprovação → publicação.

## Componentes identificados

Cada linha é um bloco BEM com arquivo próprio em `css/`. "Onde aparece" usa o número da tela.

| Componente | Arquivo | Onde aparece | Variações | Quem |
|---|---|---|---|---|
| `header` | `navigation.css` | todas | — | ![Isa](https://img.shields.io/badge/Isa-1F7A6D?style=flat-square) |
| `nav` | `navigation.css` | 01, 02, 03, 04, 11, 12, 13, 14 | `--active`, `__drawer` | ![Isa](https://img.shields.io/badge/Isa-1F7A6D?style=flat-square) |
| `footer` | `navigation.css` | todas | — | ![Isa](https://img.shields.io/badge/Isa-1F7A6D?style=flat-square) |
| `section` | `layout.css` | 01, 02, 03, 05–10, 11, 14 | — | ![Isa](https://img.shields.io/badge/Isa-1F7A6D?style=flat-square) |
| `button` | `button.css` | todas | `--primary`, `--secondary`, `--danger`, `--disabled` | ![Isa](https://img.shields.io/badge/Isa-1F7A6D?style=flat-square) |
| `card` | `card.css` | 01, 02, 03, 11 | padrão, `--compact`, `--featured` | ![Isa](https://img.shields.io/badge/Isa-1F7A6D?style=flat-square) |
| `chip` | `chip.css` | 01, 02, footer | `--selected`, `--category` | ![Isa](https://img.shields.io/badge/Isa-1F7A6D?style=flat-square) |
| _componente_ | _arquivo_ | _telas_ | _variações_ | ![Murilo](https://img.shields.io/badge/Murilo-3C5FA8?style=flat-square) |
| _componente_ | _arquivo_ | _telas_ | _variações_ | ![Artur](https://img.shields.io/badge/Artur-B4700F?style=flat-square) |

<!-- Murilo e Artur: adicionem as linhas dos componentes de vocês acima, na ordem em que aparecem nas telas. -->

## Variações previstas

Modificador representa uma variação do bloco inteiro; elemento representa uma parte interna do bloco. Exemplo com os dois componentes de referência do enunciado:

```css
.card { }
.card__title { }
.card__content { }
.card__image { }
.card--featured { }
.card--compact { }

.button { }
.button--primary { }
.button--secondary { }
.button--danger { }
.button--disabled { }
```

Estados de conteúdo (rascunho, publicado, em análise, ativo, bloqueado, em revisão) são modificadores de um mesmo componente de rótulo, definido uma única vez e reutilizado nas telas 08, 09, 10 e 14.

## Organização dos arquivos

```
projeto-mobile/
├── wireframes/        14 telas em PNG, 390×844, nome tela_NN_nome.png
├── css/
│   ├── variables.css  cores, espaçamento, tipografia — único lugar com valores
│   ├── navigation.css header, nav, footer
│   ├── layout.css     section
│   ├── button.css
│   ├── card.css
│   ├── chip.css
│   └── ...            um arquivo por componente, nome igual ao bloco
└── README.md
```

### Convenções

| Regra | Como |
|---|---|
| Nomenclatura | inglês, minúsculas, `bloco__elemento--modificador`, um nível de elemento no máximo |
| Valores | nenhum arquivo além de `variables.css` contém cor ou medida literal — sempre `var(--nome)` |
| Um bloco, um arquivo | o arquivo em `css/` tem o mesmo nome do bloco |
| Commits | direto na `main`, um por tela e um por arquivo CSS, mensagem `tela_05: wireframe categorias` |
| Wireframes | PNG 1x, 390×844, preto/cinza/verde `#1F7A6D`, nome de classe anotado ao lado de cada bloco |

---

<p align="center">
  <sub>Desenvolvimento Mobile · Engenharia da Computação · Mackenzie · 2026</sub>
</p>
