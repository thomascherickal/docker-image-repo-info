## `rabbitmq:latest`

```console
$ docker pull rabbitmq@sha256:ebeda6be109f93f1d723b4e59377a8010427983e8197650456e9efd58ddb7c57
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `rabbitmq:latest` - linux; amd64

```console
$ docker pull rabbitmq@sha256:242b31161f9eab4cbcb0dd420954468a558f3e81aef2b92855830e303ab76e9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (102035416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7d2d17a7c5c2e31a0cdd9707ad1bcc25ef96300d07e3603538bf0ee667eda91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 05:34:21 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Wed, 18 Oct 2023 05:34:21 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Wed, 18 Oct 2023 05:34:21 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.3","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.3?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 05:34:21 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Wed, 18 Oct 2023 05:34:21 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		ldconfig; 	sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
ENV RABBITMQ_VERSION=3.12.7
# Wed, 18 Oct 2023 05:34:21 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 18 Oct 2023 05:34:21 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 18 Oct 2023 05:34:21 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 05:34:21 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.7","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.7?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
RUN gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 18 Oct 2023 05:34:21 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 18 Oct 2023 05:34:21 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 18 Oct 2023 05:34:21 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 05:34:21 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Wed, 18 Oct 2023 05:34:21 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:aece8493d3972efa43bfd4ee3cdba659c0f787f8f59c82fb3e48c87cbb22a12e`  
		Last Modified: Thu, 05 Oct 2023 07:43:26 GMT  
		Size: 29.5 MB (29537387 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95a7e9731f67235af4bc92ace8d1e0c1bb0f36cd2a940702e1b36331e381510b`  
		Last Modified: Thu, 19 Oct 2023 01:12:48 GMT  
		Size: 44.4 MB (44434134 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d5bb659a4871eb79b68698b62f61f95c19c63601a9fcd7d7057768d1538062c`  
		Last Modified: Thu, 19 Oct 2023 01:12:46 GMT  
		Size: 391.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfe39921a0ad0ef1cf8ec761b8e50bb22e1bb0e356250aa70c500d40823a9541`  
		Last Modified: Thu, 19 Oct 2023 01:12:46 GMT  
		Size: 7.5 MB (7456646 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a222b0c42b15f6496da0e254c40b1a83c9d440836ab5fb3dedea6ba4ad8b158`  
		Last Modified: Thu, 19 Oct 2023 01:12:46 GMT  
		Size: 388.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:af78870756d5346683976af7024bf39ef8f5151d7af8783b5ab1f43e05df4c73`  
		Last Modified: Thu, 19 Oct 2023 01:12:47 GMT  
		Size: 10.7 KB (10718 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dd1547e5e0a8641d2dd99dc1f78f92fe21e7d73d862234727df81b38e65fe0e`  
		Last Modified: Thu, 19 Oct 2023 01:12:48 GMT  
		Size: 20.6 MB (20594000 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e00ac9a1fa5d656fcbe066387762dbca451ab97942d465e5b0de8d644d83844`  
		Last Modified: Thu, 19 Oct 2023 01:12:47 GMT  
		Size: 190.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fdde25f2038d1376b7555fd9dd9d9d58f355059a94dee54178576e5b657c940`  
		Last Modified: Thu, 19 Oct 2023 01:12:48 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f80ae364b06196ed744ebd72d6dfa7f015911d282d83a73eb8f96bc51258fdf`  
		Last Modified: Thu, 19 Oct 2023 01:12:48 GMT  
		Size: 621.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8161bf23459e544bd40b02aff07cf9ec4904fb15d9535cb18aeed0f03497b32`  
		Last Modified: Thu, 19 Oct 2023 01:12:49 GMT  
		Size: 832.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:latest` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:2dd114426b97cfa2f842d873f139e8624924506f2cc5adedeec4f6766ca7398e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14732799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c862691abb9996bd26829143d5dacb0b23903d92f8a25228d59b2ca7f79937`

```dockerfile
```

-	Layers:
	-	`sha256:63fd319925b46db6b5d8a7b916345bebb1891d889c021fbe78d3e46c997fbed0`  
		Last Modified: Thu, 19 Oct 2023 01:12:46 GMT  
		Size: 2.5 MB (2482738 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9f2cef48a9c9d8c54c4cbaa6d04646159e0ad234799d7d3b14848d1bd84f10b1`  
		Last Modified: Thu, 19 Oct 2023 01:12:46 GMT  
		Size: 4.1 MB (4059998 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2946fad23e35a9387d6772f693d19e96519e5f8fc8c8e2006dad24ed008b0004`  
		Last Modified: Thu, 19 Oct 2023 01:12:46 GMT  
		Size: 4.1 MB (4060954 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6726bca3076d120ae044b7d74a8b5ded1b7079efcd0c682762ae979ed4f193c2`  
		Last Modified: Thu, 19 Oct 2023 01:12:46 GMT  
		Size: 4.1 MB (4060008 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9df5152992dc6a558b0651f052bb1d881950d1a1f7462a8680fe5353a39a4b54`  
		Last Modified: Thu, 19 Oct 2023 01:12:47 GMT  
		Size: 69.1 KB (69101 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:latest` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:3973f5e381d9af342e5d0de1c91edd48fa275e0b022f9c0a49f872131b8c3a1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.9 MB (85939429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32893d78cdec9933129845132b6c433ebad27e47be59cc9f9b5ad771063c0cc6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 18:44:42 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Thu, 12 Oct 2023 18:44:42 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Thu, 12 Oct 2023 18:44:42 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.3","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.3?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 18:44:42 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 12 Oct 2023 18:44:42 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		ldconfig; 	sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
ENV RABBITMQ_VERSION=3.12.6
# Thu, 12 Oct 2023 18:44:42 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 12 Oct 2023 18:44:42 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 12 Oct 2023 18:44:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 18:44:42 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.6","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.6?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
RUN gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 12 Oct 2023 18:44:42 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 12 Oct 2023 18:44:42 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 12 Oct 2023 18:44:42 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Oct 2023 18:44:42 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 12 Oct 2023 18:44:42 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:4091a3a7d6aa711dc0e0bbacfd3546df44ca257c300de1ad00fbdc95e218f7bd`  
		Last Modified: Thu, 05 Oct 2023 07:43:39 GMT  
		Size: 26.6 MB (26629612 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1c0d6d130ad31b7ebf90481ea768a73d3f707d74da864298ae273ff35ef4abb1`  
		Last Modified: Fri, 13 Oct 2023 05:19:05 GMT  
		Size: 32.7 MB (32747573 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:45453c12558c31f60aa945336a43dbd5a3ef29d1337eb083625ab7c05bd7c52c`  
		Last Modified: Fri, 13 Oct 2023 05:19:04 GMT  
		Size: 395.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a649c99d3201128684769a55154423277d509412b9d9be482c4c4e7afb1eee11`  
		Last Modified: Fri, 13 Oct 2023 05:19:04 GMT  
		Size: 6.1 MB (6056463 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:561ee6edf6fe7663873520b11f81a7ce9b2ef73bb8d929bc14cd95746ef216f3`  
		Last Modified: Fri, 13 Oct 2023 05:19:04 GMT  
		Size: 388.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea809ab724ff1de3cd78015d47e142e892f4d96ea289f22d2710451b1e562655`  
		Last Modified: Fri, 13 Oct 2023 05:19:05 GMT  
		Size: 10.7 KB (10711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d894427abb6451d9d345e65f78a770f76047cf86aedcc607314410cdfad40773`  
		Last Modified: Fri, 13 Oct 2023 05:19:07 GMT  
		Size: 20.5 MB (20492542 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9628369ecc1ccd7cb368be8796ef445eac4210e91b5a1e34a40622f367c542bd`  
		Last Modified: Fri, 13 Oct 2023 05:19:06 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0f67ebfeb02d2457b66692114c6e987b052943442d4007c7698ca20a4035e74`  
		Last Modified: Fri, 13 Oct 2023 05:19:06 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:78365ebe40ff9fc6757de8e5f8fb914cc20e08fd102694b72374bb5513874451`  
		Last Modified: Fri, 13 Oct 2023 05:19:07 GMT  
		Size: 617.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cff052ba3edff1c7fc26bab60f77748ba6b411907de9be56edc0c18fe5380490`  
		Last Modified: Fri, 13 Oct 2023 05:19:07 GMT  
		Size: 832.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:latest` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:9bd590c97789b971fcefd5f27ea4e984226f6e8cea00f55ed6396c40af7d6cb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14361915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef501494dfa4f5bee52e8ede9312aefe36823aaecb89f9dda75321021e884ed9`

```dockerfile
```

-	Layers:
	-	`sha256:9ad19b2a61c3d91573660de5990e78745e43f90e1d8230ecd6f085efa3764cc1`  
		Last Modified: Fri, 13 Oct 2023 05:19:04 GMT  
		Size: 2.5 MB (2491262 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d62613aa66fbc91b18376b73f5a4c2d93bb57e3affe41e078d80e55cb5b08ac`  
		Last Modified: Fri, 13 Oct 2023 05:19:04 GMT  
		Size: 3.9 MB (3933458 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fa33cc7a8d6b60f1c6738d93c4a2bed1b11456d3b4f9f22bbbc1729b23b212fe`  
		Last Modified: Fri, 13 Oct 2023 05:19:04 GMT  
		Size: 3.9 MB (3934414 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b2771a49a38f03e74fda21e62514b312923afd5606de757752b5e58c4d980888`  
		Last Modified: Fri, 13 Oct 2023 05:19:04 GMT  
		Size: 3.9 MB (3933468 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:161ca6ec9f68170e21ba0bfca95f09617938186a473f128d211a47106080b05c`  
		Last Modified: Fri, 13 Oct 2023 05:19:05 GMT  
		Size: 69.3 KB (69313 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:latest` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:49c48842b6e8797b228c86ad9aa98b6ff77ab650e25d17ec1f171ad7a0a83b73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97248649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abe85937b1124df588763b27da37c0bcae44859258e65f85bdb3f6873b09137`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 18:44:42 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Thu, 12 Oct 2023 18:44:42 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Thu, 12 Oct 2023 18:44:42 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.3","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.3?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 18:44:42 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 12 Oct 2023 18:44:42 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		ldconfig; 	sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
ENV RABBITMQ_VERSION=3.12.6
# Thu, 12 Oct 2023 18:44:42 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 12 Oct 2023 18:44:42 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 12 Oct 2023 18:44:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 18:44:42 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.6","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.6?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
RUN gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 12 Oct 2023 18:44:42 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 12 Oct 2023 18:44:42 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 12 Oct 2023 18:44:42 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Oct 2023 18:44:42 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 12 Oct 2023 18:44:42 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:bfbe77e41a78ee38147c5761aa8bc896d9f6e1e648b23468f294065ffe03c107`  
		Last Modified: Thu, 05 Oct 2023 07:43:33 GMT  
		Size: 27.4 MB (27351048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eff91934b4f1b432862ee2ca3298c552a9ad7b40e52f352b18f22e1d304997ba`  
		Last Modified: Fri, 13 Oct 2023 15:13:28 GMT  
		Size: 42.3 MB (42286569 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e263c0a725b1c3a3fb3bbcf371490759d9020c28f0913e09b28b565f24be8ec`  
		Last Modified: Fri, 13 Oct 2023 15:13:25 GMT  
		Size: 394.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef489f41c4dc239c770424ab84afb41d5ec917e331de1a93b8c1eeeb70bc78e5`  
		Last Modified: Fri, 13 Oct 2023 15:13:26 GMT  
		Size: 7.1 MB (7113724 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a23861d96e07c21c205320363fa0c401c1da4f4628dc360a3d1459a3931973d8`  
		Last Modified: Fri, 13 Oct 2023 15:13:25 GMT  
		Size: 385.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1411271f10a2b60cd5e8de358a4ffd05228944cf47409164bf64dc2fafd9b78b`  
		Last Modified: Fri, 13 Oct 2023 15:13:26 GMT  
		Size: 10.7 KB (10704 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a3513cc3f324821f75087ce401881dea8f1968cd3095488e96662dd8078de0f`  
		Last Modified: Fri, 13 Oct 2023 15:13:28 GMT  
		Size: 20.5 MB (20484079 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e956d04bc3254f9a4db4066aa92e6761ab2e2d6258491c2efe350f6e98a4e18`  
		Last Modified: Fri, 13 Oct 2023 15:13:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6d6c45234f92657cecc5fbe4f5e005225bc4c862f746dd4bea753428eb46e69`  
		Last Modified: Fri, 13 Oct 2023 15:13:27 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7276d5e164ddf3ecac9ff9a25cef7e3cd82894d69d64a26fb0bcd32198b5ca1d`  
		Last Modified: Fri, 13 Oct 2023 15:13:28 GMT  
		Size: 617.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e293e34cf4eedae225ae7924eece717852c0d3d88be3130ac05fcdecca819114`  
		Last Modified: Fri, 13 Oct 2023 15:13:29 GMT  
		Size: 831.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:latest` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:48ce399c892b863c3816140aff74e9942590b6ef600cad40075fa9d6d19100fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14747903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2ce3737d2eabe75cea8e61a8fdd0489452a596a9975482230174a2e55581023`

```dockerfile
```

-	Layers:
	-	`sha256:fbb344a18fb822871fe0787498c48ddc19ffc65a855a7e15d5043ffdd40673e0`  
		Last Modified: Fri, 13 Oct 2023 15:13:26 GMT  
		Size: 2.5 MB (2485193 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:778c2985cfcc2a8dbbc6894bdf63b6b2d7356a4eb2ae5ff23257f7c517309823`  
		Last Modified: Fri, 13 Oct 2023 15:13:26 GMT  
		Size: 4.1 MB (4064211 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8ed140e6db303277ac64d50eb15454788bbbdd33dabed2f57cf89ca755eb3019`  
		Last Modified: Fri, 13 Oct 2023 15:13:26 GMT  
		Size: 4.1 MB (4065167 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ad25d5cf315134ffcad0d6b73cf42eb47c0112c96fcc9b99885c4b16dabdca08`  
		Last Modified: Fri, 13 Oct 2023 15:13:26 GMT  
		Size: 4.1 MB (4064221 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:226936113bf699fc689b1855136566545b07cff327c08328ba7906e5a56ac4c6`  
		Last Modified: Fri, 13 Oct 2023 15:13:27 GMT  
		Size: 69.1 KB (69111 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:latest` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:3f8350bbc9a623681abf69b904ee3f09b9c840115d587c4cec67ef0f9383df9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101705327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d225758c989af9a4afab32eeb5237beff5906b809c4a4b2cf8570b1b03097548`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
# Wed, 18 Oct 2023 05:34:21 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Wed, 18 Oct 2023 05:34:21 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Wed, 18 Oct 2023 05:34:21 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.3","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.3?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 05:34:21 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Wed, 18 Oct 2023 05:34:21 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		ldconfig; 	sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
ENV RABBITMQ_VERSION=3.12.7
# Wed, 18 Oct 2023 05:34:21 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 18 Oct 2023 05:34:21 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 18 Oct 2023 05:34:21 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Oct 2023 05:34:21 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.7","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.7?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
RUN gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 18 Oct 2023 05:34:21 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 18 Oct 2023 05:34:21 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 18 Oct 2023 05:34:21 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 05:34:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 05:34:21 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Wed, 18 Oct 2023 05:34:21 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:90496cba4a92b0bf6a8307bab5dd30100905ac891d478aa27771408328244c33`  
		Last Modified: Thu, 05 Oct 2023 07:43:45 GMT  
		Size: 34.6 MB (34555968 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f5cf081d84ec0db73d6f038275d5d28867733f5052e9a4dccd95295f83dfc62`  
		Last Modified: Fri, 13 Oct 2023 12:44:23 GMT  
		Size: 38.8 MB (38768475 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a531104a95c52c0dbb02b11daf3df39d7fd1def2c7da2cbaa659d2ecf300c492`  
		Last Modified: Fri, 13 Oct 2023 12:44:20 GMT  
		Size: 392.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3bd5b0b8f859f675992b4a73774fce6a37164aacd2a24429af1055bc9948ae3b`  
		Last Modified: Fri, 13 Oct 2023 12:44:21 GMT  
		Size: 7.8 MB (7836656 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e17229535514abb86075e3888da17df59395ad97fcee69b8208c2ae73e952d4`  
		Last Modified: Fri, 13 Oct 2023 12:44:21 GMT  
		Size: 391.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0bd39b6025dc4abb1fb1b636579fa4662c18eaca2d98aa428a061798ed5da904`  
		Last Modified: Fri, 13 Oct 2023 12:44:21 GMT  
		Size: 10.6 KB (10640 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcfe8f5306c8418e8deeb582301fd6f6f3cdf51bf52ddc550567e4b2bf28f41c`  
		Last Modified: Thu, 19 Oct 2023 02:16:41 GMT  
		Size: 20.5 MB (20531058 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:58acbd9f020e65b07daf981f7d6a40137eb82bbb37b9ae01f55dec9ad439f951`  
		Last Modified: Thu, 19 Oct 2023 02:16:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f348699b323d105655f3d2598240fdb427486ac2665f3877d208e3189674b41`  
		Last Modified: Thu, 19 Oct 2023 02:16:40 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:820f5edd091f3cd697d62c746ca54df8a2c2ca536f783631bd986c76754a6ca5`  
		Last Modified: Thu, 19 Oct 2023 02:16:40 GMT  
		Size: 621.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a09c0d463496dc89c6bc07940becdd005216c5a38f70dd6be734dad59bc30ffb`  
		Last Modified: Thu, 19 Oct 2023 02:16:41 GMT  
		Size: 830.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:latest` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:9eb0cdfb29fc3e9c0f26257e055c865c7cd2f725535591b8af7d7b4db779857d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14737464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7da38541b5b216ba6d2099323cfd245df2ef67527db893ab5282d3438f5334ef`

```dockerfile
```

-	Layers:
	-	`sha256:de197e7200701acdef00501aef09af474579786d082e54907cd8a90904bac313`  
		Last Modified: Thu, 19 Oct 2023 02:16:40 GMT  
		Size: 2.5 MB (2497761 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ddea5f9e4de0806a11a2fadf0f92cc21bfde4388ccfb60f8445ec1ca0a6f1127`  
		Last Modified: Thu, 19 Oct 2023 02:16:40 GMT  
		Size: 4.1 MB (4056579 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:865d9d0c668ef4e5d07a6c03aa9972ccc9c73248cb5aedf72906611290aecff6`  
		Last Modified: Thu, 19 Oct 2023 02:16:40 GMT  
		Size: 4.1 MB (4057535 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:66564d17aee0fcf36f001c0a6833ab0122dfe71494fa0bcdbbb7e666434d331d`  
		Last Modified: Thu, 19 Oct 2023 02:16:41 GMT  
		Size: 4.1 MB (4056589 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5b114cee0b989886fe83885c380c0c7f4d778c7ac63e1af61f4ace96cd2edd25`  
		Last Modified: Thu, 19 Oct 2023 02:16:41 GMT  
		Size: 69.0 KB (69000 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:latest` - linux; s390x

```console
$ docker pull rabbitmq@sha256:1ce5662c459223c0a5573ebfa361da9d64e3820765f5cf926692e8ec0bc7612e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.5 MB (92508365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93fd8f7dc1d198f51216da12eb22c3717a65d983276f959312b4b8b937a51e2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 05 Oct 2023 07:29:34 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:29:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:29:36 GMT
ADD file:d165475f8f027ab758a463da57c8c29f5d302f0a87a475ac68fdfae30005c7ac in / 
# Thu, 05 Oct 2023 07:29:36 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 18:44:42 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Thu, 12 Oct 2023 18:44:42 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Thu, 12 Oct 2023 18:44:42 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.3","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.3?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 18:44:42 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 12 Oct 2023 18:44:42 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		ldconfig; 	sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
ENV RABBITMQ_VERSION=3.12.6
# Thu, 12 Oct 2023 18:44:42 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 12 Oct 2023 18:44:42 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 12 Oct 2023 18:44:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 18:44:42 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.6","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.6?os_name=ubuntu&os_version=22.04"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
RUN gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 12 Oct 2023 18:44:42 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 12 Oct 2023 18:44:42 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 12 Oct 2023 18:44:42 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 12 Oct 2023 18:44:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Oct 2023 18:44:42 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 12 Oct 2023 18:44:42 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:0ffe28a7c279dfdb86b23c0d22d37e89442a6d771fbded124aee76b24119c2c1`  
		Last Modified: Thu, 05 Oct 2023 07:43:51 GMT  
		Size: 28.0 MB (28023918 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fbc84f1bf54d1b74d6ca166cbb2520f26e5b9d365d5d7be9ca7af046d33494b7`  
		Last Modified: Fri, 13 Oct 2023 14:49:58 GMT  
		Size: 37.4 MB (37422260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:802b9ae85cc037faf4d711cd66526242b0a3ecd3504568455b14fcef2579822f`  
		Last Modified: Fri, 13 Oct 2023 14:49:55 GMT  
		Size: 394.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf0fa9a51a3eef2b59fd807b0787a62f851ea406919dbd8acd65a636ad7aacf5`  
		Last Modified: Fri, 13 Oct 2023 14:49:56 GMT  
		Size: 6.5 MB (6505063 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12aa2d372f322c92bf1e831c702fa986e70845a01d64506e0f1e4c4104f9267b`  
		Last Modified: Fri, 13 Oct 2023 14:49:55 GMT  
		Size: 387.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e7f9a2621fd3f2511972cc7c45cf6838fd4881200c6598f2bd993a01fefd4954`  
		Last Modified: Fri, 13 Oct 2023 14:49:56 GMT  
		Size: 10.8 KB (10768 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:409e1d1aeb35aa3a30e2de308c6bdba2b0bcae9d1d5f749d6b507f2dec402c03`  
		Last Modified: Fri, 13 Oct 2023 14:49:58 GMT  
		Size: 20.5 MB (20543831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1d0523afd4bf6093c1d6996f1f75be62b1bbdcbe49dbcb291bb7a8bc303d99c8`  
		Last Modified: Fri, 13 Oct 2023 14:49:57 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18cddaf5444a86ee185e2501e97d534147b86939f1ca2dd47ece54b945ce31ce`  
		Last Modified: Fri, 13 Oct 2023 14:49:57 GMT  
		Size: 106.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cc340fc7cdd6de9045cc10738e883a7198d052270c1a8690c4358d1d7a95f5ed`  
		Last Modified: Fri, 13 Oct 2023 14:49:58 GMT  
		Size: 619.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27fe2f4c5a8bd724bd519698353b85b2e3d5f2ef150b7c35e75a1343edb346bf`  
		Last Modified: Fri, 13 Oct 2023 14:49:58 GMT  
		Size: 831.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:latest` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:785802131331cc6dc2ac78c13702210826be3fabaacd399b877b80bb88517234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.3 MB (14349688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9fc0eb3b9286fbac725ffd202165f4b4e4301f6fe210d1ee3d6999cc0ef9769`

```dockerfile
```

-	Layers:
	-	`sha256:cd16be1dac002a2b5b7306a464a66c1779c1bb4a1cd931f385af81c5a68cd378`  
		Last Modified: Fri, 13 Oct 2023 14:49:55 GMT  
		Size: 2.5 MB (2482277 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b91d2f3ca6d1119060df90c7609d44b0f8ea4de842adc3ed208bb029c4c7b266`  
		Last Modified: Fri, 13 Oct 2023 14:49:56 GMT  
		Size: 3.9 MB (3932448 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:513b9ceec7834dac34543c0b87d891051916ef9d505f417fdc795e1b068a7135`  
		Last Modified: Fri, 13 Oct 2023 14:49:56 GMT  
		Size: 3.9 MB (3933404 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a68e561a55fc7a79f2d08d1b1b3cdd77354ef2fff4edf6cc25a00071b06e3e0f`  
		Last Modified: Fri, 13 Oct 2023 14:49:55 GMT  
		Size: 3.9 MB (3932458 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:db0862ce6066720f66fde9af731c107b2a43eb4d930be3998880bac848c5006d`  
		Last Modified: Fri, 13 Oct 2023 14:49:57 GMT  
		Size: 69.1 KB (69101 bytes)  
		MIME: application/vnd.in-toto+json
