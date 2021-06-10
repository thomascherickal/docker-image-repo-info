## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:699404cfeaf1b53b36b5cad0c6d2fe8858034adb85e80f41f14f9fbe13a22366
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:d4a3e0eabf14e4f98a9bcf5eada28d1443573b082afe95028d548d5b88a2b33e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654170862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736d3aa581b715efdf7c0431ebfbaed21b664091d8e8f7e4595c5f9dabbd2acb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:08:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:08:07 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:08:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:08:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:08:49 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:08:51 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:08:53 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:08:55 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:08:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:09:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:09:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:09:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:09:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:09:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:09:14 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:09:17 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:09:19 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:09:41 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:09:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dc18d712eacfb666370e311daaf51e09fc2f76ca762e4592e149fbe6aba561`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 361.4 KB (361380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b774f6019fa0c611532d02bdf31c54e9da56fe2330e3e0745538ef036cfb87`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e977598d13d0ee9ae780f2cf34706c57e810301d20d9fc8286ad9390b9166b`  
		Last Modified: Wed, 09 Jun 2021 20:19:37 GMT  
		Size: 11.9 MB (11906202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7361692fe34486902f2dd9f69cc3bce54c4cb8c5c86ed80a0d75033f25ae5213`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35d39d3918ab9262122b494a653aec25e76a65396f9198d7be955cb9c26c6f3`  
		Last Modified: Wed, 09 Jun 2021 20:19:34 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66891a50a919af8d3cb83358a7f8d33b2055c143bd3499cc431fd32d053ed393`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519d446a1689a5424a77bf1cbf0f00153b28c6eff9ee22f0f88e0e32b3f6bda3`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ea2eef93aa67b4ac4bfb48ac5498fa33b02d0b88b9ae60b8ae159addacecc`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fc40bc9ade11a1755b185c529e961b474d959d45a44b1b1ab5f12e3d17863a`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ef9960b6bac284e65c351bc447bb8931486a0c1c3ee68c9e5a62828b4ae0e`  
		Last Modified: Wed, 09 Jun 2021 20:19:31 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfda8707421463aa0f297ce5d4ac3a615f60caf56e6e69a299caa08a04f7da`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa0c9ece6e3482cf3ffc8d9a087d113db0f7c249f59bcf06f3ffc65c5e4bce0`  
		Last Modified: Wed, 09 Jun 2021 20:19:29 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6614223fb410a8262956f73a038f6d79b67d5976fe8740b21dfa2121a9cbd7f2`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354857e070035731eb660ec35ff9f8549b6cc79211bab40ae642d9875f98f8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc94f29a4cb79013fce0bf1a5776868fa31912b598231e46883a114d86f712d3`  
		Last Modified: Wed, 09 Jun 2021 20:19:28 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e536fde913e2e2d5ae24846adca32195330a9be6e7d1c3180ce7ac6bc6a35ae1`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b11db027637bf7abeec6bbcd83920c4eb7c291aeeae4d2886a1563bf41289a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3a70d973d27d739faae877290b3184bee11c706ebd4bfa515d180fba88ef0f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7b3e3d99424f8d3737a4502a6f50767ae25b699a315155b98700af682b64f`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 292.6 KB (292631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d435932a64bec158a6193fa4a31a1b38e446ec9f63c0b6be3282c3acf3288949`  
		Last Modified: Wed, 09 Jun 2021 20:19:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
