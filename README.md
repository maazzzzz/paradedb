<h1 align="center">
  <a href="https://paradedb.com"><img src="docs/logo/readme.svg" alt="ParadeDB"></a>
<br>
</h1>

<p align="center">
  <b>The Transactional Elasticsearch Alternative</b><br/>
</p>

<h2 align="center">
  <a href="https://paradedb.com">Website</a> &bull;
  <a href="https://docs.paradedb.com">Docs</a> &bull;
  <a href="https://join.slack.com/t/paradedbcommunity/shared_invite/zt-32abtyjg4-yoYoi~RPh9MSW8tDbl0BQw">Community</a> &bull;
  <a href="https://paradedb.com/blog/">Blog</a> &bull;
  <a href="https://docs.paradedb.com/changelog/">Changelog</a>
</h2>

---

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/paradedb)](https://artifacthub.io/packages/search?repo=paradedb)
[![Docker Pulls](https://img.shields.io/docker/pulls/paradedb/paradedb)](https://hub.docker.com/r/paradedb/paradedb)
[![License](https://img.shields.io/github/license/paradedb/paradedb?color=blue)](https://github.com/paradedb/paradedb?tab=AGPL-3.0-1-ov-file#readme)
[![Slack URL](https://img.shields.io/badge/Join%20Slack-purple?logo=slack&link=https%3A%2F%2Fjoin.slack.com%2Ft%2Fparadedbcommunity%2Fshared_invite%2Fzt-32abtyjg4-yoYoi~RPh9MSW8tDbl0BQw)](https://join.slack.com/t/paradedbcommunity/shared_invite/zt-32abtyjg4-yoYoi~RPh9MSW8tDbl0BQw)
[![X URL](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fparadedb&label=Follow%20%40paradedb)](https://x.com/paradedb)

[ParadeDB](https://paradedb.com) is a transactional alternative to Elasticsearch. It is an open source, ACID-compliant search and analytics database built on Postgres and optimized for update-heavy workloads.

- [ ] Powerful query DSL
- [ ] Columnar index
- [ ] Full Postgres compatibility

Watch "releases" to get notified of major updates.

## Documentation

For full documentation, visit [docs.paradedb.com](https://docs.paradedb.com).

For what features you can expect next, visit [our public roadmap](https://docs.paradedb.com/welcome/roadmap).

To see how to contribute, visit [Contributing Guide](/CONTRIBUTING.md).

## Community & Support

- [Community Forum](https://github.com/orgs/paradedb/discussions). Best for: help with building, discussion about database best practices.
- [Community Slack](https://join.slack.com/t/paradedbcommunity/shared_invite/zt-32abtyjg4-yoYoi~RPh9MSW8tDbl0BQw). Best for: sharing your applications and hanging out with the community.
- [GitHub Issues](https://github.com/paradedb/paradedb/issues). Best for: bugs and errors you encounter using ParadeDB.
- [Email Support](mailto:support@paradedb.com). Best for: problems with your database or infrastructure.

## How It Works

ParadeDB is a search engine packaged as a PostgreSQL extension. We're building the features of Elasticsearch/OpenSearch directly inside Postgres, as an extension. ParadeDB is not a 1-to-1 mapping of Elasticsearch. Our aim is to give developers an Elasticsearch-like feature set and performance, and improve upon the developer experience, infrastructure management, and cost.

### Architecture

Today, ParadeDB is a self-hosted product. In the future, we plan to build a hosted ParadeDB Cloud. You can easily start using ParadeDB with Docker:

```bash
# Pull the ParadeDB Docker image
docker run --name paradedb -e POSTGRES_PASSWORD=password paradedb/paradedb

# Connect to your database
docker exec -it paradedb psql -U postgres
```

ParadeDB is also available as a [PostgreSQL extension](https://github.com/paradedb/paradedb/releases/latest) and as a [Helm Chart](https://artifacthub.io/packages/helm/cloudnative-pg/cloudnative-pg).

ParadeDB supports all versions supported by the PostgreSQL Global Development Group, which includes PostgreSQL 14+, and you can compile the extensions for other versions of Postgres by following the instructions in the respective extension's README.

## License

ParadeDB is licensed under the [GNU Affero General Public License v3.0](LICENSE) and as commercial software. For commercial licensing, please contact us at [sales@paradedb.com](mailto:sales@paradedb.com).
