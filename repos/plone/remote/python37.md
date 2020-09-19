## `plone:python37`

```console
$ docker pull plone@sha256:a78ad5998ca84c71408a974f62c102d90f133c07d030f00613511ca72e4793eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `plone:python37` - linux; amd64

```console
$ docker pull plone@sha256:1f42e3668764ba573e8b3ea2f4cb3705a835cd3f21056d994f236afd879c3d39
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.2 MB (191160606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85aea4f7802275e7bd72bf20b9ec366a879b3fa64d1e25d80ba23b88b961267`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 16:28:20 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 16:28:20 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 16:28:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 17:11:30 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 17:11:31 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 17:23:32 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 17:23:32 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 17:23:33 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 17:23:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 17:23:33 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 17:23:49 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 17:23:49 GMT
CMD ["python3"]
# Sat, 19 Sep 2020 00:32:29 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Sat, 19 Sep 2020 00:32:30 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Sat, 19 Sep 2020 00:32:30 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Sat, 19 Sep 2020 00:32:31 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 00:35:37 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 00:35:38 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 00:35:39 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Sat, 19 Sep 2020 00:35:39 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 00:35:39 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 00:35:39 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 00:35:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 00:35:40 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:d121f8d1c4128ebc1e95e5bfad90a0189b84eadbbb2fbaad20cbb26d20b2c8a2`  
		Last Modified: Thu, 10 Sep 2020 00:34:02 GMT  
		Size: 27.1 MB (27092161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca572574cc82ba635292c0aba70b719de39faffe7a40a802bb0f8c22663b51ac`  
		Last Modified: Thu, 10 Sep 2020 18:56:57 GMT  
		Size: 2.7 MB (2749988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bec6349c99d9ce28745c68ca3b7739db00f66cbacb488b9dfd6c548fb5058c1`  
		Last Modified: Thu, 10 Sep 2020 18:57:53 GMT  
		Size: 10.1 MB (10062557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087ac0b72728719a9249ebec6f2970597890a512fe16a8168e33aa3eac8090f7`  
		Last Modified: Thu, 10 Sep 2020 18:57:50 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca52d7c92b3065641ebfed14427f514fe20b9dcef29a3b586b5b0ff98e7cb0d`  
		Last Modified: Thu, 10 Sep 2020 18:57:51 GMT  
		Size: 2.4 MB (2408145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438bf6fb05c17d0b2181d479c631cb0bae0c958ace7bc65a0c5ec7003af06066`  
		Last Modified: Sat, 19 Sep 2020 00:49:54 GMT  
		Size: 3.9 KB (3900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fb4a5cdc82584e2ecf8d32c980ffdb1b35a317aa8a0a92b0f6b2f54f839d4d`  
		Last Modified: Sat, 19 Sep 2020 00:49:55 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6348b4b6e79d104d1fbbb9d25f8c6e3e152b46214211cc7f38c583c815dc51`  
		Last Modified: Sat, 19 Sep 2020 00:50:20 GMT  
		Size: 148.8 MB (148839733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e9a02b211814f8cfe3cc5588605a1bcb617e567ba27299e9972802c52bb5b9`  
		Last Modified: Sat, 19 Sep 2020 00:49:54 GMT  
		Size: 2.8 KB (2844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python37` - linux; arm variant v5

```console
$ docker pull plone@sha256:3c914cdfffffd329b88a4a1bbcd2abce02b3290477cae9779bcda90c0e00acb6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178228840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53fa5f81253500b80dd0e5dc05685bba9bbbcefa443835e5fa8af72cbf8fac7e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 09 Sep 2020 23:53:49 GMT
ADD file:34835d84d87e3ee1178aa150793d75a4d4a7a28c013ca3495dbcca2b570270bf in / 
# Wed, 09 Sep 2020 23:53:53 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 07:30:10 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 07:30:11 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 07:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 08:28:15 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 08:28:17 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 08:44:27 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 08:44:50 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 08:44:53 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 08:44:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 08:45:00 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 08:45:45 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 08:45:50 GMT
CMD ["python3"]
# Sat, 19 Sep 2020 00:06:47 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Sat, 19 Sep 2020 00:06:56 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Sat, 19 Sep 2020 00:07:38 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Sat, 19 Sep 2020 00:07:51 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 00:21:55 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 00:22:07 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 00:22:34 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Sat, 19 Sep 2020 00:22:48 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 00:22:56 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 00:23:05 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 00:23:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 00:23:27 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0a51b5143468e1b44dafa16fea3541e28e369071f6837337ee95e37f0ad81d99`  
		Last Modified: Thu, 10 Sep 2020 00:02:48 GMT  
		Size: 24.8 MB (24835974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f7f84dcaf455e5855a19d17b45c956054d715bebddc69382b6f8d9d74771e9`  
		Last Modified: Thu, 10 Sep 2020 10:37:26 GMT  
		Size: 2.4 MB (2448920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664f8820e212bf50649a2df56390841cd8567442e610b785dd2b8fbf74b9bfcd`  
		Last Modified: Thu, 10 Sep 2020 10:38:30 GMT  
		Size: 9.7 MB (9740965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1853d44438b0b9144457951f5e8b2607518f5f6610186acc660ee6748e43e082`  
		Last Modified: Thu, 10 Sep 2020 10:38:26 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775cb1bbbc6e63a1e61e95f440148b16f7fd2259f56157d081c798ebae21dba7`  
		Last Modified: Thu, 10 Sep 2020 10:38:27 GMT  
		Size: 2.4 MB (2408159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35bfe90ef5ccb834f094d8745506bd1122389dc4af2e9d1a1f744ecf77722f3`  
		Last Modified: Sat, 19 Sep 2020 00:41:29 GMT  
		Size: 3.9 KB (3941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fcb2164b0844636798bf02aeccf20e07bc41f7e3de6c13e6c5ec4c698d8409`  
		Last Modified: Sat, 19 Sep 2020 00:41:29 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2761d5f31c2c17d3e44d21c0e39ec4b81c80e9458fab437b555018c26f12da18`  
		Last Modified: Sat, 19 Sep 2020 00:42:17 GMT  
		Size: 138.8 MB (138786754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccdd06d362da1232814e4ad6843d0f9fa915cabf42ac0581c57e5ef61746edd`  
		Last Modified: Sat, 19 Sep 2020 00:41:28 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python37` - linux; arm variant v7

```console
$ docker pull plone@sha256:cad4c5a00f4eeb40814e4de37c51e0c6dfa2e1aa46645b2c816b24111bbd2d8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174317582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a12ee1c00d114423c18cb8eb2457aab052b57fade2a1e000b270eb77805593`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 10 Sep 2020 00:08:04 GMT
ADD file:5ec0d2c3043ae64cb72698b0f6fe7387884f4195df962466215ce534d2208327 in / 
# Thu, 10 Sep 2020 00:08:06 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 14:43:21 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 14:43:42 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 14:45:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 15:44:26 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 15:44:27 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 16:00:12 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 16:00:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 16:00:25 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 16:00:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 16:00:27 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 16:01:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 16:01:10 GMT
CMD ["python3"]
# Sat, 19 Sep 2020 00:33:54 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Sat, 19 Sep 2020 00:34:03 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Sat, 19 Sep 2020 00:34:31 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Sat, 19 Sep 2020 00:34:43 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 00:46:45 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 00:47:04 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 00:47:24 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Sat, 19 Sep 2020 00:47:34 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 00:47:48 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 00:48:05 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 00:48:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 00:48:34 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:a7c65856610cb24c46ede2ffe313cbf933c44fa20ba213835af953646f3eb1ed`  
		Last Modified: Thu, 10 Sep 2020 00:17:52 GMT  
		Size: 22.7 MB (22699896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d804fbb637381cd4f9ca3a07c8e0b3da642d028734d7fd49ad91a58fa71bfb`  
		Last Modified: Thu, 10 Sep 2020 17:54:46 GMT  
		Size: 2.3 MB (2347444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45712f189332ede475923a5981e3e50b6da0279cc54133fbaaea99f8ef390689`  
		Last Modified: Thu, 10 Sep 2020 17:56:19 GMT  
		Size: 9.3 MB (9313642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb09030de47ba366c5a8c04b033a367b5b76a3de49e9fe788490f9c85b0ab9a3`  
		Last Modified: Thu, 10 Sep 2020 17:56:16 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ba6eee29ca75ac119a23db2b258df3df9a6b73a1d02d5a17c9156aa1617ee9`  
		Last Modified: Thu, 10 Sep 2020 17:56:17 GMT  
		Size: 2.4 MB (2408116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722e6c087f369594a194f2549fe560d1a7876956ce49d41b4b25a880ee937fc7`  
		Last Modified: Sat, 19 Sep 2020 01:07:41 GMT  
		Size: 3.9 KB (3942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbab31a999cba6a0f7300625fb28f9d29dfa785506b8581df355fae1001ee610`  
		Last Modified: Sat, 19 Sep 2020 01:07:41 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838229d296ab4cce82845a67a7124a3d86aed405e7454254da4cc2369f26e29`  
		Last Modified: Sat, 19 Sep 2020 01:08:34 GMT  
		Size: 137.5 MB (137540417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a74881b383b1f2b2bb891cf4589274124ed2fe61a29bb47c8f0bec8e033c57f`  
		Last Modified: Sat, 19 Sep 2020 01:07:41 GMT  
		Size: 2.8 KB (2844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python37` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:1ccd4d53a5cb22696271fbadce2a04b0e5285a576d3e1601ccbbc0fc2bb62169
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180885763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e9721013aa854edfd0f3f32318a3001a7fef9f37d23511ac5333903dfd053d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 14:43:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 14:43:52 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 14:45:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 15:32:45 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 15:32:46 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 15:46:13 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 15:46:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 15:46:17 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 15:46:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 15:46:19 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 15:46:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 15:46:43 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:53:30 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:53:31 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:53:33 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:53:34 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 00:08:08 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 00:08:21 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 00:08:22 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Sat, 19 Sep 2020 00:08:24 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 00:08:25 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 00:08:26 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 00:08:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 00:08:28 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73aab3bdbed885a7b51e5d6142da269ed9b6d4e447f902edf1b83581f5bd4386`  
		Last Modified: Thu, 10 Sep 2020 17:25:54 GMT  
		Size: 2.6 MB (2622846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8402c6fdb392ce21b77f3b732eb3f024d23798355df3744e441057203c990bf5`  
		Last Modified: Thu, 10 Sep 2020 17:27:03 GMT  
		Size: 10.1 MB (10100857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89859317f5be5569a961a09e5350149ad04fc43ff72a0cb50af1a90c14eb4996`  
		Last Modified: Thu, 10 Sep 2020 17:27:01 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044c3ed0d4de82bfb7dd497c99f4d2999a669c8f90d65ebb03fa70a940193e82`  
		Last Modified: Thu, 10 Sep 2020 17:27:01 GMT  
		Size: 2.4 MB (2408507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7b75a3697d6c169a1042911ece940b5908cf9d1d47bcc42bfbbaf5904114df`  
		Last Modified: Sat, 19 Sep 2020 00:44:16 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0784b9ec59f17ccce07dbea67606d8e2f69922240acc12e939563c83a8d31c`  
		Last Modified: Sat, 19 Sep 2020 00:44:16 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7582c0f7cd430458d45ff8ece8beb895ca7358d06cd0269519c4790398485c63`  
		Last Modified: Sat, 19 Sep 2020 00:45:05 GMT  
		Size: 139.9 MB (139896147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ac853dd1e7d4460e4b4fdf6d76a8680987e4c8033e72940003e9269a72d967`  
		Last Modified: Sat, 19 Sep 2020 00:44:17 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python37` - linux; 386

```console
$ docker pull plone@sha256:163c170dd60d0708823c925a0ef9c18d9541858fdad7cb728ac67923d276309f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190302325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5f16d91d6da43164182c3ea3ec2dbec219980fbc2b9224642a99f854b2f2e4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 12:08:06 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 12:08:06 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 12:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 13:04:14 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 13:04:14 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 13:20:13 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 13:20:14 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 13:20:15 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 13:20:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 13:20:16 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 13:20:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 13:20:35 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:42:31 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:42:31 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:42:32 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:42:33 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:46:13 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:46:14 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:46:15 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:46:15 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:46:15 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:46:15 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:46:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:46:16 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d544ba083dbbb592a070f573056e56421093aaefdcfd18226c45aea7640564ce`  
		Last Modified: Thu, 10 Sep 2020 15:17:32 GMT  
		Size: 2.8 MB (2764118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada7f75be7e313c1417d4eef6a4ecf8a8a3e777252f35c70d9f97ce7e650e639`  
		Last Modified: Thu, 10 Sep 2020 15:18:47 GMT  
		Size: 10.2 MB (10167326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995322669b2e9c9e3aa6e6aadd59765980a29fc10c205919044c29adfd3da3be`  
		Last Modified: Thu, 10 Sep 2020 15:18:42 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb83ff96ffd0669278942525f75b196ee5136e94137663f90e352e0f2c555651`  
		Last Modified: Thu, 10 Sep 2020 15:18:45 GMT  
		Size: 2.4 MB (2407567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8f11c57212e0df747cfa3494892ad3114979d8e9a02473f6f95ef5009f1fa8`  
		Last Modified: Sat, 19 Sep 2020 00:02:26 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1595f2d72404e233016d775816de60b3e554c3439fd21755435fa0d58e26f4d`  
		Last Modified: Sat, 19 Sep 2020 00:02:26 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079cc4eb77c78c58115436732433ac44b03d7cf2ace7497fab6fb84550609597`  
		Last Modified: Sat, 19 Sep 2020 00:03:02 GMT  
		Size: 147.2 MB (147204969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614eb21f6d14c022667955f63cf6ecd4c1bba1bf14909b068545980efba89fe1`  
		Last Modified: Sat, 19 Sep 2020 00:02:26 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python37` - linux; ppc64le

```console
$ docker pull plone@sha256:754e09e739c508861c50bbcc2b2e1aabc89a13ee14c1de4640ed14c41f9ae55d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.2 MB (189167340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbaea6d28f48c5a3e37b47751b65ea3e7bbf1deb8b7df2293d4587c18d5950b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:11 GMT
ADD file:4dede556abae88027bd22f3166fdbc38778a6fcd686c5ce768c3ca024ab3f9cf in / 
# Thu, 10 Sep 2020 01:06:20 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 07:50:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 07:50:29 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 07:51:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 09:21:54 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 09:22:01 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 09:44:49 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 09:45:03 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 09:45:14 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 09:45:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 09:45:28 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 09:46:19 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 09:46:24 GMT
CMD ["python3"]
# Sat, 19 Sep 2020 01:34:02 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Sat, 19 Sep 2020 01:34:13 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Sat, 19 Sep 2020 01:34:48 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Sat, 19 Sep 2020 01:34:52 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 02:29:31 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 02:29:45 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 02:29:49 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Sat, 19 Sep 2020 02:30:02 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 02:30:26 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 02:30:43 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 02:30:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 02:31:00 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:f8aef3d2247e5f990bc767bc99f575b9bcec34aaa37183414eebe28fcd09519d`  
		Last Modified: Thu, 10 Sep 2020 01:28:12 GMT  
		Size: 30.5 MB (30517880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4d247642a66d35883ab30db545f1107dcb4bbab943229fb877b803001699e8`  
		Last Modified: Thu, 10 Sep 2020 10:57:57 GMT  
		Size: 2.9 MB (2871879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf8714fd06908708d9ebfced8229490bb9a7660221b24caa6ce3f07c1f4f5c9`  
		Last Modified: Thu, 10 Sep 2020 11:01:20 GMT  
		Size: 10.9 MB (10860153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bea689dd9df1f3c5c439d9abd188cc6ce0fc06d038065b17c9efa373ced626e`  
		Last Modified: Thu, 10 Sep 2020 11:00:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe3e54535f0df1c812729c7f18dd8a62aa166ea126a6fed07daee158f6a4da1`  
		Last Modified: Thu, 10 Sep 2020 11:01:07 GMT  
		Size: 2.4 MB (2409952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced1aaf911a254b8b889ec8ea5bcfe9bf6890d0f0883731b47ec21a34711dfd1`  
		Last Modified: Sat, 19 Sep 2020 03:24:26 GMT  
		Size: 4.0 KB (3965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef287ec433394d4d2e71c6beedf5c980cd1c3f75c8ad72de3a97f23d691ffb5`  
		Last Modified: Sat, 19 Sep 2020 03:24:25 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c580df630dcae0300930626f7a5b1c90e45ddce88009ee0567a939748287938`  
		Last Modified: Sat, 19 Sep 2020 03:28:20 GMT  
		Size: 142.5 MB (142499382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0ae4972ae29c4b85b95006983cf962fee68311864a2b291ac08c57d4983b9a`  
		Last Modified: Sat, 19 Sep 2020 03:24:25 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python37` - linux; s390x

```console
$ docker pull plone@sha256:150303d1edfeadc3985b8f7ef2c42a5620d90af64ac7a63ca631a1eaa4b864ee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.2 MB (180224738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29fa09f9ad7a4abc06263b3967c2a7fae08fbe7416bc808af607a95b6bb8803`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 02:08:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 02:08:40 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 02:08:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:29:24 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 02:29:24 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 02:34:31 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:34:32 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:34:33 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:34:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:34:33 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:34:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:34:47 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:48:38 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:48:38 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:48:39 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:48:39 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:53:34 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:53:42 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:53:42 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:53:42 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:53:43 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:53:43 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:53:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:53:43 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:07e4a6dbced6eed74bdb331987f95c00aa5b46543570b7adc1575121e66102dd`  
		Last Modified: Wed, 09 Sep 2020 23:46:28 GMT  
		Size: 25.7 MB (25707597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74271825cb478ad15a51d22ed474afc61dd029f780c3fd46cd33f059bef09ac2`  
		Last Modified: Thu, 10 Sep 2020 02:53:03 GMT  
		Size: 2.4 MB (2444050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532e64f8fc6bc6b020c1b66ac90a20deaa7347529b07aca50a3c4badc342ade3`  
		Last Modified: Thu, 10 Sep 2020 02:53:46 GMT  
		Size: 10.0 MB (9958159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b376f03fc298a3b87c34cc812e00e98eddd8216236f594b04175ecbfe8d7ef27`  
		Last Modified: Thu, 10 Sep 2020 02:53:44 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4546d813b69ec76b44829d50d25fe6859f27bc5e5e4ac15b3d8cb2867fed0c76`  
		Last Modified: Thu, 10 Sep 2020 02:53:45 GMT  
		Size: 2.4 MB (2407641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1848b50afabad8d209691407d42fcf78a82074004e3e12a71d2b80e14a917602`  
		Last Modified: Sat, 19 Sep 2020 00:06:58 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03149d5c00ffaefa86c8878b47131aa1f572a8918ea72af03e1347ca524ddd4d`  
		Last Modified: Sat, 19 Sep 2020 00:06:58 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e266dd74f90009b1c7f05ab968c92696bbb03f69c13f1539b4a878926ac36704`  
		Last Modified: Sat, 19 Sep 2020 00:07:17 GMT  
		Size: 139.7 MB (139699212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f1a813842fc647a09301e74401df671d8ffb613af7c9a4e033be7558b60d8e`  
		Last Modified: Sat, 19 Sep 2020 00:06:58 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
