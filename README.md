# Bancos Brasileiros

Listagem de bancos comerciais brasileiros

[![Build status](https://ci.appveyor.com/api/projects/status/f9sx7ux82epp8bd6?svg=true)](https://ci.appveyor.com/project/guibranco/bancosbrasileiros)
[![GitHub last commit](https://img.shields.io/github/last-commit/guibranco/BancosBrasileiros)](https://wakatime.com/badge/github/guibranco/BancosBrasileiros)
[![GitHub license](https://img.shields.io/github/license/guibranco/BancosBrasileiros)](https://wakatime.com/badge/github/guibranco/BancosBrasileiros)
[![GitHub issues by-label](https://img.shields.io/github/issues/guibranco/BancosBrasileiros/help%20wanted.svg)](https://github.com/guibranco/BancosBrasileiros/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
[![time tracker](https://wakatime.com/badge/github/guibranco/BancosBrasileiros.svg)](https://wakatime.com/badge/github/guibranco/BancosBrasileiros)

***For a english version of README.md, please [follow me](/README.en.md)***

---

## Lista de bancos

### Formatos

Esta lista contém 259 bancos cadastrados, nos seguintes formatos:

- **CSV**: [bancos.csv](/data/bancos.csv)
- **JSON**: [bancos.json](/data/bancos.json)
- **Markdown**: [bancos.md](/data/bancos.md)
- **SQL**: [bancos.sql](/data/bancos.sql)
- **XML**: [bancos.xml](/data/bancos.xml)

### Dados disponíves

Cada uma das listas possui as seguintes informações (schema):

| Coluna | Descrição | Observações |
|-------------------|:---------------------------------------:|:--------------------------------------------------------------------------:|
| COMPE | Código do banco - COMPE | 3 dígitos |
| ISPB | Código do banco - ISPB | 8 dígitos |
| Document | Documento do banco - CNPJ | 14 números - 18 dígitos (formatado) |
| FiscalName | Razão social do banco | Conforme Receita Federal do Brasil |
| FantasyName | Nome fantasia do banco | Nome comercial/popular |
| Network | Rede a qual o banco faz parte | RSFN; internet; null |
| Type | Tipo de banco | comercial; múltiplo; caixa econômica; null |
| Url | Url do website | - |
| DateOperationStarted | Data do início de operação do banco | - |
| DateRegistered | Data de cadastro no schema | - |
| DateUpdated | Data de alteração no schema | - |
| DateRemoved | Data de exclusão no schema | [Exclusão lógica](https://pt.stackoverflow.com/questions/10304/exclus%C3%A3o-f%C3%ADsica-vs-exclus%C3%A3o-l%C3%B3gica) |
| IsRemoved | Flag indicativa se este banco foi removido ou não | [Exclusão lógica](https://pt.stackoverflow.com/questions/10304/exclus%C3%A3o-f%C3%ADsica-vs-exclus%C3%A3o-l%C3%B3gica) |

---

## Schemas e classes

Um arquivo de schema está disponível na pasta [schemas](/schemas) para as listas do tipo:

- [JSON](/schemas/schema.json)
- [SQL](/schemas/schema.sql)
- [XML](/schemas/schema.xml)

E classes (DTO - Data Transport Object) das seguintes linguagens:

- [C#](/schemas/csharp.cs)
- [Go](/schemas/go.go)
- [Java](/schemas/java.java)
- [JavaScript](/schemas/javascript.js)
- [Kotlin](/schemas/kotlin.kt)
- [PHP](/schemas/php.php)
- [Python](/schemas/python.py)
- [Rust](/schemas/rust.rs)
- [TypeScript](/schemas/typescript.ts)

---

## NPM - Node Package Manager

[![npm](https://img.shields.io/npm/v/bancos-brasileiros)](https://www.npmjs.com/package/bancos-brasileiros)
[![npm](https://img.shields.io/npm/dy/bancos-brasileiros)](https://www.npmjs.com/package/bancos-brasileiros)

Este repositório está disponível no NPM com o nome [bancos-brasileiros](https://www.npmjs.com/package/bancos-brasileiros).
Um agradecimento ao [@RauppRafael](https://github.com/RauppRafael) por ter idealizado e criado a versão 1.0.0 no NPM.

```bash

npm i bancos-brasileiros

```

---

## Siglas e abreviações

Para aqueles que não estão familiarizados com entidades brasileiras:

- **ABBC** - Associação Brasileira de Bancos
- **BCB** - Banco Central do Brasil (autoridade reguladora) (também chamado de Bacen ou BC)
- **CIP** - Câmara Interbancária de Pagamentos
- **CNPJ** - Cadastro Nacional de Pessoa Jurídica - RFB
- **COMPE** - Sistema de Compensação de Cheques e Outros Papéis
- **CPF** - Cadastro Pessoa Física - RFB
- **FEBRABAN** - Federação Brasileira de Bancos
- **ISPB** - Identificação do SPB
- **PIX** - Pagamentos Instantâneos
- **RFB** - Receita Federal do Brasil
- **RSFN** - Rede do SFN
- **SFN** - Sistema Financeiro Nacional
- **SPB** - Sistema de Pagamentos Brasileiro
- **SPI** - Sistema de Pagamentos Instantâneos
- **STR** - Sistema de Transferência de Reserva

---

## Changelog

- 2021-04-27: [Issue #45](http://github.com/guibranco/BancosBrasileiros/issues/45) - Adicionado schemas/classes - [@guibranco](https://github.com/guibranco)
- 2021-04-27: [Issue #44](http://github.com/guibranco/BancosBrasileiros/issues/44) - Adicionado lista Markdown - [@guibranco](https://github.com/guibranco)
- 2021-04-27: [Issue #42](http://github.com/guibranco/BancosBrasileiros/issues/42) - Código COMPE no arquivo Bancos.sql convertido de integer para string/varchar - [@silverio27](https://github.com/silverio27)
- 2021-04-27: [Issue #36](http://github.com/guibranco/BancosBrasileiros/issues/36) - Listas normalizadas (dados e estrutura) - [@guibranco](https://github.com/guibranco)
- 2021-04-27: [Issue #31](http://github.com/guibranco/BancosBrasileiros/issues/31) - Adicionado ISP nas listas - [@guibranco](https://github.com/guibranco)
- 2021-04-27: [Issue #9](http://github.com/guibranco/BancosBrasileiros/issues/9) - Adicionado sites nas listas - [@guibranco](https://github.com/guibranco)
- 2021-04-27: [Issue #4](http://github.com/guibranco/BancosBrasileiros/issues/4) - Adicionado CNPJ nas listas - [@guibranco](https://github.com/guibranco)
- 2021-01-20: [Issue #53](http://github.com/guibranco/BancosBrasileiros/issues/53) - Adicionado Digio (COMPE: 335 / ISPB: 27098060) - [@gslvrp](https://github.com/gslvrp)
- 2021-01-06: [Issue #51](http://github.com/guibranco/BancosBrasileiros/issues/51) - Adicionado PicPay (COMPE: 380 / ISPB: 22896431) - [@kingaspx](https://github.com/kingaspx)
- 2020-06-18: [Issue #46](http://github.com/guibranco/BancosBrasileiros/issues/46) - Corrige dados do Santander (033 e 502) - [@raframil](https://github.com/raframil)
- 2020-05-12: [Issue #41](http://github.com/guibranco/BancosBrasileiros/issues/41) - Corrige data de atualização do Banco Neon - [@silverio27](https://github.com/silverio27)
- 2020-05-12: [Issue #41](http://github.com/guibranco/BancosBrasileiros/issues/41) - Corrigido data de atualização do Banco Neon - [@silverio27](https://github.com/silverio27)
- 2020-04-29: [Issue #40](http://github.com/guibranco/BancosBrasileiros/issues/40) - Corrigido nome do Banco Inter - [@iurisilvio](https://github.com/iurisilvio)
- 2020-04-28: Removido vírgula em excesso no arquivo bancos.json - [@wesleydeveloper](https://github.com/wesleydeveloper)
- 2020-04-24: [Issue #35](https://github.com/guibranco/BancosBrasileiros/issues/35) - Adicionado Stone Pagamentos S.A. - [@lucastorress](https://github.com/lucastorress)
- 2020-04-23: [Issue #34](https://github.com/guibranco/BancosBrasileiros/issues/34) - Publicação automática do pacote NPM - [@guibranco](https://github.com/guibranco)
- 2020-04-23: [Issue #32](https://github.com/guibranco/BancosBrasileiros/issues/32) - Corrigido dados do Banco Órama em bancos.sql - [@VGsss](https://github.com/VGsss)
- 2020-04-23: [Issue #33](https://github.com/guibranco/BancosBrasileiros/issues/33) - Corrigido dados do RaboBank - [@rpenha](https://github.com/rpenha)
- 2020-04-17: Atualização do readme.md e do readme.en.md, publicação do github.io pages
- 2020-04-15: [Issue #30](https://github.com/guibranco/BancosBrasileiros/issues/30) - Adicionado package.json para pacote NPM - [@RauppRafael](https://github.com/RauppRafael)
- 2020-04-15: Adicionado badges - [@guibranco](https://github.com/guibranco)
- 2020-03-20: [Issue #25](https://github.com/guibranco/BancosBrasileiros/issues/25) - Corrigido acentuação do Banco de Brasília - [@luisccf](https://github.com/luisccf)
- 2020-03-20: [Issue #28](https://github.com/guibranco/BancosBrasileiros/issues/28) - Adicionado Banco Brasil Plural - [@lucastorress](https://github.com/lucastorress)
- 2020-03-20: [Issue #27](https://github.com/guibranco/BancosBrasileiros/issues/27) - Adicionado Cooperativa Central de Crédito - AILOS - [@olvsamuel](https://github.com/olvsamuel)
- 2020-03-20: [Issue #29](https://github.com/guibranco/BancosBrasileiros/issues/29) - Adicionado coluna "UpdatedAt" em bancos.sql - [@guibranco](https://github.com/guibranco)
- 2020-03-20: [Issue #22](https://github.com/guibranco/BancosBrasileiros/issues/22) - Adicionado Banco Máxima - [@guibranco](https://github.com/guibranco)
- 2020-02-19: [Issue #23](https://github.com/guibranco/BancosBrasileiros/issues/23) - Corrigido dados do NuBank - [@rodrigondec](https://github.com/rodrigondec)
- 2020-01-15: [Issue #21](https://github.com/guibranco/BancosBrasileiros/issues/21) - Adicionado Órama DTVM S.A. - [@guibranco](https://github.com/guibranco)
- 2019-12-26: [Issue #19](https://github.com/guibranco/BancosBrasileiros/issues/19) - Adicionado Acesso Soluções e Pagamento S.A. - [@baldini](https://github.com/Baldini)
- 2019-11-12: [Issue #17](https://github.com/guibranco/BancosBrasileiros/issues/17) - Adicionado coluna IsDeleted no arquivo .sql - [@guibranco](https://github.com/guibranco)
- 2019-11-12: [Issue #16](https://github.com/guibranco/BancosBrasileiros/issues/16) - Substituido Banco Potencial pelo Neon. Removido banco Neon - [@RauppAndPony](https://github.com/RauppAndPony)
- 2019-08-02: [Issue #11](https://github.com/guibranco/BancosBrasileiros/issues/11) - Adicionado Banco C6 - [@guibranco](https://github.com/guibranco)
- 2019-05-21: [Issue #10](https://github.com/guibranco/BancosBrasileiros/issues/10) - Adicionado versão inglês do **README.md** - [@guibranco](https://github.com/guibranco)
- 2019-05-21: [Issue #5](https://github.com/guibranco/BancosBrasileiros/issues/5) e [Issue #6](https://github.com/guibranco/BancosBrasileiros/issues/6) - Adicionado listas **CSV** e **XML** dos dados - [@guibranco](https://github.com/guibranco)
- 2019-05-21: [Issue #8](https://github.com/guibranco/BancosBrasileiros/issues/8) - Adicionado Banco BS2 - [@guibranco](https://github.com/guibranco)
- 2019-04-03: [PR #7](https://github.com/guibranco/BancosBrasileiros/pull/7) - Corrigido nome do Bradesco em bancos.json - [@jesobreira](https://github.com/jesobreira)
- 2019-01-15: [Issue #3](https://github.com/guibranco/BancosBrasileiros/issues/3) - Adicionado Banco Inter em bancos.sql - [@diegolourenco](https://github.com/DiegoLourenco)
- 2019-01-15: Renomeado arquivos para **bancos.formato** - [@guibranco](https://github.com/guibranco)
- 2018-01-28: Adicionado formato **JSON** - [@raphaelcunha](https://github.com/raphaelcunha)
- 2018-01-28: Adicionado XP Investimentos e NuBank - [@raphaelcunha](https://github.com/raphaelcunha)
- 2017-10-26: Adicionado 248 bancos no formato **T-SQL** - [@guibranco](https://github.com/guibranco)
