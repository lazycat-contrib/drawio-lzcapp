# draw.io for LazyCat

- Original upstream: https://github.com/jgraph/drawio
- Official Docker packaging: https://github.com/jgraph/docker-drawio
- Package `community.lazycat.app.drawio`, initial version 32.6.1, Linux amd64.
- Mirror delivery of `docker.io/jgraph/drawio` via `docker.1ms.run`, requiring matching source/image digests.
- Upstream Tomcat service listens on port 8080. No database, initial application password or server-side document store is configured.
- Keep LazyCat entry authentication. Choose Device to save diagrams and export backups.
- Opening `/?offline=1` disables cloud-storage support according to upstream documentation; it is not a guarantee of zero external network requests.
- No cloud-storage OAuth is provisioned. Cloud integrations and server-side PDF/image export are not verified or promised by this package.
- No file-chooser interceptor, smoke job or container-start test gate, as requested.

The reusable workflow builds a versioned Release LPK. Both automatic store publishers are disabled. Submit only the verified Release URL/SHA256 to MiaoMiao community store after full source/alias duplicate checks. Do not publish to the official store.

Build, configuration and digest verification are not runtime, device, editing or import/export interaction tests.
