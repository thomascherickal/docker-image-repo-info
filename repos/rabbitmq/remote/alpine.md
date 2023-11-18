## `rabbitmq:alpine`

```console
$ docker pull rabbitmq@sha256:b381171138c63aee1c804a03c7008548aa272b671c6566aebfe4c86401dca1e4
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 13
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `rabbitmq:alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:157e239ad75922d8fceb3e7613296146b3af1d1a4b9fd377426980c6c9370ebc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (71023532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f07e801679b733b3d8c050da9c3dc47598084f8223d6472d591fc46b2e514e3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 17 Nov 2023 12:05:25 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 17 Nov 2023 12:05:25 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 17 Nov 2023 12:05:25 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_VERSION=3.12.9
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Nov 2023 12:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.9","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.9?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 17 Nov 2023 12:05:25 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 17 Nov 2023 12:05:25 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Nov 2023 12:05:25 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 17 Nov 2023 12:05:25 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:998a810efc3af272610df3e6c3f6aedf52c9a8c4df3f0dc28f24d20152d18020`  
		Last Modified: Sat, 18 Nov 2023 00:23:15 GMT  
		Size: 40.1 MB (40076553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5441979ce9739b337e51023b5aa68f9e5765395c931f1804be4786a5dfa7e559`  
		Last Modified: Sat, 18 Nov 2023 00:23:14 GMT  
		Size: 389.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea4f1a1db6fc681378a591a6d024b70445e60dd8bae28a26bd187d881c310899`  
		Last Modified: Sat, 18 Nov 2023 00:23:15 GMT  
		Size: 7.6 MB (7550206 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ef59d46d601febc480c116bc9e15d19c2bfa0466c31b82b12fe4ddd12dcf5c4`  
		Last Modified: Sat, 18 Nov 2023 00:23:14 GMT  
		Size: 390.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce6b5a8be69c71c7227c731fc99e23240633529b6937051599a9e0a7545cff4f`  
		Last Modified: Sat, 18 Nov 2023 00:23:15 GMT  
		Size: 2.3 MB (2297442 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51ac8c2d5f62b4922e84c66c8c37a69a1001056afb3436ee0bee29c6471f792e`  
		Last Modified: Sat, 18 Nov 2023 00:23:16 GMT  
		Size: 17.7 MB (17694835 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8ecf82e3ef9cde71a243ae3bfed661013ace37e858a3eac0e3aacbcd2922b68`  
		Last Modified: Sat, 18 Nov 2023 00:23:16 GMT  
		Size: 190.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f5b8c90441def8b0c617aa2b7f8b7bc66a73fbfcbea166a3704bba592950fad`  
		Last Modified: Sat, 18 Nov 2023 00:23:16 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:93b6664adac4b2c07814c0746b3051748dbb3e8f543ad35641bf07e71cf0bd3f`  
		Last Modified: Sat, 18 Nov 2023 00:23:17 GMT  
		Size: 622.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1c030eff7644e775ed67bc2142cde245b157b3b4621a0b6d38440395146a08c1`  
		Last Modified: Sat, 18 Nov 2023 00:23:17 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:ce895aaa36cf31a179cd591a0aa220410d0dc2bec6d6e66b8b5d1dbf1f88bbb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5390423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a641b4755fb76fbbcefad86ca42dcca49f29fd2e4f59fce4fca859b128f23b1a`

```dockerfile
```

-	Layers:
	-	`sha256:8542ff9bb68da64a268d5744ba6c9fdcb5f4c93fc817e064db3846158626e10e`  
		Last Modified: Sat, 18 Nov 2023 00:23:14 GMT  
		Size: 760.4 KB (760353 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:00dd5083a3625e93a044071bb3525e21129bedd9e5dad566aa92f2bb0df29a23`  
		Last Modified: Sat, 18 Nov 2023 00:23:14 GMT  
		Size: 2.3 MB (2280847 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:73b527f55172b41defd6b0bbdc9a7234391eea5adbd356d6c64a5449a2dc42db`  
		Last Modified: Sat, 18 Nov 2023 00:23:14 GMT  
		Size: 2.3 MB (2279957 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8149f2fb374fb59d92382cc3832c786629ece193ea9f6ab68fbcfa1f42279d40`  
		Last Modified: Sat, 18 Nov 2023 00:23:14 GMT  
		Size: 69.3 KB (69266 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:c76117fc2d9aa0e8aa8ffd19315f8cfb21ffc70671d9b8bbf94fa9d7318a5a26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61026840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d85125073720738106ac4a523456eae3f0235ea4abe9352fbcc99dba566a1f8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 17 Nov 2023 12:05:25 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 17 Nov 2023 12:05:25 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 17 Nov 2023 12:05:25 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_VERSION=3.12.9
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Nov 2023 12:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.9","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.9?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 17 Nov 2023 12:05:25 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 17 Nov 2023 12:05:25 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Nov 2023 12:05:25 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 17 Nov 2023 12:05:25 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63534738a5c56b76c8f1d4065951fb85d4a64e9a1624d3f96f9f79e31334744`  
		Last Modified: Sat, 18 Nov 2023 00:23:09 GMT  
		Size: 32.4 MB (32388815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a09c01244848bb9521601c8201eb4e1f00042e0a8db88d66d2acc29802414e`  
		Last Modified: Sat, 18 Nov 2023 00:23:03 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee68b5ff2d0bee3664d23cc949f3048ba7f91993e75bd88de259eb0c0a1c3e9`  
		Last Modified: Sat, 18 Nov 2023 00:23:05 GMT  
		Size: 6.4 MB (6382861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5a329eacce4ee0f079d1d605a030240f4878a148f4d76ded34ca732fc1a9c8`  
		Last Modified: Sat, 18 Nov 2023 00:23:04 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d375284e26a52a0a14494c19b6a52286906c5646343ae93ebe38cfd6c1e04c04`  
		Last Modified: Sat, 18 Nov 2023 00:23:03 GMT  
		Size: 1.4 MB (1412509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19970a65d067d42c5c4790c683b23681ce7a9e5fabeb958add63bd14ca415bf`  
		Last Modified: Sat, 18 Nov 2023 00:23:03 GMT  
		Size: 17.7 MB (17694839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae400199c2e89eb04dd778dda048cbda8f2e19b097af5f094c51123a473cbdb7`  
		Last Modified: Sat, 18 Nov 2023 00:23:01 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8f016add640ff118a7f444325b0c8c5c96eb943f356f21a07ac06495d9579c`  
		Last Modified: Sat, 18 Nov 2023 00:23:01 GMT  
		Size: 109.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9de5c1deab1091d3bac6603370c727a84b8669f162ed72c0fe5137214e06cec`  
		Last Modified: Sat, 18 Nov 2023 00:23:01 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277c129b39e86c4cab4d880c469d8c48f384c2fabfe1485056b9d348b79488ce`  
		Last Modified: Sat, 18 Nov 2023 00:23:01 GMT  
		Size: 829.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:bbfb5ad1ea80321418dc93f6226c48dac90748e740feb5ca96c3b618dd19cb39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60251039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf20af7a561817b5109d81177f9a0040455ec3d81ec3494b85329390aaa73fed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 17 Nov 2023 12:05:25 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 17 Nov 2023 12:05:25 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 17 Nov 2023 12:05:25 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_VERSION=3.12.9
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Nov 2023 12:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.9","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.9?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 17 Nov 2023 12:05:25 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 17 Nov 2023 12:05:25 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Nov 2023 12:05:25 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 17 Nov 2023 12:05:25 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f7f57e652bf551759f9169cf7cbc65a05f05678d004fb4ecf84bbcb2ce36eb87`  
		Last Modified: Fri, 27 Oct 2023 17:51:19 GMT  
		Size: 32.3 MB (32271017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f327defd88b9aa4fddd69dee7ffebd3b13314b7841fc6c136fa4838e309016d`  
		Last Modified: Fri, 27 Oct 2023 17:51:16 GMT  
		Size: 394.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f463091713f46b393a8ec9a3be629a5c67b73263f8d101dd87a6ec7599de0249`  
		Last Modified: Fri, 27 Oct 2023 17:51:18 GMT  
		Size: 6.1 MB (6082548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9385564d576ce6ba34e74067f4819742b82ac5ab8f4fa3f3b39834b27d0eefe2`  
		Last Modified: Fri, 27 Oct 2023 17:51:17 GMT  
		Size: 390.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f4080c6f809b4aadf1a7dcb3b7042f5ba8d014b7e1bf1128277f41807cb4db2`  
		Last Modified: Fri, 27 Oct 2023 17:51:18 GMT  
		Size: 1.3 MB (1300444 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b3295011c160ef017437099dca62cfa75e5fa35df0c1f314bf17424b9c9476c8`  
		Last Modified: Sat, 18 Nov 2023 00:37:43 GMT  
		Size: 17.7 MB (17694595 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3989fbf2a877a8f2dc380457e70529ee99e7ca7a3241ccbe18e43381a0fa7c0c`  
		Last Modified: Sat, 18 Nov 2023 00:37:42 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b086846583e1c25e9678a6db1f58720c428f550f6a99f92e24ef43cdbbb00e58`  
		Last Modified: Sat, 18 Nov 2023 00:37:42 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:428ef4a043450834b6fac2d47fcd194416a9af276484b50174ecdd14bdbab997`  
		Last Modified: Sat, 18 Nov 2023 00:37:44 GMT  
		Size: 617.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a587884cf4355068643c8c7addfa9b8c57140a31695d606580262415d2a0107a`  
		Last Modified: Sat, 18 Nov 2023 00:37:43 GMT  
		Size: 827.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:7a4abd05fe3ea3c5c7e78e5fab9ab3f487c707d3908f46fd0efa2e43c5b86ca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5229854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9dbaeafdd8a5b31a8a25682df9e4619882c1e8133b70132c82e36039d7285a7`

```dockerfile
```

-	Layers:
	-	`sha256:100fe7e0cafce79b5e5f4205f15763ddc65a77487b94d73fd36092c4fe388fc5`  
		Last Modified: Sat, 18 Nov 2023 00:37:42 GMT  
		Size: 756.3 KB (756325 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5fd6f2a1bd42ec41f758d2bd12a25bf568b1636df91936ffb8a297a6d22a4141`  
		Last Modified: Sat, 18 Nov 2023 00:37:42 GMT  
		Size: 2.2 MB (2202553 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ea993f3088896b11b8c254059c57f7911a78bba1e0760b686aac8ca50aec3e3e`  
		Last Modified: Sat, 18 Nov 2023 00:37:42 GMT  
		Size: 2.2 MB (2201663 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:707bac35b5d835eeaae418f15cf8289727e78ed14e7d2290b122a3d240b358e3`  
		Last Modified: Sat, 18 Nov 2023 00:37:42 GMT  
		Size: 69.3 KB (69313 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:22f0aad77f97901ebac39a382c5fe4c8120d6caf5ef296a6aa25476154ef1687
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68419489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6dd7a8c8c7304459cf3e3ea7333ad20e2a4e37ff4c567b67199fdc942ae7fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 17 Nov 2023 12:05:25 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 17 Nov 2023 12:05:25 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 17 Nov 2023 12:05:25 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_VERSION=3.12.9
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Nov 2023 12:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.9","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.9?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 17 Nov 2023 12:05:25 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 17 Nov 2023 12:05:25 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Nov 2023 12:05:25 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 17 Nov 2023 12:05:25 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:196d3fd38f39c8756a92c06767d0da13ac0823d00198f79d9bce4fe20e2a3a6a`  
		Last Modified: Fri, 27 Oct 2023 17:52:52 GMT  
		Size: 37.9 MB (37874049 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf86d5275580d5e06411a30f007c63c83d1a18d534bebfaa25bde9157037a08a`  
		Last Modified: Fri, 27 Oct 2023 17:52:49 GMT  
		Size: 392.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99910fe121b7470d23958b20a4288b048b92ec93dc5bfadbd8e8091998e5afba`  
		Last Modified: Fri, 27 Oct 2023 17:52:50 GMT  
		Size: 7.1 MB (7147436 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f1b5b553370dd9791261eb07815e1a7b5468dae1f8a95d4b73861744cbac6ea`  
		Last Modified: Fri, 27 Oct 2023 17:52:50 GMT  
		Size: 387.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89b81e0e6313a3ead53ce1edcedfe133674e1a67e490963067c485e9d6d24ff7`  
		Last Modified: Fri, 27 Oct 2023 17:52:51 GMT  
		Size: 2.4 MB (2368792 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2ecc34141d100dd947c89c1913a82c944834b3671024647921b02502688fd12`  
		Last Modified: Sat, 18 Nov 2023 00:36:45 GMT  
		Size: 17.7 MB (17694854 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fa19e5d980acbdb641a68e111067091304cce780e515f750a914c3618e116f5`  
		Last Modified: Sat, 18 Nov 2023 00:36:43 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b85a9fcb568f484bc027f21f7b3c54f3adfd6373e9610e4ec8635dd01038eb7`  
		Last Modified: Sat, 18 Nov 2023 00:36:43 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:74b17befc676eefedf6d012e2a87a974eb01554586af3b34327cd995404fc7e7`  
		Last Modified: Sat, 18 Nov 2023 00:36:43 GMT  
		Size: 620.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0bd8d0f298f7486d1dcb728411bc31e0d4f8a0e6ff23a17f633f017560997e4d`  
		Last Modified: Sat, 18 Nov 2023 00:36:44 GMT  
		Size: 828.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:cffddae2f2648e7271759dc0448e637ff414fbdc5c8880bc1311d1fe7b519ddb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5422534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57819afbfc626cb71d7b7816bfc0f0c9e7ee8119697f3d33f106f932d14e051c`

```dockerfile
```

-	Layers:
	-	`sha256:e1e92bdaab78154263a4a5bbe66180219b485bf7b350fb75a8ee6ecb279a9c00`  
		Last Modified: Sat, 18 Nov 2023 00:36:43 GMT  
		Size: 760.4 KB (760364 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8e8d081a5591b7a1ab7253f930b8b5ec68428b670345b2e08ee7092043b7ae7b`  
		Last Modified: Sat, 18 Nov 2023 00:36:43 GMT  
		Size: 2.3 MB (2296975 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:484fa311ec45139d76e4476e59ee666e4dea6cead02561404eb16f4b6142a0f9`  
		Last Modified: Sat, 18 Nov 2023 00:36:43 GMT  
		Size: 2.3 MB (2296085 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:36ebec83986eaca6602b6f310925c46b7d7eb90902609733ab8547b56325fe2f`  
		Last Modified: Sat, 18 Nov 2023 00:36:43 GMT  
		Size: 69.1 KB (69110 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:4c3f610f79a094748981d5dd6f3a1acae00923b064cb47f16683383e10e365ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62439481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d624f09c9fcc2b912bb2a420234e7cb1e144dd161dd24a97df84b607d49c5a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Tue, 31 Oct 2023 17:27:40 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Tue, 31 Oct 2023 17:27:40 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Tue, 31 Oct 2023 17:27:40 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Tue, 31 Oct 2023 17:27:40 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Tue, 31 Oct 2023 17:27:40 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Tue, 31 Oct 2023 17:27:40 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Tue, 31 Oct 2023 17:27:40 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 17:27:40 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 31 Oct 2023 17:27:40 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 31 Oct 2023 17:27:40 GMT
ENV RABBITMQ_VERSION=3.12.8
# Tue, 31 Oct 2023 17:27:40 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 31 Oct 2023 17:27:40 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 31 Oct 2023 17:27:40 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 17:27:40 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.8","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.8?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Tue, 31 Oct 2023 17:27:40 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 31 Oct 2023 17:27:40 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 31 Oct 2023 17:27:40 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 31 Oct 2023 17:27:40 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 31 Oct 2023 17:27:40 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 31 Oct 2023 17:27:40 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 31 Oct 2023 17:27:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 31 Oct 2023 17:27:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Oct 2023 17:27:40 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 31 Oct 2023 17:27:40 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7084bb4371909a4112132e957798d4b5e7b50751077d645e59cd3604215428d2`  
		Last Modified: Wed, 01 Nov 2023 00:08:56 GMT  
		Size: 32.6 MB (32624623 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebc02584d5330d01f3c7b0339d95c22295337150e12f43414aac19939a818970`  
		Last Modified: Wed, 01 Nov 2023 00:08:54 GMT  
		Size: 389.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26efdf331dbe9ea75e002721b8d804e79e40472c57b073a422f626b66d803e06`  
		Last Modified: Wed, 01 Nov 2023 00:08:55 GMT  
		Size: 7.4 MB (7445765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d95f283ef0c9903e04c158f080244f27a16e718c75e46ecb2bca266f1d959cbc`  
		Last Modified: Wed, 01 Nov 2023 00:08:54 GMT  
		Size: 391.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:881f1f4cc75515fc575c3ceb089acc544fc52d98e4a8f8a55ea230ef30f95342`  
		Last Modified: Wed, 01 Nov 2023 00:08:56 GMT  
		Size: 1.4 MB (1401887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ccd41d86339012cc649dd94138a2d35fb741e45f0e9221c50a2256b939c52426`  
		Last Modified: Wed, 01 Nov 2023 00:08:57 GMT  
		Size: 17.7 MB (17728923 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb867b3c114cf41c2f851556efb691b881687e838c3439ec1620e3c9fda0c4d6`  
		Last Modified: Wed, 01 Nov 2023 00:08:56 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97ad88ac80f833d6d54b077df19944255557c71944bff93520129310b5306e5d`  
		Last Modified: Wed, 01 Nov 2023 00:08:57 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e29799fc2d6f3831bf629ad3a67bdf208589d60e9c51490c5303aee3552ee66`  
		Last Modified: Wed, 01 Nov 2023 00:08:57 GMT  
		Size: 617.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e90f15fca4ec148efcff160597b9826ac8803fa5519930724b93aa08e95f48b4`  
		Last Modified: Wed, 01 Nov 2023 00:08:57 GMT  
		Size: 827.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:93aca3e41147cd53b8799d9560d7841a74e7c3ac028db80c58acd2e59f4cad4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 KB (68999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34bb69509fe5c75b80aadde7174872ab1e4d229026d6c9ce297537d6f266c29a`

```dockerfile
```

-	Layers:
	-	`sha256:43d003fcb5a04cfeb673e9901edd25026438627dcaa4b5123b35f0908acfd27b`  
		Last Modified: Wed, 01 Nov 2023 00:08:54 GMT  
		Size: 69.0 KB (68999 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:9c82797f701486c502730c24641c613f0e86fd53191236066e91196730b308fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.3 MB (63331696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f880185da19c9782011de3dbe6a2aae9c0c1148841f627dbe1cda8b1e515f333`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Fri, 17 Nov 2023 12:05:25 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 17 Nov 2023 12:05:25 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 17 Nov 2023 12:05:25 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_VERSION=3.12.9
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Nov 2023 12:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.9","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.9?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 17 Nov 2023 12:05:25 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 17 Nov 2023 12:05:25 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Nov 2023 12:05:25 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 17 Nov 2023 12:05:25 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c683d3bbe8f22650d7212d298915ede8a21140c201e6ca5071a45567baba24af`  
		Last Modified: Fri, 27 Oct 2023 17:36:46 GMT  
		Size: 32.8 MB (32804837 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a763a9de36c15c741c7d357e1c5c520eaff5a227df81f070bc5a0efe2bb5dc0`  
		Last Modified: Fri, 27 Oct 2023 17:36:43 GMT  
		Size: 395.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50e236127e7ef69fa54b3e90d87f61f0cf35855c0d23d1462f90a88e7c49a9e3`  
		Last Modified: Fri, 27 Oct 2023 17:36:44 GMT  
		Size: 8.0 MB (7960983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a2de82464687dcdcea1488224511aaab7c076f9064c4a3104da89b19bc1184d6`  
		Last Modified: Fri, 27 Oct 2023 17:36:43 GMT  
		Size: 393.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed0b96369929775d635052541ff0f4ba42e95cccb22aff4a37b9a18475109b7d`  
		Last Modified: Fri, 27 Oct 2023 17:36:45 GMT  
		Size: 1.5 MB (1522239 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0973975d79795d41bb81effff4ba3954cdcad7f42c98a84b5031eeefea3e398d`  
		Last Modified: Sat, 18 Nov 2023 00:35:19 GMT  
		Size: 17.7 MB (17694590 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b6241f874f3c7a746408d608522f2b29861767f5dbcd29cb28810cb56fd2af8`  
		Last Modified: Sat, 18 Nov 2023 00:35:17 GMT  
		Size: 192.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:358d2e2670930d09208f9ac65d8af899ca7546b8263ba29cead38500c375b57c`  
		Last Modified: Sat, 18 Nov 2023 00:35:18 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a997479eed013cbd81be162a48a10f30ab273c6a326bd5c36dee9503707538d`  
		Last Modified: Sat, 18 Nov 2023 00:35:18 GMT  
		Size: 621.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b39ecefe053da2605543c9fe176a5bf64ac5c2d3ddd0281a92b018b8f067410`  
		Last Modified: Sat, 18 Nov 2023 00:35:19 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:931f0f5cb98e2d0fd681577fd552ec0bc06f362098d0c6c72f84aa31e21c4f54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5373005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f05acc14a9505fcc0fef411ac85efdf5be8de32eb3f2ee20db002c56e19f88d`

```dockerfile
```

-	Layers:
	-	`sha256:847aa805f6b9b0669bdfaba9e43099faf377fe4d96b6fede375509eeae2d6351`  
		Last Modified: Sat, 18 Nov 2023 00:35:18 GMT  
		Size: 754.7 KB (754687 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f2315819f21f20037f19dc7165dfa23e64883e3c2a5cbf7fc93e309f27eb872a`  
		Last Modified: Sat, 18 Nov 2023 00:35:18 GMT  
		Size: 2.3 MB (2275024 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d8f3a89c5bfec99a879cbbca74b02637b198e8a0db81287e8a674f1a40e41a9`  
		Last Modified: Sat, 18 Nov 2023 00:35:18 GMT  
		Size: 2.3 MB (2274134 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6fcf4b9918e20a3a69b31eb4eb311c04fb33419fd00d3aa4e890e47174e87a26`  
		Last Modified: Sat, 18 Nov 2023 00:35:17 GMT  
		Size: 69.2 KB (69160 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:d88a44ab5ac1d633b600be8bd312a9b12905c266bb1a7b0ac6deede93562d11e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61318767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bb7452c06fe053f4284adf67d1de65f4188ed9ea9d5b940ed70833f2ea7804c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 17 Nov 2023 12:05:25 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 17 Nov 2023 12:05:25 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 17 Nov 2023 12:05:25 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_VERSION=3.12.9
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 17 Nov 2023 12:05:25 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Nov 2023 12:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.9","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.9?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 17 Nov 2023 12:05:25 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 17 Nov 2023 12:05:25 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 17 Nov 2023 12:05:25 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 17 Nov 2023 12:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Nov 2023 12:05:25 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 17 Nov 2023 12:05:25 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6d77b2163ba1a757bf93da3911dbd17becdda540d9226ccbf8c91e3e9401caa3`  
		Last Modified: Fri, 27 Oct 2023 19:15:42 GMT  
		Size: 32.5 MB (32478957 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b95da36a2ad80551437da3d0ef4374b2297eb20cb1ede14e47086aad0207831`  
		Last Modified: Fri, 27 Oct 2023 19:15:40 GMT  
		Size: 395.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a57676d109eb9427b6a261221e9c773de3cf251045d6f0bf6049c891b87e9a4`  
		Last Modified: Fri, 27 Oct 2023 19:15:40 GMT  
		Size: 6.4 MB (6432210 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:923cf9c0996c6d47c2b9a291cf3edccd23f01ed3d7b38f61b48e35fa9dea1298`  
		Last Modified: Fri, 27 Oct 2023 19:15:40 GMT  
		Size: 392.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98cf8de2ab34adb2e862fbf73387b9307c0112125e5cd3ccc377d129238927fa`  
		Last Modified: Fri, 27 Oct 2023 19:15:41 GMT  
		Size: 1.5 MB (1495512 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:74474e01ea1b95a95890934126d1a95423df3cb522661cab682917291d06e8ce`  
		Last Modified: Sat, 18 Nov 2023 00:28:52 GMT  
		Size: 17.7 MB (17694454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5dfa171ec4099913d1dc2e0f9de6fc5dc1387e1a6337738e54f6d0a2334337bc`  
		Last Modified: Sat, 18 Nov 2023 00:28:52 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f71fef01ea9f0da25f9bd173c9848c851d67666a793f33f0760bcb30b9178132`  
		Last Modified: Sat, 18 Nov 2023 00:28:52 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5811e6a6647db003cb17773829931d19b276d242564b072280b39867bb4f3ad5`  
		Last Modified: Sat, 18 Nov 2023 00:28:52 GMT  
		Size: 617.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8ae3867e543c731ac1603a8fdf53a54650d20964fc91d9176ac88d00874ecb0d`  
		Last Modified: Sat, 18 Nov 2023 00:28:53 GMT  
		Size: 827.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:94bb1e2998bd82607bf3cc6a0006a29b70e9b39bd586d7ae9c2012367109c36c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5238870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c9cfc5c64bc93d6aa1c79964e0654c8c0a6ae631a4f82344d157b0fb70f59ab`

```dockerfile
```

-	Layers:
	-	`sha256:fc9b336313a624aca4bdb88db8b275d3387ae57a0930e2565efdc62638d093f2`  
		Last Modified: Sat, 18 Nov 2023 00:28:52 GMT  
		Size: 754.7 KB (754653 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:236acb22be95f216da207c3b5dffba4c2c968eec8a0cf240d8cc0009a1ad6f64`  
		Last Modified: Sat, 18 Nov 2023 00:28:52 GMT  
		Size: 2.2 MB (2208004 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4ebdbbf0abbc41bcd3c9c0f4b8aa91f5193a3b9825e78a00765ee47c40abb5ed`  
		Last Modified: Sat, 18 Nov 2023 00:28:52 GMT  
		Size: 2.2 MB (2207114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a0b3109599d11bec399a5947c5090aeaad62a04bc15bb985d8b514b7dfabf155`  
		Last Modified: Sat, 18 Nov 2023 00:28:52 GMT  
		Size: 69.1 KB (69099 bytes)  
		MIME: application/vnd.in-toto+json
