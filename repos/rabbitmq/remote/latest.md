## `rabbitmq:latest`

```console
$ docker pull rabbitmq@sha256:ce3956cfb0ff31b444e3bf9a69076a32f65da1b4dcaac45bfa8ddf396a724c48
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 9
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `rabbitmq:latest` - linux; amd64

```console
$ docker pull rabbitmq@sha256:8d108329a660f1d9aa5d83e8bc503f024570e20f6cdbce3df5cb9f262174028b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105713469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c985c7f8894e8f65ee4841f0440fceb2bcc2b6225b893794ce16865d280ecf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 04 Aug 2023 04:52:57 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:52:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:52:59 GMT
ADD file:bb1fa1d9d012ae826908afdce8c9fa2feebf221b2ab032e1535255905144411a in / 
# Fri, 04 Aug 2023 04:53:00 GMT
CMD ["/bin/bash"]
# Thu, 24 Aug 2023 23:29:02 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 24 Aug 2023 23:29:02 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
ENV RABBITMQ_VERSION=3.12.4
# Thu, 24 Aug 2023 23:29:02 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 24 Aug 2023 23:29:02 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 24 Aug 2023 23:29:02 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Aug 2023 23:29:02 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
RUN gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 24 Aug 2023 23:29:02 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 24 Aug 2023 23:29:02 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 24 Aug 2023 23:29:02 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Aug 2023 23:29:02 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 24 Aug 2023 23:29:02 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:b237fe92c4173e4dfb3ba82e76e5fed4b16186a6161e07af15814cb40eb9069d`  
		Last Modified: Fri, 04 Aug 2023 05:10:57 GMT  
		Size: 29.5 MB (29536501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:00e2cfb5ec44cfa488b9f01da6da447138e516418fc9244cc0c1d3482c0b7ed6`  
		Last Modified: Sat, 26 Aug 2023 01:01:25 GMT  
		Size: 429.1 KB (429117 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f8bb1fbaa2faf822e9d9af07305eec80b07b1926afbd193984e0ba28ace27a2`  
		Last Modified: Sat, 26 Aug 2023 01:01:24 GMT  
		Size: 10.1 KB (10147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34d6b4a95d7711e19119dde139fa6d1bd778cff5a746f4f9d668a20f25017c85`  
		Last Modified: Sat, 26 Aug 2023 01:01:27 GMT  
		Size: 55.2 MB (55161032 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebf2e15c53f4618a5fbffa05f77639d2555df95cafdf91c9e06dd582dbd29d73`  
		Last Modified: Sat, 26 Aug 2023 01:01:24 GMT  
		Size: 10.8 KB (10842 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:988725783fba1e87a16da7e280e7f9aa83f948365bbc56f187d5013b4e8de340`  
		Last Modified: Sat, 26 Aug 2023 01:01:27 GMT  
		Size: 20.6 MB (20564083 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e13c78ddfc234eb3e5c1f8df05324395f93d5c771fbca5ce2ffe91c2c1d320e2`  
		Last Modified: Sat, 26 Aug 2023 01:01:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73feae46200861ccbb3cabd3d4b3a735e87e107251294466c0b27045db9899a4`  
		Last Modified: Sat, 26 Aug 2023 01:01:26 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3bb37365844e2a20d472401747bba83812c677960f75a23d1256a6ff538ef4ab`  
		Last Modified: Sat, 26 Aug 2023 01:01:27 GMT  
		Size: 618.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2893efd85b51671740bdd10d058649e4dc9efe642366e00a19100bdb0ee19336`  
		Last Modified: Sat, 26 Aug 2023 01:01:27 GMT  
		Size: 832.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:latest` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:7de7bea9536bdc09e11650efb760f6c69e599f2304c4268cc884494824213f4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1913317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed5212912cee79576bda6a74dc8ecbd004be4235e150c323d06be0eedba3f7e8`

```dockerfile
```

-	Layers:
	-	`sha256:b1042bfe590e53f7a8826f4f3bed6e5998479596e2e4fc7b1b56c27a1f56169d`  
		Last Modified: Sat, 26 Aug 2023 01:01:24 GMT  
		Size: 1.9 MB (1853756 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:14674c180f95235c68533fb436f7481316980d10deb324702a37fc5798c3a1a4`  
		Last Modified: Sat, 26 Aug 2023 01:01:24 GMT  
		Size: 59.6 KB (59561 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:latest` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:85459ff6dbced849c92d5fd82c14d6cc6ce41fe3c061312b6f9b1e6b877b3ffc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.3 MB (90306948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31b4a886742b3bbd52800066ce56a568f20f33d64a18bfe6ca6dd9aebc135917`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Wed, 07 Jun 2023 11:43:59 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Wed, 07 Jun 2023 11:43:59 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Wed, 07 Jun 2023 11:43:59 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Wed, 07 Jun 2023 11:43:59 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Wed, 07 Jun 2023 11:43:59 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Wed, 07 Jun 2023 11:43:59 GMT
ENV RABBITMQ_VERSION=3.12.0
# Wed, 07 Jun 2023 11:43:59 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 07 Jun 2023 11:43:59 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 07 Jun 2023 11:43:59 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Jun 2023 11:43:59 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Wed, 07 Jun 2023 11:43:59 GMT
RUN gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Wed, 07 Jun 2023 11:43:59 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Wed, 07 Jun 2023 11:43:59 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 07 Jun 2023 11:43:59 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 07 Jun 2023 11:43:59 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 07 Jun 2023 11:43:59 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Wed, 07 Jun 2023 11:43:59 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 07 Jun 2023 11:43:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Jun 2023 11:43:59 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Wed, 07 Jun 2023 11:43:59 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea55c791dc3b03c096321b91f121ca2a705c4743ac6977c8821f6911e288a2a3`  
		Last Modified: Fri, 16 Jun 2023 01:07:12 GMT  
		Size: 391.5 KB (391474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c211f3f9b240b81388e1d6605657c90108ec1d4c3750761c270f75a06939a333`  
		Last Modified: Fri, 16 Jun 2023 01:07:11 GMT  
		Size: 10.1 KB (10147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5efb30d20d0ca9fdd974e99b00dff7096808f99c17a5364c7e4994d1f6d1c86`  
		Last Modified: Fri, 16 Jun 2023 01:07:17 GMT  
		Size: 44.0 MB (43956436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae4a430e86c33f44ad81570e09f4932d29d421df268835a8ea9c98ce8f59377`  
		Last Modified: Fri, 16 Jun 2023 01:07:11 GMT  
		Size: 10.9 KB (10909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6513dd9ce3f15eb5e52257a871b0c23f4770acfb72949f3cb5f8036055832334`  
		Last Modified: Fri, 16 Jun 2023 01:07:12 GMT  
		Size: 21.3 MB (21347114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9253ebdbbacb15acd9019018e55f86d1b12df4ee84ddda44b0fd51a84fde2b3`  
		Last Modified: Fri, 16 Jun 2023 01:07:10 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83df928b43f09213834abc7ea11c3f12d17082b80373c2f2639ce7b2b3f21701`  
		Last Modified: Fri, 16 Jun 2023 01:07:10 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de163b85ffdf251371f1d892d5eb7df0c5739120b3f64615255447e854a88b4`  
		Last Modified: Fri, 16 Jun 2023 01:07:10 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ec308b6b71f90921dbaacb3181f842e5283371c25f5a813c205f3d2d998507`  
		Last Modified: Fri, 16 Jun 2023 01:07:10 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:0cd0b79d23e9acb8e9ba4a9930e664bdb42fbf6f498d1ba198af72398a797e7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100617334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fb8a2499646fdd54bf272cff5c96525a8a6db032a2aceba4d98b6d4b5cb8a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 04 Aug 2023 04:51:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:51:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:51:18 GMT
ADD file:5cf7797cf86362218d2bd85debeff136ee897af7eef95a0b8baab9f9457c3e89 in / 
# Fri, 04 Aug 2023 04:51:18 GMT
CMD ["/bin/bash"]
# Thu, 17 Aug 2023 23:05:26 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 17 Aug 2023 23:05:26 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
ENV RABBITMQ_VERSION=3.12.3
# Thu, 17 Aug 2023 23:05:26 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 17 Aug 2023 23:05:26 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 17 Aug 2023 23:05:26 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 23:05:26 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
RUN gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 17 Aug 2023 23:05:26 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 17 Aug 2023 23:05:26 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 17 Aug 2023 23:05:26 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Aug 2023 23:05:26 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 17 Aug 2023 23:05:26 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:db76c1f8aa176de7f2698c761088ac1e18cdbbafa6210e405f310221c7a9ea6a`  
		Last Modified: Fri, 04 Aug 2023 05:11:04 GMT  
		Size: 27.3 MB (27347607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6031d0cc9c26673046f8416a6ff4f25de728d22001a66acbbce19ad088bcb036`  
		Last Modified: Thu, 17 Aug 2023 00:56:26 GMT  
		Size: 411.1 KB (411076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1dbfca14fbe36c0fb8527024e0700b3e61ea3b46610991704770a0f60cc43f5`  
		Last Modified: Thu, 17 Aug 2023 00:56:26 GMT  
		Size: 10.1 KB (10147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:928717ebb726f6a6f14169c1e923798de763852b9cad93e3157b1f719a8b494e`  
		Last Modified: Thu, 17 Aug 2023 02:03:55 GMT  
		Size: 52.4 MB (52364797 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6efcfce051baedc255b58a5f8a6995feda3b9e35cfa853a9e16937dc9bba541d`  
		Last Modified: Thu, 17 Aug 2023 02:03:52 GMT  
		Size: 10.8 KB (10802 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:999424153211737b7eda92488b8e574fa4651194e0716517551c8183ee483555`  
		Last Modified: Mon, 21 Aug 2023 23:19:20 GMT  
		Size: 20.5 MB (20471161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13cb700939fec897a7857d36ae7f51085760ad54da3352ce99db47a9f664d276`  
		Last Modified: Mon, 21 Aug 2023 23:19:19 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f7e4481ce591c0b40747fc6ab4d9a1f49959533d3a799efda35913fc52c5830`  
		Last Modified: Mon, 21 Aug 2023 23:19:19 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:252eb2ea5a6122920d2d2d6e44593d386875ea88dd1be1e42bfc4b8ae0a92e7a`  
		Last Modified: Mon, 21 Aug 2023 23:19:19 GMT  
		Size: 618.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4b2430a466760dca2d32c71f44654b61b68f145b475ea44bb5be74a42212230`  
		Last Modified: Mon, 21 Aug 2023 23:19:20 GMT  
		Size: 831.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:latest` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:c6befa3cbfcedca07f74b61c7645ecb7e9682419948d2422661f2df82485c7d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1913531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f3e9bc42260f840c2b0a1b6bedc099be063413ba2d4eaf20baa0a62458997ba`

```dockerfile
```

-	Layers:
	-	`sha256:b4dd1e956ddd98c086657710ab7e2a61c7a8cb14658279c35c076330f97194e1`  
		Last Modified: Mon, 21 Aug 2023 23:19:19 GMT  
		Size: 1.9 MB (1854123 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9c70b7355e627c1fea887eaaa0acfb211e49c35258519985455aa315d99b90ff`  
		Last Modified: Mon, 21 Aug 2023 23:19:19 GMT  
		Size: 59.4 KB (59408 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:latest` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:d28b80040963dc901b47e9ea971f71897cbeb6643e0a8955c2c1d11de8d97fcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.5 MB (105451425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fea28d056bebae3f13b54f4d04c94545653ae7d8d008c71d227a745056257ca5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 04 Aug 2023 04:56:16 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:56:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:56:20 GMT
ADD file:0e9b840e6824ee009acbddc2d337fd5083ebe606393cf7532cdca4f108813ca3 in / 
# Fri, 04 Aug 2023 04:56:20 GMT
CMD ["/bin/bash"]
# Thu, 17 Aug 2023 23:05:26 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 17 Aug 2023 23:05:26 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
ENV RABBITMQ_VERSION=3.12.3
# Thu, 17 Aug 2023 23:05:26 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 17 Aug 2023 23:05:26 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 17 Aug 2023 23:05:26 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 23:05:26 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
RUN gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 17 Aug 2023 23:05:26 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 17 Aug 2023 23:05:26 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 17 Aug 2023 23:05:26 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 17 Aug 2023 23:05:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Aug 2023 23:05:26 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 17 Aug 2023 23:05:26 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:e6140760330bb52aa780087331e6207156dc1d36e412010f0de6faacee7817be`  
		Last Modified: Fri, 04 Aug 2023 05:11:17 GMT  
		Size: 34.6 MB (34590887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e3215a3a38c6e486070118522e82aa24683bf47f4174e2bf49384ec1aaeff0dd`  
		Last Modified: Thu, 17 Aug 2023 10:42:03 GMT  
		Size: 463.8 KB (463751 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:beca762f9fa3820d6df5fe10660121405e21725d290c7b83f78cf410f0a2c136`  
		Last Modified: Thu, 17 Aug 2023 10:42:02 GMT  
		Size: 10.1 KB (10147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5c95d765c6bcbf3ae66650276285cdbf495c8e4654858ab592b6208e9bd3693`  
		Last Modified: Thu, 17 Aug 2023 13:59:13 GMT  
		Size: 49.9 MB (49877989 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:252aea12bc8625f6a09239ea1243eb0faf186913220a883f1c9158a9d8dcf283`  
		Last Modified: Thu, 17 Aug 2023 13:59:09 GMT  
		Size: 10.8 KB (10769 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7fd6148edc808683240ff61e76ea87b83257be64984ff2003b34af2dd31f7c0`  
		Last Modified: Mon, 21 Aug 2023 23:30:53 GMT  
		Size: 20.5 MB (20496135 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:96c0f2ad93749ab3f4ffc34272a1144c31ff251cd0882d6a179e93e939ce0a01`  
		Last Modified: Mon, 21 Aug 2023 23:30:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e25cee5549b628eb689fe6ff5ccfba59cff78213a439d6b90960b49ea54e8c41`  
		Last Modified: Mon, 21 Aug 2023 23:30:51 GMT  
		Size: 108.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e366804f36bb59910c3c694d1f4b012bc3d69b8a44b67eb47de49603cae9d0fc`  
		Last Modified: Mon, 21 Aug 2023 23:30:52 GMT  
		Size: 620.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9bcb353f727d8f64bd73aec4cc141d2c208d0a74a11c9e00dcf04b4513e67a89`  
		Last Modified: Mon, 21 Aug 2023 23:30:52 GMT  
		Size: 831.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:latest` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:60846b526daee8405bdbed3175c063cf3d0cbeda10c4fc9c1d3c7d5a0308a492
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1917902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3fd5cfa19a9deba3f41ff7129d978abbd92a806748217bb207a3d87cba424d1`

```dockerfile
```

-	Layers:
	-	`sha256:1d61997e4de0999a15722e302eff236c40d044b0a388c073f60b716e8d758898`  
		Last Modified: Mon, 21 Aug 2023 23:30:52 GMT  
		Size: 1.9 MB (1858448 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:50b29acf8953dd34b223146af866f88828a0e6f36e7d8e09ba2fbfcad7235c6f`  
		Last Modified: Mon, 21 Aug 2023 23:30:51 GMT  
		Size: 59.5 KB (59454 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:latest` - linux; s390x

```console
$ docker pull rabbitmq@sha256:54c7a14a744b927c6184b08fe925e55c69e719cf0abe04d83d18012804b94576
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95583824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a012ea7f63678d5f38de355ec32d77468079481be9139fa432e3fd14a073489f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:16 GMT
ADD file:d5b5687c046ca0689ccc4f42ddcc27543404ae2273aa12241e6636a2b3d675df in / 
# Fri, 04 Aug 2023 05:03:16 GMT
CMD ["/bin/bash"]
# Thu, 24 Aug 2023 23:29:02 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 24 Aug 2023 23:29:02 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		ldconfig; 	sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		groupadd --gid 999 --system rabbitmq; 	useradd --uid 999 --system --home-dir "$RABBITMQ_DATA_DIR" --gid rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
ENV RABBITMQ_VERSION=3.12.4
# Thu, 24 Aug 2023 23:29:02 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 24 Aug 2023 23:29:02 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 24 Aug 2023 23:29:02 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Aug 2023 23:29:02 GMT
RUN set -eux; 	export DEBIAN_FRONTEND=noninteractive; 	apt-get update; 	apt-get install --yes --no-install-recommends 		ca-certificates 		gosu 		tzdata 	; 	gosu nobody true; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get install --yes --no-install-recommends 		gnupg 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --progress dot:giga --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	gosu rabbitmq rabbitmqctl help; 	gosu rabbitmq rabbitmqctl list_ciphers; 	gosu rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
RUN gosu rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 24 Aug 2023 23:29:02 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 24 Aug 2023 23:29:02 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 24 Aug 2023 23:29:02 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 24 Aug 2023 23:29:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Aug 2023 23:29:02 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 24 Aug 2023 23:29:02 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:bdf265a933ffdd52ec28f006765d35d4119c012d520b564de8ea1b8cdc6c269f`  
		Last Modified: Fri, 04 Aug 2023 05:11:24 GMT  
		Size: 28.0 MB (28013360 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4eeb1731293e2e3ac5db1d7711621ddd2858b6a1890a63994c3f17c40c21d39`  
		Last Modified: Wed, 16 Aug 2023 21:31:44 GMT  
		Size: 432.4 KB (432415 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:017bc013e823a52bec726dcf5899f3beb3b23b07ea1dbe2ccdddd975500e5856`  
		Last Modified: Wed, 16 Aug 2023 21:31:43 GMT  
		Size: 10.2 KB (10150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c45fd6b2f65c92a142bb2eff9c266426e4069a28d1dc527dacf2cd08f93d58a9`  
		Last Modified: Wed, 16 Aug 2023 21:43:06 GMT  
		Size: 46.6 MB (46580780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c76ff164b79f316320550f396a814b54b3c2fb5ed768fd51ff1d9e9339e7bd8`  
		Last Modified: Wed, 16 Aug 2023 21:43:04 GMT  
		Size: 10.8 KB (10841 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d329502d70bd3f5084ef75bdae6686199b7ca449e4f4c35720f764c8d2222929`  
		Last Modified: Sat, 26 Aug 2023 02:24:36 GMT  
		Size: 20.5 MB (20534530 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c732bb98fc2314552032a2ab276b14bd63ed1199a7b9bb36f720142551fef3b`  
		Last Modified: Sat, 26 Aug 2023 02:24:35 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b2df12578e0d57d1898dc8124e519331d68f258b60e2eb775d06075d7335eef1`  
		Last Modified: Sat, 26 Aug 2023 02:24:35 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:687c7e0c3d921287cbde0f49d8657ed041dad6a3d6865a60e3154c14f83c7854`  
		Last Modified: Sat, 26 Aug 2023 02:24:35 GMT  
		Size: 619.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07da2f3bb6bc7def69550fc3bddbf1b0533335c8de05ef94baedeaadddfeef68`  
		Last Modified: Sat, 26 Aug 2023 02:24:35 GMT  
		Size: 831.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:latest` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:50bbf4b1d7a999937a09d4b9699743e53b47e13b7bf5f50189a95cbad6fca323
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1914155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c49de391d2dcb4b0c3491c927bb7e86bd6529d35aa6f1c28b18b10e4568d3d`

```dockerfile
```

-	Layers:
	-	`sha256:1639b2e35753991ed4bd4b879f167fa7bab386dc47dbde14eb336426dac41314`  
		Last Modified: Sat, 26 Aug 2023 02:24:35 GMT  
		Size: 1.9 MB (1854755 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eadb2dc6653cc1cd25320d0d3a5ab67c653b4e0ee823e8addd1dbebbd033acfb`  
		Last Modified: Sat, 26 Aug 2023 02:24:34 GMT  
		Size: 59.4 KB (59400 bytes)  
		MIME: application/vnd.in-toto+json
