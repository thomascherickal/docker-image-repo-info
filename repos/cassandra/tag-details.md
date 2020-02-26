<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `cassandra`

-	[`cassandra:2`](#cassandra2)
-	[`cassandra:2.1`](#cassandra21)
-	[`cassandra:2.1.21`](#cassandra2121)
-	[`cassandra:2.2`](#cassandra22)
-	[`cassandra:2.2.16`](#cassandra2216)
-	[`cassandra:3`](#cassandra3)
-	[`cassandra:3.0`](#cassandra30)
-	[`cassandra:3.0.20`](#cassandra3020)
-	[`cassandra:3.11`](#cassandra311)
-	[`cassandra:3.11.6`](#cassandra3116)
-	[`cassandra:latest`](#cassandralatest)

## `cassandra:2`

```console
$ docker pull cassandra@sha256:9070ccbe0f1e3cfb34c9406be2c5175a3f7c5885d1c9933bf226d2894deeff4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386

### `cassandra:2` - linux; amd64

```console
$ docker pull cassandra@sha256:0f66081a4e9c465a75ac1c62ffa73edd1cfdaae3440e8a2c8a40e9ec14abc634
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.6 MB (206645392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60547d363254b9a6384ffd567bc65333454aa37d2c652d4380add482c5597cd5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:54:12 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 21:54:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:54:19 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 21:54:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 21:54:32 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 21:54:35 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:55:41 GMT
ENV CASSANDRA_VERSION=2.2.15
# Sat, 01 Feb 2020 21:56:34 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 22x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 21:56:35 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 21:56:35 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 21:56:36 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:56:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 21:56:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:56:37 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 21:56:37 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 21:56:38 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 21:56:38 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7ac5c73a597eb88fd35e6275d72940af5c50458bce1f6ade4d131bd6d0781`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6875e232a43f309c68c25d014efc237ca60c1c5c53bb84e412fceaef1337fc9`  
		Last Modified: Sat, 01 Feb 2020 21:58:41 GMT  
		Size: 5.7 MB (5726879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89165ecf4572ded1baabf4b30188ce50f8f3d83b0ecf031e3e4fd72d488e5cb`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 958.3 KB (958278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ed6a15b620218b60330958b5c4304a9791a9a9bcb843379e41a1d7a9b7b6c`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 18.2 KB (18221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4539ff8905df073aeb921e12822f86dcc68aa201948c6f373afb690c96913ed`  
		Last Modified: Sat, 01 Feb 2020 21:59:46 GMT  
		Size: 177.4 MB (177386880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb87c5da440922b95e4dc163f59870c31bf9d5001b4f801748444938fd03d13`  
		Last Modified: Sat, 01 Feb 2020 21:59:16 GMT  
		Size: 4.9 KB (4889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b2767d4f7fe40fab7be6cb17e463ae3953747dd162ee7afae7d7c3e4f17aba`  
		Last Modified: Sat, 01 Feb 2020 21:59:17 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04db1b4299720eebdc452eaf6b58cca85213db51c44eb71da17a717bff15db7c`  
		Last Modified: Sat, 01 Feb 2020 21:59:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d71f9162e7910e3d11e39d14c34844c1a5684612172951c12a0f78591948f1`  
		Last Modified: Sat, 01 Feb 2020 21:59:16 GMT  
		Size: 22.5 KB (22504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:2` - linux; 386

```console
$ docker pull cassandra@sha256:6549a6ab21da5c260cfeb66a99dfce5efe965609d79cb6f896024c342f027730
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210257672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17a065023984308158dd4d645f556df8ae234a4d9caf9a17ca840c853aee8b50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:03:52 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:04:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:04:00 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:04:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:04:14 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:04:17 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:05:36 GMT
ENV CASSANDRA_VERSION=2.2.15
# Sat, 01 Feb 2020 17:06:38 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 22x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:06:39 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:06:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:06:40 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:06:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:06:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:06:41 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:06:42 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:06:42 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:06:42 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a9c50f749f1de3e365a46e963ec107afea92a353f9b87924b80f24b8e5edf8`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47acd99e08270efe2d386b5d15f509551ba51568a2a87ece42a79e655b1d4ff`  
		Last Modified: Sat, 01 Feb 2020 17:08:29 GMT  
		Size: 6.1 MB (6116093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e2c316cf5968ae3b65e7ac5fb815bf6d859a858c2f545026de5e5b30147721`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 937.8 KB (937830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576efa6035e57b03efee8e68ab486fe466a966565b1bdd538fe532830e437112`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 18.2 KB (18222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066e5cb19e22bb995a394515523f75116f8318ca86aa19a0e422498de896963a`  
		Last Modified: Sat, 01 Feb 2020 17:09:46 GMT  
		Size: 180.0 MB (180002961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dacc7bbd69290735cd9caa8d2dd7896ead6c1d0f862d90682a916964d2f25520`  
		Last Modified: Sat, 01 Feb 2020 17:09:08 GMT  
		Size: 4.9 KB (4887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a070f00393afb15c0a033822dec2bdeed6653f1a8fa518546ad35f30529f0965`  
		Last Modified: Sat, 01 Feb 2020 17:09:08 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf59a36f3a591f08cb1487d4ae780af9af7f0d8719be3acdad0b1ec03db689dc`  
		Last Modified: Sat, 01 Feb 2020 17:09:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46469a5665f4eb0c5d82f00652604498061072a51bacf3f0dadcb78d75f785f1`  
		Last Modified: Sat, 01 Feb 2020 17:09:08 GMT  
		Size: 22.5 KB (22504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:2.1`

```console
$ docker pull cassandra@sha256:41a70f74149c8c2b1d608d6c3d10167a9cab3f7be6bc23a855569dc2a8a250d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `cassandra:2.1` - linux; amd64

```console
$ docker pull cassandra@sha256:9c4b4817e7439762912da12d8553686676bb57e83750b359c5510e572f64dbe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.3 MB (202293528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8378f868ab7e947371c598fb76af3305cbbd5c67deb04123496057dd37f450d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:54:12 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 21:54:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:54:19 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 21:54:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 21:54:32 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 21:54:35 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:54:35 GMT
ENV CASSANDRA_VERSION=2.1.21
# Sat, 01 Feb 2020 21:55:27 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 21x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 21:55:27 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 21:55:28 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 21:55:29 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:55:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 21:55:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:55:30 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 21:55:30 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 21:55:31 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 21:55:31 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7ac5c73a597eb88fd35e6275d72940af5c50458bce1f6ade4d131bd6d0781`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6875e232a43f309c68c25d014efc237ca60c1c5c53bb84e412fceaef1337fc9`  
		Last Modified: Sat, 01 Feb 2020 21:58:41 GMT  
		Size: 5.7 MB (5726879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89165ecf4572ded1baabf4b30188ce50f8f3d83b0ecf031e3e4fd72d488e5cb`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 958.3 KB (958278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ed6a15b620218b60330958b5c4304a9791a9a9bcb843379e41a1d7a9b7b6c`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 18.2 KB (18221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45d5075508f0ab2469a7a60f767e1679598bceabedb5f278abf8ae93242ef7d`  
		Last Modified: Sat, 01 Feb 2020 21:59:12 GMT  
		Size: 173.0 MB (173037214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf9ae877708c26494df5efb441524379c50bc35b8dd6ee0a95b864bf3edd7d5`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 4.7 KB (4670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303133b4934d304dd2be47425dc80f852873b57ba93b1d8162efa4a64b523419`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f07380aafb049d0eb9489117665718a399f5f32b047a9b38e49d3182dfcada8`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2e8d269151fa89c9c81178a1f22f8c33b958914798164575b319470c45cce4`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 20.5 KB (20527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:2.1` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:00c432c70ec35baf9e912e9c55e82301df958a194b5acf54a51d62339d51adef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.7 MB (186693739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28ce1375a1edea917444d8530c11bfdb92dc8e38d3e42294921705e3ffa4aea9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:06:04 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:06:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:06:22 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:06:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:06:43 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:06:47 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:06:48 GMT
ENV CASSANDRA_VERSION=2.1.21
# Sat, 01 Feb 2020 17:08:43 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 21x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:08:46 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:08:48 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:08:49 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:08:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:08:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:08:53 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:08:54 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:08:54 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:08:55 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4555b7d02f2b0f6f8707b27582a305595a30467d8a5836d3099338c98f6dd67f`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4acbf62aed5c4291ff2f7304a5018223f160108cd228d6504407918a4f93eb`  
		Last Modified: Sat, 01 Feb 2020 17:12:13 GMT  
		Size: 5.2 MB (5195126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5c66014f05b2b864abadcb1fbd495e4fc5d72da4a85a3e0f5f890803213218`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 925.7 KB (925700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dba4804d65cfda5823ed59febf14cb99f9ebd1eacc23e11f354e13c04bb3f5c`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 18.2 KB (18219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a251785a60cd104d0711bf21b04d5e74de35ccdb38bb1958fd7e165d4e01603`  
		Last Modified: Sat, 01 Feb 2020 17:12:47 GMT  
		Size: 160.1 MB (160140603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097acef37ed6bf100e6963ed384c3af7b3d1888d84cd3e3a478c6956c367c5c`  
		Last Modified: Sat, 01 Feb 2020 17:12:10 GMT  
		Size: 4.7 KB (4673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09053cbf890231c896294d0a3a8787eeca018bea05523b8ce557cbe73d1ba837`  
		Last Modified: Sat, 01 Feb 2020 17:12:10 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756318e18e359d0294aa1f79cfbd44acdc69fcba8f4624c0e2187d36233eca35`  
		Last Modified: Sat, 01 Feb 2020 17:12:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53cb7b2c3eb3aee379cf77ce9e609facd9d68cbb3d6ceaac79662bb5f3b0c1c`  
		Last Modified: Sat, 01 Feb 2020 17:12:10 GMT  
		Size: 20.5 KB (20527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:2.1` - linux; 386

```console
$ docker pull cassandra@sha256:738ad2b44c2ae0df9e639db76c76fd083d1cf6bcdfaef81770f03117f6fa01ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205892219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff8edf2e9f21c28d295036bdf55d045512b306e63344f7d0412828a151653ca4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:03:52 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:04:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:04:00 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:04:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:04:14 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:04:17 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:04:18 GMT
ENV CASSANDRA_VERSION=2.1.21
# Sat, 01 Feb 2020 17:05:19 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 21x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:05:20 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:05:21 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:05:21 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:05:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:05:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:05:23 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:05:23 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:05:23 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:05:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a9c50f749f1de3e365a46e963ec107afea92a353f9b87924b80f24b8e5edf8`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47acd99e08270efe2d386b5d15f509551ba51568a2a87ece42a79e655b1d4ff`  
		Last Modified: Sat, 01 Feb 2020 17:08:29 GMT  
		Size: 6.1 MB (6116093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e2c316cf5968ae3b65e7ac5fb815bf6d859a858c2f545026de5e5b30147721`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 937.8 KB (937830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576efa6035e57b03efee8e68ab486fe466a966565b1bdd538fe532830e437112`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 18.2 KB (18222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c778e4b2ff1c38d05de6ad5183dd807f6854b71acec36f619dc39664d7d6fab`  
		Last Modified: Sat, 01 Feb 2020 17:09:03 GMT  
		Size: 175.6 MB (175639705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198860589e449d920a3eb83741fe991a36be79458eca60e691214d3a3df297a6`  
		Last Modified: Sat, 01 Feb 2020 17:08:26 GMT  
		Size: 4.7 KB (4670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ab5103c37dfc3caa68015cd57ac4ca82ce44f54a524af1c8345bf9051fd1af`  
		Last Modified: Sat, 01 Feb 2020 17:08:26 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502f26a557eed8b4ac7e53ec9b13e205001c0c30fc93c5df8aaf20b4b8318e60`  
		Last Modified: Sat, 01 Feb 2020 17:08:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2076b1f7acfd2e41ab2929177a77ba1e6785b5cd1af9b56912d8f8dbaf69d3`  
		Last Modified: Sat, 01 Feb 2020 17:08:26 GMT  
		Size: 20.5 KB (20525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:2.1.21`

```console
$ docker pull cassandra@sha256:41a70f74149c8c2b1d608d6c3d10167a9cab3f7be6bc23a855569dc2a8a250d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `cassandra:2.1.21` - linux; amd64

```console
$ docker pull cassandra@sha256:9c4b4817e7439762912da12d8553686676bb57e83750b359c5510e572f64dbe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.3 MB (202293528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8378f868ab7e947371c598fb76af3305cbbd5c67deb04123496057dd37f450d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:54:12 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 21:54:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:54:19 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 21:54:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 21:54:32 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 21:54:35 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:54:35 GMT
ENV CASSANDRA_VERSION=2.1.21
# Sat, 01 Feb 2020 21:55:27 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 21x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 21:55:27 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 21:55:28 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 21:55:29 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:55:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 21:55:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:55:30 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 21:55:30 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 21:55:31 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 21:55:31 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7ac5c73a597eb88fd35e6275d72940af5c50458bce1f6ade4d131bd6d0781`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6875e232a43f309c68c25d014efc237ca60c1c5c53bb84e412fceaef1337fc9`  
		Last Modified: Sat, 01 Feb 2020 21:58:41 GMT  
		Size: 5.7 MB (5726879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89165ecf4572ded1baabf4b30188ce50f8f3d83b0ecf031e3e4fd72d488e5cb`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 958.3 KB (958278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ed6a15b620218b60330958b5c4304a9791a9a9bcb843379e41a1d7a9b7b6c`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 18.2 KB (18221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45d5075508f0ab2469a7a60f767e1679598bceabedb5f278abf8ae93242ef7d`  
		Last Modified: Sat, 01 Feb 2020 21:59:12 GMT  
		Size: 173.0 MB (173037214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf9ae877708c26494df5efb441524379c50bc35b8dd6ee0a95b864bf3edd7d5`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 4.7 KB (4670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303133b4934d304dd2be47425dc80f852873b57ba93b1d8162efa4a64b523419`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f07380aafb049d0eb9489117665718a399f5f32b047a9b38e49d3182dfcada8`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2e8d269151fa89c9c81178a1f22f8c33b958914798164575b319470c45cce4`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 20.5 KB (20527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:2.1.21` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:00c432c70ec35baf9e912e9c55e82301df958a194b5acf54a51d62339d51adef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.7 MB (186693739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28ce1375a1edea917444d8530c11bfdb92dc8e38d3e42294921705e3ffa4aea9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:06:04 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:06:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:06:22 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:06:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:06:43 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:06:47 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:06:48 GMT
ENV CASSANDRA_VERSION=2.1.21
# Sat, 01 Feb 2020 17:08:43 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 21x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:08:46 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:08:48 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:08:49 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:08:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:08:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:08:53 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:08:54 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:08:54 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:08:55 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4555b7d02f2b0f6f8707b27582a305595a30467d8a5836d3099338c98f6dd67f`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4acbf62aed5c4291ff2f7304a5018223f160108cd228d6504407918a4f93eb`  
		Last Modified: Sat, 01 Feb 2020 17:12:13 GMT  
		Size: 5.2 MB (5195126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5c66014f05b2b864abadcb1fbd495e4fc5d72da4a85a3e0f5f890803213218`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 925.7 KB (925700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dba4804d65cfda5823ed59febf14cb99f9ebd1eacc23e11f354e13c04bb3f5c`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 18.2 KB (18219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a251785a60cd104d0711bf21b04d5e74de35ccdb38bb1958fd7e165d4e01603`  
		Last Modified: Sat, 01 Feb 2020 17:12:47 GMT  
		Size: 160.1 MB (160140603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097acef37ed6bf100e6963ed384c3af7b3d1888d84cd3e3a478c6956c367c5c`  
		Last Modified: Sat, 01 Feb 2020 17:12:10 GMT  
		Size: 4.7 KB (4673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09053cbf890231c896294d0a3a8787eeca018bea05523b8ce557cbe73d1ba837`  
		Last Modified: Sat, 01 Feb 2020 17:12:10 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756318e18e359d0294aa1f79cfbd44acdc69fcba8f4624c0e2187d36233eca35`  
		Last Modified: Sat, 01 Feb 2020 17:12:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53cb7b2c3eb3aee379cf77ce9e609facd9d68cbb3d6ceaac79662bb5f3b0c1c`  
		Last Modified: Sat, 01 Feb 2020 17:12:10 GMT  
		Size: 20.5 KB (20527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:2.1.21` - linux; 386

```console
$ docker pull cassandra@sha256:738ad2b44c2ae0df9e639db76c76fd083d1cf6bcdfaef81770f03117f6fa01ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205892219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff8edf2e9f21c28d295036bdf55d045512b306e63344f7d0412828a151653ca4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:03:52 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:04:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:04:00 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:04:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:04:14 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:04:17 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:04:18 GMT
ENV CASSANDRA_VERSION=2.1.21
# Sat, 01 Feb 2020 17:05:19 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 21x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:05:20 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:05:21 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:05:21 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:05:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:05:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:05:23 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:05:23 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:05:23 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:05:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a9c50f749f1de3e365a46e963ec107afea92a353f9b87924b80f24b8e5edf8`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47acd99e08270efe2d386b5d15f509551ba51568a2a87ece42a79e655b1d4ff`  
		Last Modified: Sat, 01 Feb 2020 17:08:29 GMT  
		Size: 6.1 MB (6116093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e2c316cf5968ae3b65e7ac5fb815bf6d859a858c2f545026de5e5b30147721`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 937.8 KB (937830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576efa6035e57b03efee8e68ab486fe466a966565b1bdd538fe532830e437112`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 18.2 KB (18222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c778e4b2ff1c38d05de6ad5183dd807f6854b71acec36f619dc39664d7d6fab`  
		Last Modified: Sat, 01 Feb 2020 17:09:03 GMT  
		Size: 175.6 MB (175639705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198860589e449d920a3eb83741fe991a36be79458eca60e691214d3a3df297a6`  
		Last Modified: Sat, 01 Feb 2020 17:08:26 GMT  
		Size: 4.7 KB (4670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ab5103c37dfc3caa68015cd57ac4ca82ce44f54a524af1c8345bf9051fd1af`  
		Last Modified: Sat, 01 Feb 2020 17:08:26 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502f26a557eed8b4ac7e53ec9b13e205001c0c30fc93c5df8aaf20b4b8318e60`  
		Last Modified: Sat, 01 Feb 2020 17:08:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2076b1f7acfd2e41ab2929177a77ba1e6785b5cd1af9b56912d8f8dbaf69d3`  
		Last Modified: Sat, 01 Feb 2020 17:08:26 GMT  
		Size: 20.5 KB (20525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:2.2`

```console
$ docker pull cassandra@sha256:9070ccbe0f1e3cfb34c9406be2c5175a3f7c5885d1c9933bf226d2894deeff4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386

### `cassandra:2.2` - linux; amd64

```console
$ docker pull cassandra@sha256:0f66081a4e9c465a75ac1c62ffa73edd1cfdaae3440e8a2c8a40e9ec14abc634
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.6 MB (206645392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60547d363254b9a6384ffd567bc65333454aa37d2c652d4380add482c5597cd5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:54:12 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 21:54:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:54:19 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 21:54:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 21:54:32 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 21:54:35 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:55:41 GMT
ENV CASSANDRA_VERSION=2.2.15
# Sat, 01 Feb 2020 21:56:34 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 22x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 21:56:35 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 21:56:35 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 21:56:36 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:56:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 21:56:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:56:37 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 21:56:37 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 21:56:38 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 21:56:38 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7ac5c73a597eb88fd35e6275d72940af5c50458bce1f6ade4d131bd6d0781`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6875e232a43f309c68c25d014efc237ca60c1c5c53bb84e412fceaef1337fc9`  
		Last Modified: Sat, 01 Feb 2020 21:58:41 GMT  
		Size: 5.7 MB (5726879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89165ecf4572ded1baabf4b30188ce50f8f3d83b0ecf031e3e4fd72d488e5cb`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 958.3 KB (958278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ed6a15b620218b60330958b5c4304a9791a9a9bcb843379e41a1d7a9b7b6c`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 18.2 KB (18221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4539ff8905df073aeb921e12822f86dcc68aa201948c6f373afb690c96913ed`  
		Last Modified: Sat, 01 Feb 2020 21:59:46 GMT  
		Size: 177.4 MB (177386880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb87c5da440922b95e4dc163f59870c31bf9d5001b4f801748444938fd03d13`  
		Last Modified: Sat, 01 Feb 2020 21:59:16 GMT  
		Size: 4.9 KB (4889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b2767d4f7fe40fab7be6cb17e463ae3953747dd162ee7afae7d7c3e4f17aba`  
		Last Modified: Sat, 01 Feb 2020 21:59:17 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04db1b4299720eebdc452eaf6b58cca85213db51c44eb71da17a717bff15db7c`  
		Last Modified: Sat, 01 Feb 2020 21:59:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d71f9162e7910e3d11e39d14c34844c1a5684612172951c12a0f78591948f1`  
		Last Modified: Sat, 01 Feb 2020 21:59:16 GMT  
		Size: 22.5 KB (22504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:2.2` - linux; 386

```console
$ docker pull cassandra@sha256:6549a6ab21da5c260cfeb66a99dfce5efe965609d79cb6f896024c342f027730
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210257672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17a065023984308158dd4d645f556df8ae234a4d9caf9a17ca840c853aee8b50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:03:52 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:04:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:04:00 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:04:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:04:14 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:04:17 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:05:36 GMT
ENV CASSANDRA_VERSION=2.2.15
# Sat, 01 Feb 2020 17:06:38 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 22x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:06:39 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:06:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:06:40 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:06:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:06:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:06:41 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:06:42 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:06:42 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:06:42 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a9c50f749f1de3e365a46e963ec107afea92a353f9b87924b80f24b8e5edf8`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47acd99e08270efe2d386b5d15f509551ba51568a2a87ece42a79e655b1d4ff`  
		Last Modified: Sat, 01 Feb 2020 17:08:29 GMT  
		Size: 6.1 MB (6116093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e2c316cf5968ae3b65e7ac5fb815bf6d859a858c2f545026de5e5b30147721`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 937.8 KB (937830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576efa6035e57b03efee8e68ab486fe466a966565b1bdd538fe532830e437112`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 18.2 KB (18222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066e5cb19e22bb995a394515523f75116f8318ca86aa19a0e422498de896963a`  
		Last Modified: Sat, 01 Feb 2020 17:09:46 GMT  
		Size: 180.0 MB (180002961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dacc7bbd69290735cd9caa8d2dd7896ead6c1d0f862d90682a916964d2f25520`  
		Last Modified: Sat, 01 Feb 2020 17:09:08 GMT  
		Size: 4.9 KB (4887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a070f00393afb15c0a033822dec2bdeed6653f1a8fa518546ad35f30529f0965`  
		Last Modified: Sat, 01 Feb 2020 17:09:08 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf59a36f3a591f08cb1487d4ae780af9af7f0d8719be3acdad0b1ec03db689dc`  
		Last Modified: Sat, 01 Feb 2020 17:09:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46469a5665f4eb0c5d82f00652604498061072a51bacf3f0dadcb78d75f785f1`  
		Last Modified: Sat, 01 Feb 2020 17:09:08 GMT  
		Size: 22.5 KB (22504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:2.2.16`

**does not exist** (yet?)

## `cassandra:3`

```console
$ docker pull cassandra@sha256:98531a31f213e62df138441ba074e7394372b244d3c2f99a120cdf80ef431d14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cassandra:3` - linux; amd64

```console
$ docker pull cassandra@sha256:215efca073d7e621500cd1b874a51ff97d45054afe8b9a43542512d39a3f04d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132875655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b571e0906e1b1dd106beed4045191a0f01a03d8e9f3ee43bad6c4d6b3cb73c29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:54:12 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 21:54:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:54:19 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 21:54:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 21:54:32 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 21:54:35 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:57:22 GMT
ENV CASSANDRA_VERSION=3.11.5
# Sat, 01 Feb 2020 21:58:05 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 311x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 21:58:06 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 21:58:08 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 21:58:08 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:58:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 21:58:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:58:11 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 21:58:12 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 21:58:12 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 21:58:13 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7ac5c73a597eb88fd35e6275d72940af5c50458bce1f6ade4d131bd6d0781`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6875e232a43f309c68c25d014efc237ca60c1c5c53bb84e412fceaef1337fc9`  
		Last Modified: Sat, 01 Feb 2020 21:58:41 GMT  
		Size: 5.7 MB (5726879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89165ecf4572ded1baabf4b30188ce50f8f3d83b0ecf031e3e4fd72d488e5cb`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 958.3 KB (958278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ed6a15b620218b60330958b5c4304a9791a9a9bcb843379e41a1d7a9b7b6c`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 18.2 KB (18221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731cf201b9413b2735fddf88fa9c6b594ef8d73c07fdf5418cc70f506ac3b310`  
		Last Modified: Sat, 01 Feb 2020 22:00:30 GMT  
		Size: 103.6 MB (103609077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b87af3649c326245fb70b808c5bd228d7a6ca7c23520bcadaaaf6c43b3869e3`  
		Last Modified: Sat, 01 Feb 2020 22:00:09 GMT  
		Size: 4.7 KB (4656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3c5e9be55fca67486482797d1fe7401c3c167f0b3e987e1c856372e1912805`  
		Last Modified: Sat, 01 Feb 2020 22:00:09 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a5f6b75d1972396465aca6aa6cd4aa1ea24a649d8251b1875ad7f324eba55b`  
		Last Modified: Sat, 01 Feb 2020 22:00:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9db1dfbf451f326f952b5ff0d791cd1e2e867c413d26e6bf459072d6fbc32c`  
		Last Modified: Sat, 01 Feb 2020 22:00:09 GMT  
		Size: 30.8 KB (30806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:ffba9338fc84b09b9db28dd4359db35f8cfd816d59d750eb31730b74e6b7fd7c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122370780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c974d34bfd76d0c32829a0cfe84a7db5ce39b71485c711598a389ee924e6d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:06:04 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:06:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:06:22 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:06:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:06:43 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:06:47 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:10:34 GMT
ENV CASSANDRA_VERSION=3.11.5
# Sat, 01 Feb 2020 17:11:41 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 311x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:11:43 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:11:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:11:45 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:11:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:11:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:11:48 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:11:49 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:11:50 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:11:50 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4555b7d02f2b0f6f8707b27582a305595a30467d8a5836d3099338c98f6dd67f`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4acbf62aed5c4291ff2f7304a5018223f160108cd228d6504407918a4f93eb`  
		Last Modified: Sat, 01 Feb 2020 17:12:13 GMT  
		Size: 5.2 MB (5195126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5c66014f05b2b864abadcb1fbd495e4fc5d72da4a85a3e0f5f890803213218`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 925.7 KB (925700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dba4804d65cfda5823ed59febf14cb99f9ebd1eacc23e11f354e13c04bb3f5c`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 18.2 KB (18219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902c42467f4cac0febff5612beb77be72be4e23d04bd6c2397e2af414f36caa9`  
		Last Modified: Sat, 01 Feb 2020 17:13:42 GMT  
		Size: 95.8 MB (95807384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8028dc8cd5fff0fadf733d14bfbc26014043ab1641312770a951c8d51db4374f`  
		Last Modified: Sat, 01 Feb 2020 17:13:20 GMT  
		Size: 4.7 KB (4657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d51e9c9822364aab68ccbd0ddd5efa6f5caade53286627f19e7fa4fe09984e`  
		Last Modified: Sat, 01 Feb 2020 17:13:20 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26254284266697c14994d7f04a52c3afd2d8254e8960e6f35c9964ea7409dbb7`  
		Last Modified: Sat, 01 Feb 2020 17:13:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c039d24984d26ccaf29dac22ef382283371c44c2fb239a1cbc7d82a7cace7`  
		Last Modified: Sat, 01 Feb 2020 17:13:20 GMT  
		Size: 30.8 KB (30805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3` - linux; 386

```console
$ docker pull cassandra@sha256:b088655d149fdced41f60c11bc3c94a94255074cf749d087741c31bda8d34b49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132939339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a2e01fe42b0fd832311ddd3ce2b596a32530eee2787700fccdf58da3cd28cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:03:52 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:04:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:04:00 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:04:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:04:14 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:04:17 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:07:36 GMT
ENV CASSANDRA_VERSION=3.11.5
# Sat, 01 Feb 2020 17:08:08 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 311x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:08:09 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:08:09 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:08:09 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:08:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:08:11 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:08:11 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:08:12 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:08:12 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a9c50f749f1de3e365a46e963ec107afea92a353f9b87924b80f24b8e5edf8`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47acd99e08270efe2d386b5d15f509551ba51568a2a87ece42a79e655b1d4ff`  
		Last Modified: Sat, 01 Feb 2020 17:08:29 GMT  
		Size: 6.1 MB (6116093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e2c316cf5968ae3b65e7ac5fb815bf6d859a858c2f545026de5e5b30147721`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 937.8 KB (937830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576efa6035e57b03efee8e68ab486fe466a966565b1bdd538fe532830e437112`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 18.2 KB (18222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b6a385acbf9c7b4bf002808e9db2cfbea1c8d10beb8bd7d3d6faea4b65ec3d`  
		Last Modified: Sat, 01 Feb 2020 17:10:33 GMT  
		Size: 102.7 MB (102676565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0ceae0975f0bc0776f57e95df4db288797cd062441cf8f0b6d7eb863eca63a`  
		Last Modified: Sat, 01 Feb 2020 17:10:14 GMT  
		Size: 4.7 KB (4653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4139c6aab82b85d7a1c671a1749f04aed3908150a3a4e00b55652f43a6ad1f7b`  
		Last Modified: Sat, 01 Feb 2020 17:10:13 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8f3fe043f3b2cb9ab4612bfceae32f672dc803176ff6c2c303673dd7d30de0`  
		Last Modified: Sat, 01 Feb 2020 17:10:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e556f0438aa2477f913b29359dfc3311ddf6a89029a90403d435d2ffade22d`  
		Last Modified: Sat, 01 Feb 2020 17:10:14 GMT  
		Size: 30.8 KB (30802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3` - linux; ppc64le

```console
$ docker pull cassandra@sha256:b46d128639d73ed9550db8153c404f6fa496ad90c64b80ab9948ceff6f3eaab5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125891750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a1a9a1d2fcf21431804a4d58f7e5912b24019fdce561408769e3423df52cc25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:8840e8b11ab671d52cc308dfcd68117cbff88d7e5e18e0628683d75699a7c131 in / 
# Sat, 01 Feb 2020 17:20:49 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:36:46 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 19:37:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:37:36 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 19:38:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 19:38:33 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 19:38:48 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 19:43:10 GMT
ENV CASSANDRA_VERSION=3.11.5
# Sat, 01 Feb 2020 19:45:57 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 311x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 19:46:05 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 19:46:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 19:46:18 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 19:46:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 19:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 19:46:39 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 19:46:43 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 19:46:48 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 19:46:52 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:4b12198d119cc40a2102fa8f986f1f3bc6f22967a421939f96b52470129050b9`  
		Last Modified: Sat, 01 Feb 2020 17:31:15 GMT  
		Size: 22.8 MB (22800759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf92a8b07f08de99975697e965970e019460963251517a56584e5871784af96c`  
		Last Modified: Sat, 01 Feb 2020 19:47:15 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b0287928e15d05f504151a7671f55b4e8132919c52f67a136cbc75d21b388`  
		Last Modified: Sat, 01 Feb 2020 19:47:16 GMT  
		Size: 5.6 MB (5594681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db99c7d2b25291eadb7c7175ae2b270c14b747b63f46e898b43a9a8c8aac88c`  
		Last Modified: Sat, 01 Feb 2020 19:47:16 GMT  
		Size: 926.9 KB (926911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf485f8f959fa3e0e5655c2a064eec4f546a86f4ec5af1da4f3897fb175f0da`  
		Last Modified: Sat, 01 Feb 2020 19:47:14 GMT  
		Size: 18.2 KB (18219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8136e69a60b569a523a3e735ba7f919918fb2b3e66e0a26eee6532204d7c0b1`  
		Last Modified: Sat, 01 Feb 2020 19:47:57 GMT  
		Size: 96.5 MB (96508924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea22564e9e0427b8ba0920d6f39070bd2be15557f04036d97e5ae5ae728d6176`  
		Last Modified: Sat, 01 Feb 2020 19:47:38 GMT  
		Size: 8.4 KB (8418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096d1486853874d6cb73464666bf49cc489898becb0de09c02372e57a8802700`  
		Last Modified: Sat, 01 Feb 2020 19:47:39 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2994292121733d9f12e1c52dd6e1389b4b0b01eed552700173b3c30cf0b63124`  
		Last Modified: Sat, 01 Feb 2020 19:47:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec2cfddbca54923722035d4419fd9b74697637555f00a3e30cd75eb028eabc`  
		Last Modified: Sat, 01 Feb 2020 19:47:39 GMT  
		Size: 30.8 KB (30810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:3.0`

```console
$ docker pull cassandra@sha256:9fb3c04a91e1871ff9b8ab95fc595f38c35144cbcf24d0e50ecc41e36146947c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cassandra:3.0` - linux; amd64

```console
$ docker pull cassandra@sha256:b01e4bda39cbceb76f00f878bd36cb3b12811ddf98ce012eadc506ca735e59d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128053033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6593163290a2d6a984ed9b95f1ff840a925b1472a848eb3755212489f5bd187`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:54:12 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 21:54:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:54:19 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 21:54:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 21:54:32 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 21:54:35 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:56:44 GMT
ENV CASSANDRA_VERSION=3.0.19
# Sat, 01 Feb 2020 21:57:14 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 30x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 21:57:14 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 21:57:15 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 21:57:15 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:57:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 21:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:57:17 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 21:57:17 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 21:57:17 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 21:57:18 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7ac5c73a597eb88fd35e6275d72940af5c50458bce1f6ade4d131bd6d0781`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6875e232a43f309c68c25d014efc237ca60c1c5c53bb84e412fceaef1337fc9`  
		Last Modified: Sat, 01 Feb 2020 21:58:41 GMT  
		Size: 5.7 MB (5726879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89165ecf4572ded1baabf4b30188ce50f8f3d83b0ecf031e3e4fd72d488e5cb`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 958.3 KB (958278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ed6a15b620218b60330958b5c4304a9791a9a9bcb843379e41a1d7a9b7b6c`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 18.2 KB (18221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cdc2b9791b6383a99da7d30f5e540e907cfbf9f5d2477722ac3a9491d04cc8`  
		Last Modified: Sat, 01 Feb 2020 22:00:05 GMT  
		Size: 98.8 MB (98790895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e5b0c29fb7bbc10240a93459d9d536b1fda5919bfc64650ce5e706a7b1a311`  
		Last Modified: Sat, 01 Feb 2020 21:59:51 GMT  
		Size: 5.0 KB (4953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58dc1e0eba3a98b504438665121d2ac61806739ca3b65073d29289efe607a4e`  
		Last Modified: Sat, 01 Feb 2020 21:59:50 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f861bc912ce44ef027e8f1691b53dfc64be08197d8ea40bc9c4bc8dba7a2e24`  
		Last Modified: Sat, 01 Feb 2020 21:59:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1178c78192e3a86b8a0eb30901836530813a13a3812f7c709e28ff1505b3fcce`  
		Last Modified: Sat, 01 Feb 2020 21:59:50 GMT  
		Size: 26.1 KB (26069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.0` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:3a9bed3a932b7794c2acc48f594e475254ce125c83f2e8b57c377ce47daf3f22
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117558716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba346026ac9d2368e9a1cb0d93079614b2e0260ae4dbf09ca2f7670db2070a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:06:04 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:06:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:06:22 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:06:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:06:43 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:06:47 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:09:04 GMT
ENV CASSANDRA_VERSION=3.0.19
# Sat, 01 Feb 2020 17:10:09 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 30x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:10:11 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:10:13 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:10:13 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:10:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:10:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:10:17 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:10:18 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:10:18 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:10:19 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4555b7d02f2b0f6f8707b27582a305595a30467d8a5836d3099338c98f6dd67f`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4acbf62aed5c4291ff2f7304a5018223f160108cd228d6504407918a4f93eb`  
		Last Modified: Sat, 01 Feb 2020 17:12:13 GMT  
		Size: 5.2 MB (5195126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5c66014f05b2b864abadcb1fbd495e4fc5d72da4a85a3e0f5f890803213218`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 925.7 KB (925700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dba4804d65cfda5823ed59febf14cb99f9ebd1eacc23e11f354e13c04bb3f5c`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 18.2 KB (18219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0baaf3c9a6fecda990b730f7dd4a5798043db425587ed9c500710908b2a81efd`  
		Last Modified: Sat, 01 Feb 2020 17:13:14 GMT  
		Size: 91.0 MB (90999758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0400a4dde101ae5c48508e1a6da9a0d2758a77833b2c67980e501addb76f57`  
		Last Modified: Sat, 01 Feb 2020 17:12:53 GMT  
		Size: 5.0 KB (4953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397e0bb107547a67fcc194e4b9a1671faee7f621599fa9a3ccae44e048478177`  
		Last Modified: Sat, 01 Feb 2020 17:12:53 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d6018d4d605f7421b54b6b330874ed9a41a1c59a5e1d10a78017b646e6e68b`  
		Last Modified: Sat, 01 Feb 2020 17:12:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce3a6a24bd0aac3a24f4a19fe8728cb31a7026ea96d70017cba7a6f4dae75cb`  
		Last Modified: Sat, 01 Feb 2020 17:12:53 GMT  
		Size: 26.1 KB (26070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.0` - linux; 386

```console
$ docker pull cassandra@sha256:ef8b8b60e8939ba63dd8f0f28bac2e3c614bf1e0545efc537d2c6e775e0ed368
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128124806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e22531ea8a652b88e293a58e99685d627db7a82703e603f798ef59ea28654d1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:03:52 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:04:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:04:00 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:04:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:04:14 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:04:17 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:06:51 GMT
ENV CASSANDRA_VERSION=3.0.19
# Sat, 01 Feb 2020 17:07:23 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 30x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:07:24 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:07:24 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:07:24 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:07:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:07:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:07:26 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:07:26 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:07:27 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:07:27 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a9c50f749f1de3e365a46e963ec107afea92a353f9b87924b80f24b8e5edf8`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47acd99e08270efe2d386b5d15f509551ba51568a2a87ece42a79e655b1d4ff`  
		Last Modified: Sat, 01 Feb 2020 17:08:29 GMT  
		Size: 6.1 MB (6116093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e2c316cf5968ae3b65e7ac5fb815bf6d859a858c2f545026de5e5b30147721`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 937.8 KB (937830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576efa6035e57b03efee8e68ab486fe466a966565b1bdd538fe532830e437112`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 18.2 KB (18222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0ea9431ceabd6fb96e505e0ded7ca086803e93294d3b6ec4abf0564d696793`  
		Last Modified: Sat, 01 Feb 2020 17:10:10 GMT  
		Size: 97.9 MB (97866466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b772c43163e329e61d06df9238b9f5878e57c8cf073dfbab5c513e9c69e7b5cf`  
		Last Modified: Sat, 01 Feb 2020 17:09:50 GMT  
		Size: 4.9 KB (4949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb764a5017a45b2c479126d7d88da9a9aea1125bd70890daae5b3c557d5595d3`  
		Last Modified: Sat, 01 Feb 2020 17:09:50 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834a8896db6b234be86868816bd2376544b7d72462793ec1be2894b6435dd22d`  
		Last Modified: Sat, 01 Feb 2020 17:09:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d28f543eff438691f31d1a3db478e1f43d4ecaf697d05af1c2a7c9138154bef`  
		Last Modified: Sat, 01 Feb 2020 17:09:50 GMT  
		Size: 26.1 KB (26071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.0` - linux; ppc64le

```console
$ docker pull cassandra@sha256:049147515a0aff9804a24a52d8b26e62f13d622cec6a8d74acc63bd65cf45037
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121081157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ab0294cfc442be7ec666125a7df02cfd725002af4e01788dc2be364467d9b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:8840e8b11ab671d52cc308dfcd68117cbff88d7e5e18e0628683d75699a7c131 in / 
# Sat, 01 Feb 2020 17:20:49 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:36:46 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 19:37:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:37:36 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 19:38:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 19:38:33 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 19:38:48 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 19:38:56 GMT
ENV CASSANDRA_VERSION=3.0.19
# Sat, 01 Feb 2020 19:41:56 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 30x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 19:42:04 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 19:42:13 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 19:42:15 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 19:42:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 19:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 19:42:38 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 19:42:46 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 19:42:50 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 19:42:52 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:4b12198d119cc40a2102fa8f986f1f3bc6f22967a421939f96b52470129050b9`  
		Last Modified: Sat, 01 Feb 2020 17:31:15 GMT  
		Size: 22.8 MB (22800759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf92a8b07f08de99975697e965970e019460963251517a56584e5871784af96c`  
		Last Modified: Sat, 01 Feb 2020 19:47:15 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b0287928e15d05f504151a7671f55b4e8132919c52f67a136cbc75d21b388`  
		Last Modified: Sat, 01 Feb 2020 19:47:16 GMT  
		Size: 5.6 MB (5594681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db99c7d2b25291eadb7c7175ae2b270c14b747b63f46e898b43a9a8c8aac88c`  
		Last Modified: Sat, 01 Feb 2020 19:47:16 GMT  
		Size: 926.9 KB (926911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf485f8f959fa3e0e5655c2a064eec4f546a86f4ec5af1da4f3897fb175f0da`  
		Last Modified: Sat, 01 Feb 2020 19:47:14 GMT  
		Size: 18.2 KB (18219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbb0eecc35d1a0ee63a9b4dd9fc6e719a31aecd4303bb17a541d7ae1e65c7cd`  
		Last Modified: Sat, 01 Feb 2020 19:47:27 GMT  
		Size: 91.7 MB (91706534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e29e3018d28166a102635a4faa15d183dee518ed13a8a066f7ee0c66520851`  
		Last Modified: Sat, 01 Feb 2020 19:47:12 GMT  
		Size: 5.0 KB (4955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a74bace4b5ca5f99d6ba8e80e55be4c8665d6a59bb051b3f5b9cff210ddad9`  
		Last Modified: Sat, 01 Feb 2020 19:47:11 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302abfd0211ff7415e46ba5f2c0ac990d793dd774f304203f36286f9b349acf4`  
		Last Modified: Sat, 01 Feb 2020 19:47:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251ad4fb8bdde257e0aa48776686dbacd5922b60913aecbf07d3644da22b2b20`  
		Last Modified: Sat, 01 Feb 2020 19:47:11 GMT  
		Size: 26.1 KB (26070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:3.0.20`

**does not exist** (yet?)

## `cassandra:3.11`

```console
$ docker pull cassandra@sha256:98531a31f213e62df138441ba074e7394372b244d3c2f99a120cdf80ef431d14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cassandra:3.11` - linux; amd64

```console
$ docker pull cassandra@sha256:215efca073d7e621500cd1b874a51ff97d45054afe8b9a43542512d39a3f04d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132875655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b571e0906e1b1dd106beed4045191a0f01a03d8e9f3ee43bad6c4d6b3cb73c29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:54:12 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 21:54:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:54:19 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 21:54:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 21:54:32 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 21:54:35 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:57:22 GMT
ENV CASSANDRA_VERSION=3.11.5
# Sat, 01 Feb 2020 21:58:05 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 311x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 21:58:06 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 21:58:08 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 21:58:08 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:58:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 21:58:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:58:11 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 21:58:12 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 21:58:12 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 21:58:13 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7ac5c73a597eb88fd35e6275d72940af5c50458bce1f6ade4d131bd6d0781`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6875e232a43f309c68c25d014efc237ca60c1c5c53bb84e412fceaef1337fc9`  
		Last Modified: Sat, 01 Feb 2020 21:58:41 GMT  
		Size: 5.7 MB (5726879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89165ecf4572ded1baabf4b30188ce50f8f3d83b0ecf031e3e4fd72d488e5cb`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 958.3 KB (958278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ed6a15b620218b60330958b5c4304a9791a9a9bcb843379e41a1d7a9b7b6c`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 18.2 KB (18221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731cf201b9413b2735fddf88fa9c6b594ef8d73c07fdf5418cc70f506ac3b310`  
		Last Modified: Sat, 01 Feb 2020 22:00:30 GMT  
		Size: 103.6 MB (103609077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b87af3649c326245fb70b808c5bd228d7a6ca7c23520bcadaaaf6c43b3869e3`  
		Last Modified: Sat, 01 Feb 2020 22:00:09 GMT  
		Size: 4.7 KB (4656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3c5e9be55fca67486482797d1fe7401c3c167f0b3e987e1c856372e1912805`  
		Last Modified: Sat, 01 Feb 2020 22:00:09 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a5f6b75d1972396465aca6aa6cd4aa1ea24a649d8251b1875ad7f324eba55b`  
		Last Modified: Sat, 01 Feb 2020 22:00:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9db1dfbf451f326f952b5ff0d791cd1e2e867c413d26e6bf459072d6fbc32c`  
		Last Modified: Sat, 01 Feb 2020 22:00:09 GMT  
		Size: 30.8 KB (30806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.11` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:ffba9338fc84b09b9db28dd4359db35f8cfd816d59d750eb31730b74e6b7fd7c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122370780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c974d34bfd76d0c32829a0cfe84a7db5ce39b71485c711598a389ee924e6d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:06:04 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:06:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:06:22 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:06:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:06:43 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:06:47 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:10:34 GMT
ENV CASSANDRA_VERSION=3.11.5
# Sat, 01 Feb 2020 17:11:41 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 311x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:11:43 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:11:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:11:45 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:11:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:11:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:11:48 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:11:49 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:11:50 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:11:50 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4555b7d02f2b0f6f8707b27582a305595a30467d8a5836d3099338c98f6dd67f`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4acbf62aed5c4291ff2f7304a5018223f160108cd228d6504407918a4f93eb`  
		Last Modified: Sat, 01 Feb 2020 17:12:13 GMT  
		Size: 5.2 MB (5195126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5c66014f05b2b864abadcb1fbd495e4fc5d72da4a85a3e0f5f890803213218`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 925.7 KB (925700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dba4804d65cfda5823ed59febf14cb99f9ebd1eacc23e11f354e13c04bb3f5c`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 18.2 KB (18219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902c42467f4cac0febff5612beb77be72be4e23d04bd6c2397e2af414f36caa9`  
		Last Modified: Sat, 01 Feb 2020 17:13:42 GMT  
		Size: 95.8 MB (95807384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8028dc8cd5fff0fadf733d14bfbc26014043ab1641312770a951c8d51db4374f`  
		Last Modified: Sat, 01 Feb 2020 17:13:20 GMT  
		Size: 4.7 KB (4657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d51e9c9822364aab68ccbd0ddd5efa6f5caade53286627f19e7fa4fe09984e`  
		Last Modified: Sat, 01 Feb 2020 17:13:20 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26254284266697c14994d7f04a52c3afd2d8254e8960e6f35c9964ea7409dbb7`  
		Last Modified: Sat, 01 Feb 2020 17:13:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c039d24984d26ccaf29dac22ef382283371c44c2fb239a1cbc7d82a7cace7`  
		Last Modified: Sat, 01 Feb 2020 17:13:20 GMT  
		Size: 30.8 KB (30805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.11` - linux; 386

```console
$ docker pull cassandra@sha256:b088655d149fdced41f60c11bc3c94a94255074cf749d087741c31bda8d34b49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132939339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a2e01fe42b0fd832311ddd3ce2b596a32530eee2787700fccdf58da3cd28cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:03:52 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:04:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:04:00 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:04:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:04:14 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:04:17 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:07:36 GMT
ENV CASSANDRA_VERSION=3.11.5
# Sat, 01 Feb 2020 17:08:08 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 311x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:08:09 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:08:09 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:08:09 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:08:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:08:11 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:08:11 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:08:12 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:08:12 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a9c50f749f1de3e365a46e963ec107afea92a353f9b87924b80f24b8e5edf8`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47acd99e08270efe2d386b5d15f509551ba51568a2a87ece42a79e655b1d4ff`  
		Last Modified: Sat, 01 Feb 2020 17:08:29 GMT  
		Size: 6.1 MB (6116093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e2c316cf5968ae3b65e7ac5fb815bf6d859a858c2f545026de5e5b30147721`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 937.8 KB (937830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576efa6035e57b03efee8e68ab486fe466a966565b1bdd538fe532830e437112`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 18.2 KB (18222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b6a385acbf9c7b4bf002808e9db2cfbea1c8d10beb8bd7d3d6faea4b65ec3d`  
		Last Modified: Sat, 01 Feb 2020 17:10:33 GMT  
		Size: 102.7 MB (102676565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0ceae0975f0bc0776f57e95df4db288797cd062441cf8f0b6d7eb863eca63a`  
		Last Modified: Sat, 01 Feb 2020 17:10:14 GMT  
		Size: 4.7 KB (4653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4139c6aab82b85d7a1c671a1749f04aed3908150a3a4e00b55652f43a6ad1f7b`  
		Last Modified: Sat, 01 Feb 2020 17:10:13 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8f3fe043f3b2cb9ab4612bfceae32f672dc803176ff6c2c303673dd7d30de0`  
		Last Modified: Sat, 01 Feb 2020 17:10:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e556f0438aa2477f913b29359dfc3311ddf6a89029a90403d435d2ffade22d`  
		Last Modified: Sat, 01 Feb 2020 17:10:14 GMT  
		Size: 30.8 KB (30802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.11` - linux; ppc64le

```console
$ docker pull cassandra@sha256:b46d128639d73ed9550db8153c404f6fa496ad90c64b80ab9948ceff6f3eaab5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125891750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a1a9a1d2fcf21431804a4d58f7e5912b24019fdce561408769e3423df52cc25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:8840e8b11ab671d52cc308dfcd68117cbff88d7e5e18e0628683d75699a7c131 in / 
# Sat, 01 Feb 2020 17:20:49 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:36:46 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 19:37:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:37:36 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 19:38:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 19:38:33 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 19:38:48 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 19:43:10 GMT
ENV CASSANDRA_VERSION=3.11.5
# Sat, 01 Feb 2020 19:45:57 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 311x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 19:46:05 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 19:46:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 19:46:18 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 19:46:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 19:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 19:46:39 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 19:46:43 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 19:46:48 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 19:46:52 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:4b12198d119cc40a2102fa8f986f1f3bc6f22967a421939f96b52470129050b9`  
		Last Modified: Sat, 01 Feb 2020 17:31:15 GMT  
		Size: 22.8 MB (22800759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf92a8b07f08de99975697e965970e019460963251517a56584e5871784af96c`  
		Last Modified: Sat, 01 Feb 2020 19:47:15 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b0287928e15d05f504151a7671f55b4e8132919c52f67a136cbc75d21b388`  
		Last Modified: Sat, 01 Feb 2020 19:47:16 GMT  
		Size: 5.6 MB (5594681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db99c7d2b25291eadb7c7175ae2b270c14b747b63f46e898b43a9a8c8aac88c`  
		Last Modified: Sat, 01 Feb 2020 19:47:16 GMT  
		Size: 926.9 KB (926911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf485f8f959fa3e0e5655c2a064eec4f546a86f4ec5af1da4f3897fb175f0da`  
		Last Modified: Sat, 01 Feb 2020 19:47:14 GMT  
		Size: 18.2 KB (18219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8136e69a60b569a523a3e735ba7f919918fb2b3e66e0a26eee6532204d7c0b1`  
		Last Modified: Sat, 01 Feb 2020 19:47:57 GMT  
		Size: 96.5 MB (96508924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea22564e9e0427b8ba0920d6f39070bd2be15557f04036d97e5ae5ae728d6176`  
		Last Modified: Sat, 01 Feb 2020 19:47:38 GMT  
		Size: 8.4 KB (8418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096d1486853874d6cb73464666bf49cc489898becb0de09c02372e57a8802700`  
		Last Modified: Sat, 01 Feb 2020 19:47:39 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2994292121733d9f12e1c52dd6e1389b4b0b01eed552700173b3c30cf0b63124`  
		Last Modified: Sat, 01 Feb 2020 19:47:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec2cfddbca54923722035d4419fd9b74697637555f00a3e30cd75eb028eabc`  
		Last Modified: Sat, 01 Feb 2020 19:47:39 GMT  
		Size: 30.8 KB (30810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:3.11.6`

**does not exist** (yet?)

## `cassandra:latest`

```console
$ docker pull cassandra@sha256:98531a31f213e62df138441ba074e7394372b244d3c2f99a120cdf80ef431d14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cassandra:latest` - linux; amd64

```console
$ docker pull cassandra@sha256:215efca073d7e621500cd1b874a51ff97d45054afe8b9a43542512d39a3f04d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132875655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b571e0906e1b1dd106beed4045191a0f01a03d8e9f3ee43bad6c4d6b3cb73c29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:54:12 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 21:54:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:54:19 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 21:54:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 21:54:32 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 21:54:35 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:57:22 GMT
ENV CASSANDRA_VERSION=3.11.5
# Sat, 01 Feb 2020 21:58:05 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 311x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 21:58:06 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 21:58:08 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 21:58:08 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:58:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 21:58:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:58:11 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 21:58:12 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 21:58:12 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 21:58:13 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7ac5c73a597eb88fd35e6275d72940af5c50458bce1f6ade4d131bd6d0781`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6875e232a43f309c68c25d014efc237ca60c1c5c53bb84e412fceaef1337fc9`  
		Last Modified: Sat, 01 Feb 2020 21:58:41 GMT  
		Size: 5.7 MB (5726879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89165ecf4572ded1baabf4b30188ce50f8f3d83b0ecf031e3e4fd72d488e5cb`  
		Last Modified: Sat, 01 Feb 2020 21:58:39 GMT  
		Size: 958.3 KB (958278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ed6a15b620218b60330958b5c4304a9791a9a9bcb843379e41a1d7a9b7b6c`  
		Last Modified: Sat, 01 Feb 2020 21:58:38 GMT  
		Size: 18.2 KB (18221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731cf201b9413b2735fddf88fa9c6b594ef8d73c07fdf5418cc70f506ac3b310`  
		Last Modified: Sat, 01 Feb 2020 22:00:30 GMT  
		Size: 103.6 MB (103609077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b87af3649c326245fb70b808c5bd228d7a6ca7c23520bcadaaaf6c43b3869e3`  
		Last Modified: Sat, 01 Feb 2020 22:00:09 GMT  
		Size: 4.7 KB (4656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3c5e9be55fca67486482797d1fe7401c3c167f0b3e987e1c856372e1912805`  
		Last Modified: Sat, 01 Feb 2020 22:00:09 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a5f6b75d1972396465aca6aa6cd4aa1ea24a649d8251b1875ad7f324eba55b`  
		Last Modified: Sat, 01 Feb 2020 22:00:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9db1dfbf451f326f952b5ff0d791cd1e2e867c413d26e6bf459072d6fbc32c`  
		Last Modified: Sat, 01 Feb 2020 22:00:09 GMT  
		Size: 30.8 KB (30806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:latest` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:ffba9338fc84b09b9db28dd4359db35f8cfd816d59d750eb31730b74e6b7fd7c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122370780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c974d34bfd76d0c32829a0cfe84a7db5ce39b71485c711598a389ee924e6d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:06:04 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:06:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:06:22 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:06:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:06:43 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:06:47 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:10:34 GMT
ENV CASSANDRA_VERSION=3.11.5
# Sat, 01 Feb 2020 17:11:41 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 311x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:11:43 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:11:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:11:45 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:11:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:11:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:11:48 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:11:49 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:11:50 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:11:50 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4555b7d02f2b0f6f8707b27582a305595a30467d8a5836d3099338c98f6dd67f`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4acbf62aed5c4291ff2f7304a5018223f160108cd228d6504407918a4f93eb`  
		Last Modified: Sat, 01 Feb 2020 17:12:13 GMT  
		Size: 5.2 MB (5195126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5c66014f05b2b864abadcb1fbd495e4fc5d72da4a85a3e0f5f890803213218`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 925.7 KB (925700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dba4804d65cfda5823ed59febf14cb99f9ebd1eacc23e11f354e13c04bb3f5c`  
		Last Modified: Sat, 01 Feb 2020 17:12:12 GMT  
		Size: 18.2 KB (18219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902c42467f4cac0febff5612beb77be72be4e23d04bd6c2397e2af414f36caa9`  
		Last Modified: Sat, 01 Feb 2020 17:13:42 GMT  
		Size: 95.8 MB (95807384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8028dc8cd5fff0fadf733d14bfbc26014043ab1641312770a951c8d51db4374f`  
		Last Modified: Sat, 01 Feb 2020 17:13:20 GMT  
		Size: 4.7 KB (4657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d51e9c9822364aab68ccbd0ddd5efa6f5caade53286627f19e7fa4fe09984e`  
		Last Modified: Sat, 01 Feb 2020 17:13:20 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26254284266697c14994d7f04a52c3afd2d8254e8960e6f35c9964ea7409dbb7`  
		Last Modified: Sat, 01 Feb 2020 17:13:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c039d24984d26ccaf29dac22ef382283371c44c2fb239a1cbc7d82a7cace7`  
		Last Modified: Sat, 01 Feb 2020 17:13:20 GMT  
		Size: 30.8 KB (30805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:latest` - linux; 386

```console
$ docker pull cassandra@sha256:b088655d149fdced41f60c11bc3c94a94255074cf749d087741c31bda8d34b49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132939339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a2e01fe42b0fd832311ddd3ce2b596a32530eee2787700fccdf58da3cd28cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:03:52 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 17:04:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:04:00 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 17:04:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 17:04:14 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 17:04:17 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 17:07:36 GMT
ENV CASSANDRA_VERSION=3.11.5
# Sat, 01 Feb 2020 17:08:08 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 311x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 17:08:09 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 17:08:09 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 17:08:09 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 17:08:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 17:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 17:08:11 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 17:08:11 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 17:08:12 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 17:08:12 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a9c50f749f1de3e365a46e963ec107afea92a353f9b87924b80f24b8e5edf8`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47acd99e08270efe2d386b5d15f509551ba51568a2a87ece42a79e655b1d4ff`  
		Last Modified: Sat, 01 Feb 2020 17:08:29 GMT  
		Size: 6.1 MB (6116093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e2c316cf5968ae3b65e7ac5fb815bf6d859a858c2f545026de5e5b30147721`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 937.8 KB (937830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576efa6035e57b03efee8e68ab486fe466a966565b1bdd538fe532830e437112`  
		Last Modified: Sat, 01 Feb 2020 17:08:27 GMT  
		Size: 18.2 KB (18222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b6a385acbf9c7b4bf002808e9db2cfbea1c8d10beb8bd7d3d6faea4b65ec3d`  
		Last Modified: Sat, 01 Feb 2020 17:10:33 GMT  
		Size: 102.7 MB (102676565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0ceae0975f0bc0776f57e95df4db288797cd062441cf8f0b6d7eb863eca63a`  
		Last Modified: Sat, 01 Feb 2020 17:10:14 GMT  
		Size: 4.7 KB (4653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4139c6aab82b85d7a1c671a1749f04aed3908150a3a4e00b55652f43a6ad1f7b`  
		Last Modified: Sat, 01 Feb 2020 17:10:13 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8f3fe043f3b2cb9ab4612bfceae32f672dc803176ff6c2c303673dd7d30de0`  
		Last Modified: Sat, 01 Feb 2020 17:10:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e556f0438aa2477f913b29359dfc3311ddf6a89029a90403d435d2ffade22d`  
		Last Modified: Sat, 01 Feb 2020 17:10:14 GMT  
		Size: 30.8 KB (30802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:latest` - linux; ppc64le

```console
$ docker pull cassandra@sha256:b46d128639d73ed9550db8153c404f6fa496ad90c64b80ab9948ceff6f3eaab5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125891750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a1a9a1d2fcf21431804a4d58f7e5912b24019fdce561408769e3423df52cc25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:8840e8b11ab671d52cc308dfcd68117cbff88d7e5e18e0628683d75699a7c131 in / 
# Sat, 01 Feb 2020 17:20:49 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:36:46 GMT
RUN groupadd -r cassandra --gid=999 && useradd -r -g cassandra --uid=999 cassandra
# Sat, 01 Feb 2020 19:37:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		libjemalloc1 		procps 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:37:36 GMT
ENV GOSU_VERSION=1.10
# Sat, 01 Feb 2020 19:38:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	gosu nobody true
# Sat, 01 Feb 2020 19:38:33 GMT
ENV GPG_KEYS=514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA
# Sat, 01 Feb 2020 19:38:48 GMT
RUN set -eux; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/cassandra.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 19:43:10 GMT
ENV CASSANDRA_VERSION=3.11.5
# Sat, 01 Feb 2020 19:45:57 GMT
RUN set -eux; 		mkdir -p /usr/share/man/man1/; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386) 			echo 'deb http://www.apache.org/dist/cassandra/debian 311x main' > /etc/apt/sources.list.d/cassandra.list; 			apt-get update; 			;; 		*) 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get install -y --no-install-recommends 				wget ca-certificates 				dpkg-dev 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						tempDir="$(mktemp -d)"; 			for pkg in cassandra cassandra-tools; do 				deb="${pkg}_${CASSANDRA_VERSION}_all.deb"; 				wget -O "$tempDir/$deb" "https://www.apache.org/dist/cassandra/debian/pool/main/c/cassandra/$deb"; 			done; 						ls -lAFh "$tempDir"; 			( cd "$tempDir" && dpkg-scanpackages . > Packages ); 			grep '^Package: ' "$tempDir/Packages"; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y 		cassandra="$CASSANDRA_VERSION" 		cassandra-tools="$CASSANDRA_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "${tempDir:-}" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Sat, 01 Feb 2020 19:46:05 GMT
ENV CASSANDRA_CONFIG=/etc/cassandra
# Sat, 01 Feb 2020 19:46:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONFIG/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONFIG/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONFIG/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONFIG/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONFIG/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONFIG/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONFIG/cassandra-env.sh"; 			fi; 			;; 	esac; 		sed -ri 's/^(JVM_PATCH_VERSION)=.*/\1=25/' "$CASSANDRA_CONFIG/cassandra-env.sh"
# Sat, 01 Feb 2020 19:46:18 GMT
COPY file:32df6d10eaefa72af8b8f14546dffbafa553b673990a6dbbe9870c1909627db8 in /usr/local/bin/ 
# Sat, 01 Feb 2020 19:46:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 01 Feb 2020 19:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 19:46:39 GMT
RUN mkdir -p /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chown -R cassandra:cassandra /var/lib/cassandra "$CASSANDRA_CONFIG" 	&& chmod 777 /var/lib/cassandra "$CASSANDRA_CONFIG"
# Sat, 01 Feb 2020 19:46:43 GMT
VOLUME [/var/lib/cassandra]
# Sat, 01 Feb 2020 19:46:48 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 01 Feb 2020 19:46:52 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:4b12198d119cc40a2102fa8f986f1f3bc6f22967a421939f96b52470129050b9`  
		Last Modified: Sat, 01 Feb 2020 17:31:15 GMT  
		Size: 22.8 MB (22800759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf92a8b07f08de99975697e965970e019460963251517a56584e5871784af96c`  
		Last Modified: Sat, 01 Feb 2020 19:47:15 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b0287928e15d05f504151a7671f55b4e8132919c52f67a136cbc75d21b388`  
		Last Modified: Sat, 01 Feb 2020 19:47:16 GMT  
		Size: 5.6 MB (5594681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db99c7d2b25291eadb7c7175ae2b270c14b747b63f46e898b43a9a8c8aac88c`  
		Last Modified: Sat, 01 Feb 2020 19:47:16 GMT  
		Size: 926.9 KB (926911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf485f8f959fa3e0e5655c2a064eec4f546a86f4ec5af1da4f3897fb175f0da`  
		Last Modified: Sat, 01 Feb 2020 19:47:14 GMT  
		Size: 18.2 KB (18219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8136e69a60b569a523a3e735ba7f919918fb2b3e66e0a26eee6532204d7c0b1`  
		Last Modified: Sat, 01 Feb 2020 19:47:57 GMT  
		Size: 96.5 MB (96508924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea22564e9e0427b8ba0920d6f39070bd2be15557f04036d97e5ae5ae728d6176`  
		Last Modified: Sat, 01 Feb 2020 19:47:38 GMT  
		Size: 8.4 KB (8418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096d1486853874d6cb73464666bf49cc489898becb0de09c02372e57a8802700`  
		Last Modified: Sat, 01 Feb 2020 19:47:39 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2994292121733d9f12e1c52dd6e1389b4b0b01eed552700173b3c30cf0b63124`  
		Last Modified: Sat, 01 Feb 2020 19:47:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec2cfddbca54923722035d4419fd9b74697637555f00a3e30cd75eb028eabc`  
		Last Modified: Sat, 01 Feb 2020 19:47:39 GMT  
		Size: 30.8 KB (30810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
