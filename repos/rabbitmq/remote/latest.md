## `rabbitmq:latest`

```console
$ docker pull rabbitmq@sha256:d0f4866bd72e09c09cc96098a7d29a14dd389adf8db1da127f132f6f1ad4f094
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:latest` - linux; amd64

```console
$ docker pull rabbitmq@sha256:6f642cafdf4edbb8c1789a8a9cb8724c313b17c36f70f72b81957bbad3976feb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.5 MB (105501123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e03303f2197e93dcccef9fab7936af8c9d86386b0a2548dbb59ace0f021bf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_VERSION=3.11.10
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 11 Mar 2023 00:07:30 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 11 Mar 2023 00:07:30 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Mar 2023 00:07:30 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 11 Mar 2023 00:07:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fd8067e26d2796d30d5a361ad352de42198ef289794a911985c1f449aa1ebb`  
		Last Modified: Thu, 16 Mar 2023 05:53:46 GMT  
		Size: 424.7 KB (424651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f617f636f46570027b391d03afb523a3428ef9f151ad1d7db000c36084d9e7`  
		Last Modified: Thu, 16 Mar 2023 05:53:46 GMT  
		Size: 10.1 KB (10125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa68bb7204a51c8540192f7426b32a78a007d9afaf72e615c396f42d62e8690`  
		Last Modified: Thu, 16 Mar 2023 05:53:53 GMT  
		Size: 54.9 MB (54892905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55a28a6ac3f96a5cd5e2fa0a754928e1b204ba3fef40c941c85c98d60c7878c`  
		Last Modified: Tue, 21 Mar 2023 00:05:32 GMT  
		Size: 10.9 KB (10878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6eb577a2a1d138bcf2acdaa8c6fc696afeb8632b9f413b442ca54d67631d72`  
		Last Modified: Tue, 21 Mar 2023 00:05:54 GMT  
		Size: 21.6 MB (21582785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a979304bda2657b93d0938f2daf0710ede956cc3407ac94fb5121bf0ade2ca50`  
		Last Modified: Tue, 21 Mar 2023 00:05:52 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fdda97b46a66bb315be095891d685f4d5ea1e8f296f6d2fb3c5a2024b3a982`  
		Last Modified: Tue, 21 Mar 2023 00:05:52 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad95befe22f9c336fa03e07ccde7eaed580a1f81db02b5edc21763eae11d131`  
		Last Modified: Tue, 21 Mar 2023 00:05:52 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082f933a70c5eaf6daf11577ae71aaea1480bcb88c848974d987da9ca8841c68`  
		Last Modified: Tue, 21 Mar 2023 00:05:52 GMT  
		Size: 833.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:6c7dc1310e13e8d03410c3c073876c0648fc8cc16f7764ca7fc4aca2229744a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90095156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d085579e1c3e96809211dee83c7fc9b7f48b3a238fa5a3e86142af4f480353`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 16 Mar 2023 03:03:40 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 16 Mar 2023 03:03:40 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 16 Mar 2023 03:03:42 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 16 Mar 2023 03:03:42 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 16 Mar 2023 03:03:42 GMT
ENV RABBITMQ_VERSION=3.11.10
# Thu, 16 Mar 2023 03:03:42 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 16 Mar 2023 03:03:42 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 16 Mar 2023 03:03:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 03:04:58 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 16 Mar 2023 03:04:59 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Thu, 16 Mar 2023 03:04:59 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 16 Mar 2023 03:04:59 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 16 Mar 2023 03:04:59 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 16 Mar 2023 03:04:59 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:04:59 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 16 Mar 2023 03:04:59 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 16 Mar 2023 03:04:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Mar 2023 03:04:59 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 16 Mar 2023 03:04:59 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66856c3f04df9a1a7fc6115deabed9bbc5b36763ba558fc622b601b664f5af2`  
		Last Modified: Thu, 16 Mar 2023 03:08:52 GMT  
		Size: 390.6 KB (390586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f4f2f1e62b9a46248513230d622372b4983228f475e00f6d449d4b229b1ae3`  
		Last Modified: Thu, 16 Mar 2023 03:08:51 GMT  
		Size: 10.1 KB (10137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd5ef912b647348167b8fdcf1e82d6c76bd77fc64f5dd603153f6799aa263bb`  
		Last Modified: Thu, 16 Mar 2023 03:08:57 GMT  
		Size: 43.9 MB (43941826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42bc1a27f2a641f00b506e0731d1de6bc14718cce6ff420470a38e6507f8418`  
		Last Modified: Thu, 16 Mar 2023 03:08:51 GMT  
		Size: 10.8 KB (10827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d76c8149b27c2696e75d4607970f0e319b114667bfb5bec94a7229dc718e65`  
		Last Modified: Thu, 16 Mar 2023 03:09:26 GMT  
		Size: 21.2 MB (21153589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3e85167b9c4ac31a307e6d0095eae9862ec976068c5e47696a5abe9cf900ce`  
		Last Modified: Thu, 16 Mar 2023 03:09:23 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5848957a0c2dea21553819f649d1ac4ac604a8287d1af93c01dcbc77ffd00da8`  
		Last Modified: Thu, 16 Mar 2023 03:09:23 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcef18b386904a7bcc44777ca3d83907392f540b49ab5f052866abaf017d187`  
		Last Modified: Thu, 16 Mar 2023 03:09:23 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f913f042ab576f770fa594fde67ed9a6c4c2cf255dd2cc6f864b94473ea62cf0`  
		Last Modified: Thu, 16 Mar 2023 03:09:23 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:00403e7f6c228a489baf74a27b42dd6905180798bb259d9729ccf7d1469d12c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101967915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cdf4a751b0eaf4e1ebf2ffc17e09dd694bde63cf339709051d278347ac4a6f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_VERSION=3.11.10
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 11 Mar 2023 00:07:30 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 11 Mar 2023 00:07:30 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Mar 2023 00:07:30 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 11 Mar 2023 00:07:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39f435f458d06973355f6fc5c0bf42af21cd9a429430d0b50ca4f2bcc49c437`  
		Last Modified: Thu, 16 Mar 2023 04:31:58 GMT  
		Size: 409.1 KB (409058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea08ad42e588719c2465aec2ebfb8ebb4e9e0ffadf505d4b55c680651a9fe3b`  
		Last Modified: Thu, 16 Mar 2023 04:31:57 GMT  
		Size: 10.1 KB (10134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7f7468488467ae4ce6ca6cd45aa9d076e979b5d81f2479f0ff7a61a7d83d8c`  
		Last Modified: Thu, 16 Mar 2023 04:32:03 GMT  
		Size: 52.9 MB (52940386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4baa3e31da578670a65f24a43b1d25bfdbbdcd22488337440284cf8144ee5bc5`  
		Last Modified: Tue, 21 Mar 2023 00:17:16 GMT  
		Size: 10.9 KB (10881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ceb2edc498f493757c26b53b2c853f69722a8a0ce5394d669f10fdef929df`  
		Last Modified: Tue, 21 Mar 2023 00:17:37 GMT  
		Size: 21.4 MB (21399583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b95b7224f50e0ed2cefcd7cdb43865901e597e24921dd61b0808ca309501eac`  
		Last Modified: Tue, 21 Mar 2023 00:17:35 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e751ad84368078d36f08387301fffa810f41d7fd04828a4aecf75a76e4b67`  
		Last Modified: Tue, 21 Mar 2023 00:17:35 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9750c785cd3f6f5cf7fdef5b9b5c13586810b46ac8e61d3abcff722b7dccc8`  
		Last Modified: Tue, 21 Mar 2023 00:17:35 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6063bba8a3a87fcc57d07b66af8bb394253fbea62483de1528287b380eff2cde`  
		Last Modified: Tue, 21 Mar 2023 00:17:35 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:26270ab6244a97b889891ca2d3f7d76d916b6a7395f3119c342a331ae7507ebd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.5 MB (103518315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c0581b2547fa53319ca083cb8ae68fae7386fdda878c9c0afd304a87bf088fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:14 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:39:17 GMT
ADD file:e8eae0af07e662df38a5b691d04648b4fc72382b6918877da22520ed4d01c3a6 in / 
# Wed, 08 Mar 2023 04:39:17 GMT
CMD ["/bin/bash"]
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_VERSION=3.11.10
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 11 Mar 2023 00:07:30 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 11 Mar 2023 00:07:30 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Mar 2023 00:07:30 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 11 Mar 2023 00:07:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:35c7876eb976fb68d0f3bf24f227b6220a73f879e77ad564d913af35104da2eb`  
		Last Modified: Thu, 16 Mar 2023 01:58:06 GMT  
		Size: 33.3 MB (33300378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51eac5e0f20f0ba928841bb2e5d37553da383cc39f193745a0533518cfc530e4`  
		Last Modified: Thu, 16 Mar 2023 02:45:57 GMT  
		Size: 451.0 KB (451041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b249cea74aa342d32fcd9e2e75c960a857b61d291675e4cdee46bb144afea3e0`  
		Last Modified: Thu, 16 Mar 2023 02:45:57 GMT  
		Size: 10.1 KB (10139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba016b6e9b8502b81a0776aaac20aaeb7e9652bbbdffeb6124f6d590879c6c91`  
		Last Modified: Thu, 16 Mar 2023 02:46:07 GMT  
		Size: 48.0 MB (48023432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052acc834e5c63af7c3f8fa1e7b050fafbdb90fda8de862d6efbc5d1cb5bb4e2`  
		Last Modified: Tue, 21 Mar 2023 00:00:50 GMT  
		Size: 10.9 KB (10873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4405aaac469ea58f261c0111686b719ccdb2555dd7080a8068206e5619b49493`  
		Last Modified: Tue, 21 Mar 2023 00:01:22 GMT  
		Size: 21.7 MB (21720737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e359345e4cd9f81ccd6aeb6b09f332225e0baab3197bcad44df50de8f0d6cd19`  
		Last Modified: Tue, 21 Mar 2023 00:01:18 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557caeef008e6f3c5e4b5196c191efa8bd181cbe10b1c9fbc8168749e12d747f`  
		Last Modified: Tue, 21 Mar 2023 00:01:18 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fa44d5d34b4ed09d0011b755e36dce411ef0694d17ca61a8f87ec3d74f2767`  
		Last Modified: Tue, 21 Mar 2023 00:01:18 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0032fe9a907cad1fcf9487b88ce00eb7146d32c09c825a8fb1aee18526fafb51`  
		Last Modified: Tue, 21 Mar 2023 00:01:18 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; s390x

```console
$ docker pull rabbitmq@sha256:febc61e8338fe61490c1c2142dfd5c2c5901587e2e9e1cbae44068822dee2da0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98956484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c494238d26e032825d99d1e4458c0ce78ab647ef439fd24d0ec9c3fbe32817f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:58 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:42:00 GMT
ADD file:4463dafd3352de8c5ff87090e2f30be9bdffc3fa9d84e27b13e2364d856f82e9 in / 
# Wed, 08 Mar 2023 04:42:00 GMT
CMD ["/bin/bash"]
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_VERSION=3.11.11
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 20 Mar 2023 23:05:20 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 20 Mar 2023 23:05:20 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Mar 2023 23:05:20 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 20 Mar 2023 23:05:20 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:422c367cdac1ee2f6bd9ea546c8e5a643af0847a822d04ba202af409973273ad`  
		Last Modified: Thu, 16 Mar 2023 01:40:19 GMT  
		Size: 27.0 MB (27016120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47a7e1f090e04a728408c58f6022d846f3061d7407b385b3507852f3a6f04a7`  
		Last Modified: Thu, 16 Mar 2023 01:40:15 GMT  
		Size: 425.8 KB (425776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21fe49ecbadda9d41e39185251d9cc83053a9e437eb735be12618a82baf4710`  
		Last Modified: Thu, 16 Mar 2023 01:40:14 GMT  
		Size: 10.1 KB (10125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d432de49c7c71ab93ff10e9489dc8150a2143ef7ed24bba9754e27d995b53ea4`  
		Last Modified: Thu, 16 Mar 2023 01:40:20 GMT  
		Size: 44.7 MB (44741629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a92d66e1505b7d04d579753952e9ea8b21d8cf3104060401a297edbe7926087`  
		Last Modified: Tue, 21 Mar 2023 00:13:11 GMT  
		Size: 10.9 KB (10894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d07193569408709900f0596f61b0f873fbb90f13e768941c46da0bf4d47f639`  
		Last Modified: Tue, 21 Mar 2023 00:45:48 GMT  
		Size: 26.8 MB (26750227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1ed2a27cc3d05c548d18f1adbd5016ca69c7650456c8b28d0866993a5e9a26`  
		Last Modified: Tue, 21 Mar 2023 00:45:46 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfce4b72ead99df18cd6dc867376b26fb6ce52a4c44fc816fd17a3069b9d149f`  
		Last Modified: Tue, 21 Mar 2023 00:45:46 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1a3b01c4835b559e4f303ec9fdabee9e1d553f03b01c382d4995b983071b9a`  
		Last Modified: Tue, 21 Mar 2023 00:45:46 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7073f73a1f90d4d3ef406061a6804f6c43ad60600c417d5f298c83b7c9d53e4e`  
		Last Modified: Tue, 21 Mar 2023 00:45:46 GMT  
		Size: 833.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
