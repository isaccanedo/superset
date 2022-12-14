<!--
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->

# Superset

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/apache/superset?sort=semver)](https://github.com/apache/superset/tree/latest)
[![Build Status](https://github.com/apache/superset/workflows/Python/badge.svg)](https://github.com/apache/superset/actions)
[![PyPI version](https://badge.fury.io/py/apache-superset.svg)](https://badge.fury.io/py/apache-superset)
[![Coverage Status](https://codecov.io/github/apache/superset/coverage.svg?branch=master)](https://codecov.io/github/apache/superset)
[![PyPI](https://img.shields.io/pypi/pyversions/apache-superset.svg?maxAge=2592000)](https://pypi.python.org/pypi/apache-superset)
[![Get on Slack](https://img.shields.io/badge/slack-join-orange.svg)](https://join.slack.com/t/apache-superset/shared_invite/zt-16jvzmoi8-sI7jKWp~xc2zYRe~NqiY9Q)
[![Documentation](https://img.shields.io/badge/docs-apache.org-blue.svg)](https://superset.apache.org)

<img
  src="https://github.com/apache/superset/raw/master/superset-frontend/src/assets/branding/superset-logo-horiz-apache.png"
  alt="Superset"
  width="500"
/>

Um aplicativo da web de business intelligence moderno e pronto para empresas.

[**Why Superset?**](#why-superset) |
[**Supported Databases**](#supported-databases) |
[**Installation and Configuration**](#installation-and-configuration) |
[**Release Notes**](RELEASING/README.md#release-notes-for-recent-releases) |
[**Get Involved**](#get-involved) |
[**Contributor Guide**](#contributor-guide) |
[**Resources**](#resources) |
[**Organizations Using Superset**](RESOURCES/INTHEWILD.md)

## Porque Superset?

Superset ?? uma plataforma moderna de explora????o e visualiza????o de dados. O Superset pode substituir ou aumentar as ferramentas propriet??rias de intelig??ncia de neg??cios para muitas equipes. O Superset integra-se bem com uma variedade de fontes de dados.

O Superset fornece:

- Uma **interface sem c??digo** para criar gr??ficos rapidamente;
- Um **Editor SQL** poderoso e baseado na Web para consultas avan??adas;
- Uma **camada sem??ntica leve** para definir rapidamente dimens??es e m??tricas personalizadas;
- Suporte pronto para uso para **quase qualquer banco de dados SQL** ou mecanismo de dados;
- Uma ampla variedade de **lindas visualiza????es** para mostrar seus dados, desde simples gr??ficos de barras at?? visualiza????es geoespaciais;
- **camada de cache** leve e configur??vel para ajudar a facilitar a carga do banco de dados;
- Op????es de **fun????es de seguran??a e autentica????o** altamente extens??veis;
- Uma API para personaliza????o program??tica;
- Uma **arquitetura nativa da nuvem** projetada desde o in??cio para escala.

## Capturas de tela e gifs

**Galeria de Visualiza????es**

<kbd><img title="Gallery" src="superset-frontend/src/assets/images/screenshots/gallery.jpg"/></kbd><br/>

**Crie pain??is bonitos e din??micos**

<kbd><img title="View Dashboards" src="superset-frontend/src/assets/images/screenshots/slack_dash.jpg"/></kbd><br/>

**Construtor de gr??ficos sem c??digo**

<kbd><img title="Slice & dice your data" src="superset-frontend/src/assets/images/screenshots/explore.jpg"/></kbd><br/>

**Poderoso Editor SQL**

<kbd><img title="SQL Lab" src="superset-frontend/src/assets/images/screenshots/sql_lab.jpg"/></kbd><br/>

## Bancos de dados compat??veis

O Superset pode consultar dados de qualquer armazenamento de dados ou mecanismo de dados que fale SQL (Presto, Trino, Athena, [e mais](https://superset.apache.org/docs/databases/installing-database-drivers/)) que tenha um driver Python DB-API e um dialeto SQLAlchemy.

Aqui est??o algumas das principais solu????es de banco de dados que s??o suportadas:

<p align="center">
  <img src="superset-frontend/src/assets/images/redshift.png" alt="redshift" border="0" width="200" height="80"/>
  <img src="superset-frontend/src/assets/images/google-biquery.png" alt="google-biquery" border="0" width="200" height="80"/>
  <img src="superset-frontend/src/assets/images/snowflake.png" alt="snowflake" border="0" width="200" height="80"/>
  <img src="superset-frontend/src/assets/images/trino.png" alt="trino" border="0" width="200" height="80"/>
  <img src="superset-frontend/src/assets/images/presto.png" alt="presto" border="0" width="200" height="80"/>
  <img src="superset-frontend/src/assets/images/databricks.png" alt="databricks" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/druid.png" alt="druid" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/firebolt.png" alt="firebolt" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/timescale.png" alt="timescale" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/rockset.png" alt="rockset" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/postgresql.png" alt="postgresql" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/mysql.png" alt="mysql" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/mssql-server.png" alt="mssql-server" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/db2.png" alt="db2" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/sqlite.png" alt="sqlite" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/sybase.png" alt="sybase" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/mariadb.png" alt="mariadb" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/vertica.png" alt="vertica" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/oracle.png" alt="oracle" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/firebird.png" alt="firebird" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/greenplum.png" alt="greenplum" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/clickhouse.png" alt="clickhouse" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/exasol.png" alt="exasol" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/monet-db.png" alt="monet-db" border="0" width="200" height="80" />
  <img src="superset-frontend/src/assets/images/apache-kylin.png" alt="apache-kylin" border="0" width="200" height="80"/>
  <img src="superset-frontend/src/assets/images/hologres.png" alt="hologres" border="0" width="200" height="80"/>
  <img src="superset-frontend/src/assets/images/netezza.png" alt="netezza" border="0" width="200" height="80"/>
  <img src="superset-frontend/src/assets/images/pinot.png" alt="pinot" border="0" width="200" height="80"/>
  <img src="superset-frontend/src/assets/images/teradata.png" alt="teradata" border="0" width="200" height="80"/>
  <img src="superset-frontend/src/assets/images/yugabyte.png" alt="yugabyte" border="0" width="200" height="80"/>
</p>

**Uma lista mais abrangente de bancos de dados suportados** junto com as instru????es de configura????o podem ser encontradas [aqui](https://superset.apache.org/docs/databases/installing-database-drivers).

Deseja adicionar suporte para seu armazenamento de dados ou mecanismo de dados? Leia mais [aqui](https://superset.apache.org/docs/frequently-asked-questions#does-superset-work-with-insert-database-engine-here) sobre os requisitos t??cnicos.

## Instala????o e configura????o

[Documenta????o estendida para Superset](https://superset.apache.org/docs/installation/installing-superset-using-docker-compose)

## Se envolver

- Fa??a e responda perguntas no [StackOverflow](https://stackoverflow.com/questions/tagged/apache-superset) usando a tag **apache-superset**;
- [Entre no Slack da nossa comunidade](https://join.slack.com/t/apache-superset/shared_invite/zt-16jvzmoi8-sI7jKWp~xc2zYRe~NqiY9Q)
  e leia nossas [Diretrizes da comunidade do Slack](https://github.com/apache/superset/blob/master/CODE_OF_CONDUCT.md#slack-community-guidelines);
- [Junte-se ?? nossa lista de discuss??o dev@superset.apache.org](https://lists.apache.org/list.html?dev@superset.apache.org).

## Guia do Colaborador

Interessado em contribuir? Confira nosso
[CONTRIBUTING.md](https://github.com/apache/superset/blob/master/CONTRIBUTING.md)
para encontrar recursos sobre como contribuir junto com um guia detalhado sobre
como configurar um ambiente de desenvolvimento.

## Recursos

Superset 2.0!
- [Encontro Superset 2.0](https://preset.io/events/superset-2-0-meetup/)
- [Notas de vers??o do Superset 2.0](https://github.com/apache/superset/tree/master/RELEASING/release-notes-2-0)

Entendendo os pontos de vista do Superset
- [O caso da visualiza????o centrada no conjunto de dados](https://preset.io/blog/dataset-centric-visualization/)
- [Entendendo a camada sem??ntica do Superset](https://preset.io/blog/understanding-superset-semantic-layer/)


- Introdu????o ao Superset
  - [Superset em 2 minutos usando o Docker Compose](https://superset.apache.org/docs/installation/installing-superset-using-docker-compose#installing-superset-locally-using-docker-compose)
  - [Instalando drivers de banco de dados](https://superset.apache.org/docs/databases/docker-add-drivers/)
  - [Criando novos conectores de banco de dados](https://preset.io/blog/building-database-connector/)
  - [Crie seu primeiro painel](https://superset.apache.org/docs/creating-charts-dashboards/first-dashboard)
  - [Tutorial abrangente para contribuir com c??digo para o Apache Superset
  ](https://preset.io/blog/tutorial-contributing-code-to-apache-superset/)
- [Recursos para dominar o Superset por Preset](https://preset.io/resources/)

- Como implantar o superconjunto
  - [Imagem oficial do Docker](https://hub.docker.com/r/apache/superset)
  - [Helm Chart](https://github.com/apache/superset/tree/master/helm/superset)

-Grava????es do Passado [Superset Community Events](https://preset.io/events)
  - [Mixed Time Series Charts](https://preset.io/events/mixed-time-series-visualization-in-superset-workshop/)  
  - [How the Bing Team Customized Superset for the Internal Self-Serve Data & Analytics Platform](https://preset.io/events/how-the-bing-team-heavily-customized-superset-for-their-internal-data/)
  - [Live Demo: Visualizing MongoDB and Pinot Data using Trino](https://preset.io/events/2021-04-13-visualizing-mongodb-and-pinot-data-using-trino/)
	- [Introduction to the Superset API](https://preset.io/events/introduction-to-the-superset-api/)
	- [Building a Database Connector for Superset](https://preset.io/events/2021-02-16-building-a-database-connector-for-superset/)

- Visualizations
  - [Building Custom Viz Plugins](https://superset.apache.org/docs/installation/building-custom-viz-plugins)
  - [Managing and Deploying Custom Viz Plugins](https://medium.com/nmc-techblog/apache-superset-manage-custom-viz-plugins-in-production-9fde1a708e55)
  - [Why Apache Superset is Betting on Apache ECharts](https://preset.io/blog/2021-4-1-why-echarts/)

- [Superset API](https://superset.apache.org/docs/rest-api)
