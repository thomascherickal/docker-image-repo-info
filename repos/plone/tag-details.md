<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `plone`

-	[`plone:5`](#plone5)
-	[`plone:5.2`](#plone52)
-	[`plone:5.2.2`](#plone522)
-	[`plone:5.2.2-alpine`](#plone522-alpine)
-	[`plone:5.2.2-python36`](#plone522-python36)
-	[`plone:5.2.2-python37`](#plone522-python37)
-	[`plone:5.2.2-python38`](#plone522-python38)
-	[`plone:5.2-alpine`](#plone52-alpine)
-	[`plone:5.2-python36`](#plone52-python36)
-	[`plone:5.2-python37`](#plone52-python37)
-	[`plone:5.2-python38`](#plone52-python38)
-	[`plone:5-alpine`](#plone5-alpine)
-	[`plone:5-python36`](#plone5-python36)
-	[`plone:5-python37`](#plone5-python37)
-	[`plone:5-python38`](#plone5-python38)
-	[`plone:alpine`](#plonealpine)
-	[`plone:latest`](#plonelatest)
-	[`plone:python36`](#plonepython36)
-	[`plone:python37`](#plonepython37)
-	[`plone:python38`](#plonepython38)

## `plone:5`

```console
$ docker pull plone@sha256:6b6714d5cc9e2d01fee3724de3081f7458d31d41d85829fa758497f6cdf54144
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

### `plone:5` - linux; amd64

```console
$ docker pull plone@sha256:ebdc38c5e493734989f7406c8549e8a8e93e0d5168711dfd6dfa48098fc4fe10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.9 MB (194934892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90313b8c04128be8ac3abbda43a853a92942ffd279c266a03e11bb2b5cfa5dd3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:37 GMT
ADD file:83fbd2352bbac612c7a954e19abd295607cea4482c556c225308e0241b58e2bf in / 
# Thu, 10 Sep 2020 00:30:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 17:34:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 17:34:09 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 17:34:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 17:34:20 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 17:34:21 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 17:45:06 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 17:45:08 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 17:45:08 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 17:45:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 17:45:09 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 17:45:30 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 17:45:30 GMT
CMD ["python3"]
# Fri, 11 Sep 2020 09:23:11 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 11 Sep 2020 09:23:11 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 11 Sep 2020 09:23:12 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 11 Sep 2020 09:23:12 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 11 Sep 2020 09:26:41 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 11 Sep 2020 09:26:42 GMT
VOLUME [/data]
# Fri, 11 Sep 2020 09:26:42 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 11 Sep 2020 09:26:42 GMT
EXPOSE 8080
# Fri, 11 Sep 2020 09:26:42 GMT
WORKDIR /plone/instance
# Fri, 11 Sep 2020 09:26:43 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 11 Sep 2020 09:26:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 09:26:43 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:abb454610128b028301ee40af387d31111a1e699e4ea424fd53186ff77067402`  
		Last Modified: Thu, 10 Sep 2020 00:37:40 GMT  
		Size: 22.5 MB (22522274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cca7c254bca20c23c661af2a80a9f2d26c1473a9fce0c4e7df958610e5125`  
		Last Modified: Thu, 10 Sep 2020 18:58:07 GMT  
		Size: 2.5 MB (2485508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09bd87eaacd2564a11aded5f30cdeb6f48fb6f0ede1e828f9ca1cb52c76a93`  
		Last Modified: Thu, 10 Sep 2020 18:58:09 GMT  
		Size: 10.0 MB (10001970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789a5a11aeffb2eca696932509ac931d098c347d5d4f76bfb854c3b094ef244b`  
		Last Modified: Thu, 10 Sep 2020 18:58:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c332a8eb758e8effc070d08aedc7897f523c1d278f86e45bb35ec19e7f177b51`  
		Last Modified: Thu, 10 Sep 2020 18:58:07 GMT  
		Size: 2.4 MB (2403392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bce5ab678c23e78b108965d3a61c3c48f7e7c07a9400e320ba9e75f83e4874e`  
		Last Modified: Fri, 11 Sep 2020 09:27:07 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d5dcf5c8e86e0104491f41454f0b87662688a91b5407e7bd3278c62eb81d84`  
		Last Modified: Fri, 11 Sep 2020 09:27:07 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee1a5781ad28ed02807ce2b28a303542c1715c0c2ef6af3d1b501369273f6b2`  
		Last Modified: Fri, 11 Sep 2020 09:27:35 GMT  
		Size: 157.5 MB (157513738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a359a8a5b787f8bb19700bb2d05fdff702bc88d675103ea127fba012ee46dc`  
		Last Modified: Fri, 11 Sep 2020 09:27:07 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; arm variant v5

```console
$ docker pull plone@sha256:55fc5ce26d1c18a9f41d85bc7ccae2d67d77e2c05cd5922583c20bf350709645
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.8 MB (184750879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f651fc0f3ff0e19b19a06bd28a0424b80472e6ad864fe4c607fcc9eec98f209`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 09 Sep 2020 23:58:43 GMT
ADD file:696a886e620f9d4e01408d475f27ce43a516a44e3689fd1bd6fa9452e27b9672 in / 
# Wed, 09 Sep 2020 23:58:46 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 08:58:06 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 08:58:10 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 08:58:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 08:59:03 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 08:59:07 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 09:09:54 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 09:10:10 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 09:10:12 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 09:10:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 09:10:17 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 09:11:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 09:11:12 GMT
CMD ["python3"]
# Thu, 10 Sep 2020 19:15:10 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 10 Sep 2020 19:15:17 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 10 Sep 2020 19:15:47 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 10 Sep 2020 19:15:59 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 10 Sep 2020 19:32:08 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 10 Sep 2020 19:32:17 GMT
VOLUME [/data]
# Thu, 10 Sep 2020 19:32:28 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Thu, 10 Sep 2020 19:32:28 GMT
EXPOSE 8080
# Thu, 10 Sep 2020 19:32:31 GMT
WORKDIR /plone/instance
# Thu, 10 Sep 2020 19:32:32 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 10 Sep 2020 19:32:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 10 Sep 2020 19:32:36 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:90bb53eced8a0fc6f31bd3ebc211839305505d162e0df809dfd951cf263f765d`  
		Last Modified: Thu, 10 Sep 2020 00:07:19 GMT  
		Size: 21.2 MB (21194357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9cf59ab1cb8914a632bf6b662cee76a27d3fb7f167e3b50abe6b956af56aab`  
		Last Modified: Thu, 10 Sep 2020 10:39:07 GMT  
		Size: 2.2 MB (2216188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f969f0e2e34b8d1e1ddee7594c94d4992977aac6eee5f40c933e5874a44942`  
		Last Modified: Thu, 10 Sep 2020 10:39:07 GMT  
		Size: 9.3 MB (9349487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56387498a6686b53e8df6491d6a8a5f550681416c6bb394c685f4fbfa2d562f`  
		Last Modified: Thu, 10 Sep 2020 10:39:04 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fe0317644c554fae33bacb2798457d2800a811ec1192ca32387d197a304f00`  
		Last Modified: Thu, 10 Sep 2020 10:39:05 GMT  
		Size: 2.4 MB (2403383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eabec6799d345384ed00826b8f6a3bc9c885e008c4752fa530cf0a3a972fd59`  
		Last Modified: Thu, 10 Sep 2020 19:32:59 GMT  
		Size: 3.9 KB (3925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a0dcee0ed0a1f60cca259c8ca72e3ad39544757270af99dc3a5f015f75366a`  
		Last Modified: Thu, 10 Sep 2020 19:32:59 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37195679d86a086c24f48d2311172303814536a04691696e10dd30ed98ebf43c`  
		Last Modified: Thu, 10 Sep 2020 19:34:00 GMT  
		Size: 149.6 MB (149579408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eb429f60a5e40315c870c33511a46bf8bf7fffb1742e006f3826351d366706`  
		Last Modified: Thu, 10 Sep 2020 19:32:59 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; arm variant v7

```console
$ docker pull plone@sha256:e7e4a86cd6cbb7d3bea3c938a0c10b902bdd7d4beec8dd0979c0de0b4abb9468
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.3 MB (181345132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90b04dd3423b22037aadf7ebe870b682f63e9990dea3cbcbd995e2d331c96e23`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 10 Sep 2020 00:13:48 GMT
ADD file:01ae1c10181763bd674d028f8ce4e5e3bf24c400e60a76fa6bfb43dfba07a0c6 in / 
# Thu, 10 Sep 2020 00:13:49 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 16:14:36 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 16:14:38 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 16:15:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 16:15:04 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 16:15:11 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 16:28:12 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 16:28:18 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 16:28:20 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 16:28:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 16:28:22 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 16:28:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 16:28:53 GMT
CMD ["python3"]
# Fri, 11 Sep 2020 04:51:12 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 11 Sep 2020 04:51:13 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 11 Sep 2020 04:51:17 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 11 Sep 2020 04:51:18 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 11 Sep 2020 05:07:57 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 11 Sep 2020 05:08:05 GMT
VOLUME [/data]
# Fri, 11 Sep 2020 05:08:14 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 11 Sep 2020 05:08:19 GMT
EXPOSE 8080
# Fri, 11 Sep 2020 05:08:22 GMT
WORKDIR /plone/instance
# Fri, 11 Sep 2020 05:08:24 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 11 Sep 2020 05:08:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 05:08:30 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:a1f2bf709796106dda8cc033b6c173e05f0838e1cf4fca653453e2999db8ba3d`  
		Last Modified: Thu, 10 Sep 2020 00:21:34 GMT  
		Size: 19.3 MB (19304627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c541d096a8ce835222b7505b2199a2fd665a67869c8b9f2b755129cb51b196b`  
		Last Modified: Thu, 10 Sep 2020 17:56:46 GMT  
		Size: 2.1 MB (2137387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed09475193f741bd43d93b83b2444cd94399ddcb2227a975304d68a02739e9d`  
		Last Modified: Thu, 10 Sep 2020 17:56:49 GMT  
		Size: 9.3 MB (9293956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d92008ba9651d6514e888d47be1fc262c6865cea3ec182df358577122da74`  
		Last Modified: Thu, 10 Sep 2020 17:56:45 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c12dad74ce56058362a96366b340dc87dc49f87db04e8d14246e63c4ad595a`  
		Last Modified: Thu, 10 Sep 2020 17:56:46 GMT  
		Size: 2.4 MB (2403222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b12d2097cddc00d8db45b6d11749e79e017704fb550fc0ab5c4d151b3dafdc3`  
		Last Modified: Fri, 11 Sep 2020 05:08:57 GMT  
		Size: 3.9 KB (3929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31af93954426c019718919233f3eb15206a5604cc98413e48cfdec64cdabda5`  
		Last Modified: Fri, 11 Sep 2020 05:08:57 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbcda2cc2eed5bbdea9a6c0752685ecdacb64742ca600ccd87b8ea556d8bcc8`  
		Last Modified: Fri, 11 Sep 2020 05:09:50 GMT  
		Size: 148.2 MB (148197887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c852bedef85ad01caf0e6adeec2050bfe963ac73e101e5e111ee34064b1bf6c`  
		Last Modified: Fri, 11 Sep 2020 05:08:57 GMT  
		Size: 2.8 KB (2842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:51a5ef5b8e0a46874b7d0c346711b28142cdb2d1bc4464925d46008c2087714a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183646561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5530a8485ac8504e02417863492f96199338b356dc633935263d903ffc48f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 09 Sep 2020 23:54:57 GMT
ADD file:fe3fc1ceb78e0b280e8429ba94710b765701de58e9958d27e9bcb8af97084f1b in / 
# Wed, 09 Sep 2020 23:55:02 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 15:58:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 15:58:53 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 15:59:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 15:59:13 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 15:59:15 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 16:11:48 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 16:11:51 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 16:11:52 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 16:11:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 16:11:53 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 16:12:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 16:12:27 GMT
CMD ["python3"]
# Fri, 11 Sep 2020 05:34:51 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 11 Sep 2020 05:34:52 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 11 Sep 2020 05:34:54 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 11 Sep 2020 05:34:55 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 11 Sep 2020 05:48:37 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 11 Sep 2020 05:48:53 GMT
VOLUME [/data]
# Fri, 11 Sep 2020 05:48:55 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 11 Sep 2020 05:48:56 GMT
EXPOSE 8080
# Fri, 11 Sep 2020 05:48:57 GMT
WORKDIR /plone/instance
# Fri, 11 Sep 2020 05:48:58 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 11 Sep 2020 05:48:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 05:48:59 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:852f38eca5e441cf6f4d6130ee167637bc8117d57f8f0156f5e489e8c3dd8f17`  
		Last Modified: Thu, 10 Sep 2020 00:01:56 GMT  
		Size: 20.4 MB (20377071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f37090d4a5cb835b768bdf2699c911f0d448d9c2ca155d22255740e1ed5eecb`  
		Last Modified: Thu, 10 Sep 2020 17:27:27 GMT  
		Size: 2.2 MB (2199149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a13a01028a219e1cf6f205fffbe7c8710d3b9fa672a17e292b9beae219621f`  
		Last Modified: Thu, 10 Sep 2020 17:27:28 GMT  
		Size: 9.7 MB (9722632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1604b0bb945c7009c3415dc70b9f5c77788464915e5e66ae28849eebc00f1b`  
		Last Modified: Thu, 10 Sep 2020 17:27:27 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd33a7d62112a6c753efacdcd14552b92159c77e934e8a618c50b69f80ac5dc`  
		Last Modified: Thu, 10 Sep 2020 17:27:27 GMT  
		Size: 2.4 MB (2403257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747938999dff604308ed02632aded572c40d7283f6e6c5bc012669a32f68621e`  
		Last Modified: Fri, 11 Sep 2020 05:49:30 GMT  
		Size: 3.9 KB (3940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00c3f60827996df5d7871fe08adbbff9791371cf329fec661818b1782329da`  
		Last Modified: Fri, 11 Sep 2020 05:49:30 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f426165c88c4f688b22dbae86d6e8f93eb94028c33457cb7e525d908ee0f225`  
		Last Modified: Fri, 11 Sep 2020 05:50:13 GMT  
		Size: 148.9 MB (148936386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38ca0ab5fcb0370dcc883c56af596750de0fc74d29827b575efe5f1416f7c4a`  
		Last Modified: Fri, 11 Sep 2020 05:49:31 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; 386

```console
$ docker pull plone@sha256:74dae2a340501d74b181e6f810bcc5987c5100d435af746737c7cd0228deea0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191123328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6446e55c7fa3222601f6ce73289c88370dc91240430988053f72b10cecd98b4`
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
# Thu, 10 Sep 2020 12:08:17 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 12:37:25 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 12:50:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 12:50:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 12:50:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 12:50:46 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:38:43 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:38:44 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:38:44 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:38:45 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:42:19 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:42:20 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:42:20 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:42:20 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:42:20 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:42:21 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:42:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:42:21 GMT
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
	-	`sha256:9f8d61ae8767c42662c4758765a4389aafccb33e94098c128d01e1436856e52a`  
		Last Modified: Thu, 10 Sep 2020 15:18:10 GMT  
		Size: 10.5 MB (10532513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fa521131d6f14a06ff5a2ba860f47bc766c993ceeacd79a375a2f8aaf1b970`  
		Last Modified: Thu, 10 Sep 2020 15:18:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b31a66bd5005cb79acf880a9bd8e2446aaa63a0e6a12ca44b136526373f7a6f`  
		Last Modified: Thu, 10 Sep 2020 15:18:06 GMT  
		Size: 2.4 MB (2407674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549278a7ff3477d1945b1c6c146a7886ea07a6e80eef07fab39ab361547ce5`  
		Last Modified: Sat, 19 Sep 2020 00:01:42 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921c0542d2620f8af6980da808c1cb6275509da47bcd7b7d17dcf0b53537c9b`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a986571b35c520ca4a2ac4d08cd48b1c84845ca0481766a1701911d257c9fe60`  
		Last Modified: Sat, 19 Sep 2020 00:02:17 GMT  
		Size: 147.7 MB (147660673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649957d7f083af5b1197f2a13e28fefffb9d9e28e07c525e8907479caf613aa`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; ppc64le

```console
$ docker pull plone@sha256:c3c2b4338c89e4b0dc0ebf0d2e7adbaaeba330d601d4ec045cd4b61db5a1b407
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197172893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c73e6fb8803df461bdc412f5b0178f5c2999e3996822554ff3965f1db75dc6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 19:31:59 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 19:32:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 19:32:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 19:33:02 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 30 Jun 2020 19:03:08 GMT
ENV PYTHON_VERSION=3.7.8
# Tue, 30 Jun 2020 19:23:23 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 30 Jun 2020 19:23:36 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 30 Jun 2020 19:23:41 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Tue, 30 Jun 2020 19:23:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Tue, 30 Jun 2020 19:23:55 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Tue, 30 Jun 2020 19:25:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 30 Jun 2020 19:25:56 GMT
CMD ["python3"]
# Tue, 30 Jun 2020 22:42:09 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Tue, 30 Jun 2020 22:42:11 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Tue, 30 Jun 2020 22:42:20 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Tue, 30 Jun 2020 22:42:22 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Tue, 30 Jun 2020 23:05:01 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Tue, 30 Jun 2020 23:05:09 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:05:10 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Tue, 30 Jun 2020 23:05:13 GMT
EXPOSE 8080
# Tue, 30 Jun 2020 23:05:19 GMT
WORKDIR /plone/instance
# Tue, 30 Jun 2020 23:05:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Tue, 30 Jun 2020 23:05:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 30 Jun 2020 23:05:31 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65db400552099f2d550e694f8b2c4585a9241771c3888459e95933e3952c00a2`  
		Last Modified: Tue, 09 Jun 2020 22:04:50 GMT  
		Size: 2.1 MB (2149602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08384149d3416d25ce4786393ffc43365435b8ee5abe3a9b312b54e165b338b`  
		Last Modified: Tue, 30 Jun 2020 21:03:12 GMT  
		Size: 19.7 MB (19714165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5889ef0bc0f687b9775913850358909987604b1b5d929b521c1ed81b9fb3e679`  
		Last Modified: Tue, 30 Jun 2020 21:03:05 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b9d713da50b69b94f1ac3a37593022c77b377fb92afa52673934aa329b289`  
		Last Modified: Tue, 30 Jun 2020 21:03:06 GMT  
		Size: 2.2 MB (2216976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b3530a849735869c2a1882cba7beda7a6fee1202289f9c121d1ec39ec3d94e`  
		Last Modified: Tue, 30 Jun 2020 23:25:33 GMT  
		Size: 3.9 KB (3942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd61c145fe975fa9ac1f3222cd64a118b9553bf87c70a56d6602c1c7134443e8`  
		Last Modified: Tue, 30 Jun 2020 23:25:32 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc23229b857f88f77670bce57410e2d75ee5cf23cdd61013b64e37d3cd424ad6`  
		Last Modified: Tue, 30 Jun 2020 23:26:05 GMT  
		Size: 150.3 MB (150292808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382269925414c1f4ccc45274913d6519255ceefabd509d702ab18e80b1100219`  
		Last Modified: Tue, 30 Jun 2020 23:25:32 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; s390x

```console
$ docker pull plone@sha256:2d15e6aa00ff378d2b1c5ea04fca06fce7564ddd991740a237282575c440a1b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180905670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6cc06ff3ca729bed0d018430778a47ff947f360d63b0e54044544f456f417f0`
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
# Thu, 10 Sep 2020 02:08:45 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 02:18:52 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 02:23:40 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:23:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:23:42 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:23:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:23:51 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:43:00 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:43:00 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:43:01 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:43:01 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:48:14 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:48:22 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:48:22 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:48:22 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:48:23 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:48:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:48:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:48:23 GMT
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
	-	`sha256:b7a30ebb749e95a6400495190e32c5b98f37145cc1741244dd3975f759240137`  
		Last Modified: Thu, 10 Sep 2020 02:53:24 GMT  
		Size: 10.3 MB (10274354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9331aa7a0a92e572dee8bf61940f31b2a95c5096898cb20f1592c6e7149db9`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465df3edf63ab70b456383487b281eec77a1064cc829206ac8fd4a9a5b77e0a2`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 2.4 MB (2407622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46fa9d8ec0f2f24706bd965bfcf0afdecd54e6df8bf5df97ae4567053cb3225`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274569e67c881a677c19e6c191f41a2ac47154ec5053ed091e4c33e6347cc6eb`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4b6a40bcb4cc4d2062a10c6aef8541998d6d36cf3acab5c17d269045be4ba`  
		Last Modified: Sat, 19 Sep 2020 00:06:46 GMT  
		Size: 140.1 MB (140063970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8675018f02a5e0a640222ef7297d4581a6cd3f0a81b53d05be3af657cafc95e1`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2`

```console
$ docker pull plone@sha256:6b6714d5cc9e2d01fee3724de3081f7458d31d41d85829fa758497f6cdf54144
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

### `plone:5.2` - linux; amd64

```console
$ docker pull plone@sha256:ebdc38c5e493734989f7406c8549e8a8e93e0d5168711dfd6dfa48098fc4fe10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.9 MB (194934892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90313b8c04128be8ac3abbda43a853a92942ffd279c266a03e11bb2b5cfa5dd3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:37 GMT
ADD file:83fbd2352bbac612c7a954e19abd295607cea4482c556c225308e0241b58e2bf in / 
# Thu, 10 Sep 2020 00:30:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 17:34:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 17:34:09 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 17:34:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 17:34:20 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 17:34:21 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 17:45:06 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 17:45:08 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 17:45:08 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 17:45:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 17:45:09 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 17:45:30 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 17:45:30 GMT
CMD ["python3"]
# Fri, 11 Sep 2020 09:23:11 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 11 Sep 2020 09:23:11 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 11 Sep 2020 09:23:12 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 11 Sep 2020 09:23:12 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 11 Sep 2020 09:26:41 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 11 Sep 2020 09:26:42 GMT
VOLUME [/data]
# Fri, 11 Sep 2020 09:26:42 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 11 Sep 2020 09:26:42 GMT
EXPOSE 8080
# Fri, 11 Sep 2020 09:26:42 GMT
WORKDIR /plone/instance
# Fri, 11 Sep 2020 09:26:43 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 11 Sep 2020 09:26:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 09:26:43 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:abb454610128b028301ee40af387d31111a1e699e4ea424fd53186ff77067402`  
		Last Modified: Thu, 10 Sep 2020 00:37:40 GMT  
		Size: 22.5 MB (22522274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cca7c254bca20c23c661af2a80a9f2d26c1473a9fce0c4e7df958610e5125`  
		Last Modified: Thu, 10 Sep 2020 18:58:07 GMT  
		Size: 2.5 MB (2485508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09bd87eaacd2564a11aded5f30cdeb6f48fb6f0ede1e828f9ca1cb52c76a93`  
		Last Modified: Thu, 10 Sep 2020 18:58:09 GMT  
		Size: 10.0 MB (10001970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789a5a11aeffb2eca696932509ac931d098c347d5d4f76bfb854c3b094ef244b`  
		Last Modified: Thu, 10 Sep 2020 18:58:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c332a8eb758e8effc070d08aedc7897f523c1d278f86e45bb35ec19e7f177b51`  
		Last Modified: Thu, 10 Sep 2020 18:58:07 GMT  
		Size: 2.4 MB (2403392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bce5ab678c23e78b108965d3a61c3c48f7e7c07a9400e320ba9e75f83e4874e`  
		Last Modified: Fri, 11 Sep 2020 09:27:07 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d5dcf5c8e86e0104491f41454f0b87662688a91b5407e7bd3278c62eb81d84`  
		Last Modified: Fri, 11 Sep 2020 09:27:07 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee1a5781ad28ed02807ce2b28a303542c1715c0c2ef6af3d1b501369273f6b2`  
		Last Modified: Fri, 11 Sep 2020 09:27:35 GMT  
		Size: 157.5 MB (157513738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a359a8a5b787f8bb19700bb2d05fdff702bc88d675103ea127fba012ee46dc`  
		Last Modified: Fri, 11 Sep 2020 09:27:07 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; arm variant v5

```console
$ docker pull plone@sha256:55fc5ce26d1c18a9f41d85bc7ccae2d67d77e2c05cd5922583c20bf350709645
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.8 MB (184750879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f651fc0f3ff0e19b19a06bd28a0424b80472e6ad864fe4c607fcc9eec98f209`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 09 Sep 2020 23:58:43 GMT
ADD file:696a886e620f9d4e01408d475f27ce43a516a44e3689fd1bd6fa9452e27b9672 in / 
# Wed, 09 Sep 2020 23:58:46 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 08:58:06 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 08:58:10 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 08:58:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 08:59:03 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 08:59:07 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 09:09:54 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 09:10:10 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 09:10:12 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 09:10:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 09:10:17 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 09:11:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 09:11:12 GMT
CMD ["python3"]
# Thu, 10 Sep 2020 19:15:10 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 10 Sep 2020 19:15:17 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 10 Sep 2020 19:15:47 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 10 Sep 2020 19:15:59 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 10 Sep 2020 19:32:08 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 10 Sep 2020 19:32:17 GMT
VOLUME [/data]
# Thu, 10 Sep 2020 19:32:28 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Thu, 10 Sep 2020 19:32:28 GMT
EXPOSE 8080
# Thu, 10 Sep 2020 19:32:31 GMT
WORKDIR /plone/instance
# Thu, 10 Sep 2020 19:32:32 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 10 Sep 2020 19:32:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 10 Sep 2020 19:32:36 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:90bb53eced8a0fc6f31bd3ebc211839305505d162e0df809dfd951cf263f765d`  
		Last Modified: Thu, 10 Sep 2020 00:07:19 GMT  
		Size: 21.2 MB (21194357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9cf59ab1cb8914a632bf6b662cee76a27d3fb7f167e3b50abe6b956af56aab`  
		Last Modified: Thu, 10 Sep 2020 10:39:07 GMT  
		Size: 2.2 MB (2216188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f969f0e2e34b8d1e1ddee7594c94d4992977aac6eee5f40c933e5874a44942`  
		Last Modified: Thu, 10 Sep 2020 10:39:07 GMT  
		Size: 9.3 MB (9349487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56387498a6686b53e8df6491d6a8a5f550681416c6bb394c685f4fbfa2d562f`  
		Last Modified: Thu, 10 Sep 2020 10:39:04 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fe0317644c554fae33bacb2798457d2800a811ec1192ca32387d197a304f00`  
		Last Modified: Thu, 10 Sep 2020 10:39:05 GMT  
		Size: 2.4 MB (2403383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eabec6799d345384ed00826b8f6a3bc9c885e008c4752fa530cf0a3a972fd59`  
		Last Modified: Thu, 10 Sep 2020 19:32:59 GMT  
		Size: 3.9 KB (3925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a0dcee0ed0a1f60cca259c8ca72e3ad39544757270af99dc3a5f015f75366a`  
		Last Modified: Thu, 10 Sep 2020 19:32:59 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37195679d86a086c24f48d2311172303814536a04691696e10dd30ed98ebf43c`  
		Last Modified: Thu, 10 Sep 2020 19:34:00 GMT  
		Size: 149.6 MB (149579408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eb429f60a5e40315c870c33511a46bf8bf7fffb1742e006f3826351d366706`  
		Last Modified: Thu, 10 Sep 2020 19:32:59 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; arm variant v7

```console
$ docker pull plone@sha256:e7e4a86cd6cbb7d3bea3c938a0c10b902bdd7d4beec8dd0979c0de0b4abb9468
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.3 MB (181345132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90b04dd3423b22037aadf7ebe870b682f63e9990dea3cbcbd995e2d331c96e23`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 10 Sep 2020 00:13:48 GMT
ADD file:01ae1c10181763bd674d028f8ce4e5e3bf24c400e60a76fa6bfb43dfba07a0c6 in / 
# Thu, 10 Sep 2020 00:13:49 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 16:14:36 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 16:14:38 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 16:15:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 16:15:04 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 16:15:11 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 16:28:12 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 16:28:18 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 16:28:20 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 16:28:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 16:28:22 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 16:28:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 16:28:53 GMT
CMD ["python3"]
# Fri, 11 Sep 2020 04:51:12 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 11 Sep 2020 04:51:13 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 11 Sep 2020 04:51:17 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 11 Sep 2020 04:51:18 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 11 Sep 2020 05:07:57 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 11 Sep 2020 05:08:05 GMT
VOLUME [/data]
# Fri, 11 Sep 2020 05:08:14 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 11 Sep 2020 05:08:19 GMT
EXPOSE 8080
# Fri, 11 Sep 2020 05:08:22 GMT
WORKDIR /plone/instance
# Fri, 11 Sep 2020 05:08:24 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 11 Sep 2020 05:08:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 05:08:30 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:a1f2bf709796106dda8cc033b6c173e05f0838e1cf4fca653453e2999db8ba3d`  
		Last Modified: Thu, 10 Sep 2020 00:21:34 GMT  
		Size: 19.3 MB (19304627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c541d096a8ce835222b7505b2199a2fd665a67869c8b9f2b755129cb51b196b`  
		Last Modified: Thu, 10 Sep 2020 17:56:46 GMT  
		Size: 2.1 MB (2137387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed09475193f741bd43d93b83b2444cd94399ddcb2227a975304d68a02739e9d`  
		Last Modified: Thu, 10 Sep 2020 17:56:49 GMT  
		Size: 9.3 MB (9293956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d92008ba9651d6514e888d47be1fc262c6865cea3ec182df358577122da74`  
		Last Modified: Thu, 10 Sep 2020 17:56:45 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c12dad74ce56058362a96366b340dc87dc49f87db04e8d14246e63c4ad595a`  
		Last Modified: Thu, 10 Sep 2020 17:56:46 GMT  
		Size: 2.4 MB (2403222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b12d2097cddc00d8db45b6d11749e79e017704fb550fc0ab5c4d151b3dafdc3`  
		Last Modified: Fri, 11 Sep 2020 05:08:57 GMT  
		Size: 3.9 KB (3929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31af93954426c019718919233f3eb15206a5604cc98413e48cfdec64cdabda5`  
		Last Modified: Fri, 11 Sep 2020 05:08:57 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbcda2cc2eed5bbdea9a6c0752685ecdacb64742ca600ccd87b8ea556d8bcc8`  
		Last Modified: Fri, 11 Sep 2020 05:09:50 GMT  
		Size: 148.2 MB (148197887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c852bedef85ad01caf0e6adeec2050bfe963ac73e101e5e111ee34064b1bf6c`  
		Last Modified: Fri, 11 Sep 2020 05:08:57 GMT  
		Size: 2.8 KB (2842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:51a5ef5b8e0a46874b7d0c346711b28142cdb2d1bc4464925d46008c2087714a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183646561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5530a8485ac8504e02417863492f96199338b356dc633935263d903ffc48f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 09 Sep 2020 23:54:57 GMT
ADD file:fe3fc1ceb78e0b280e8429ba94710b765701de58e9958d27e9bcb8af97084f1b in / 
# Wed, 09 Sep 2020 23:55:02 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 15:58:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 15:58:53 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 15:59:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 15:59:13 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 15:59:15 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 16:11:48 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 16:11:51 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 16:11:52 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 16:11:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 16:11:53 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 16:12:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 16:12:27 GMT
CMD ["python3"]
# Fri, 11 Sep 2020 05:34:51 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 11 Sep 2020 05:34:52 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 11 Sep 2020 05:34:54 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 11 Sep 2020 05:34:55 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 11 Sep 2020 05:48:37 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 11 Sep 2020 05:48:53 GMT
VOLUME [/data]
# Fri, 11 Sep 2020 05:48:55 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 11 Sep 2020 05:48:56 GMT
EXPOSE 8080
# Fri, 11 Sep 2020 05:48:57 GMT
WORKDIR /plone/instance
# Fri, 11 Sep 2020 05:48:58 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 11 Sep 2020 05:48:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 05:48:59 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:852f38eca5e441cf6f4d6130ee167637bc8117d57f8f0156f5e489e8c3dd8f17`  
		Last Modified: Thu, 10 Sep 2020 00:01:56 GMT  
		Size: 20.4 MB (20377071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f37090d4a5cb835b768bdf2699c911f0d448d9c2ca155d22255740e1ed5eecb`  
		Last Modified: Thu, 10 Sep 2020 17:27:27 GMT  
		Size: 2.2 MB (2199149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a13a01028a219e1cf6f205fffbe7c8710d3b9fa672a17e292b9beae219621f`  
		Last Modified: Thu, 10 Sep 2020 17:27:28 GMT  
		Size: 9.7 MB (9722632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1604b0bb945c7009c3415dc70b9f5c77788464915e5e66ae28849eebc00f1b`  
		Last Modified: Thu, 10 Sep 2020 17:27:27 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd33a7d62112a6c753efacdcd14552b92159c77e934e8a618c50b69f80ac5dc`  
		Last Modified: Thu, 10 Sep 2020 17:27:27 GMT  
		Size: 2.4 MB (2403257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747938999dff604308ed02632aded572c40d7283f6e6c5bc012669a32f68621e`  
		Last Modified: Fri, 11 Sep 2020 05:49:30 GMT  
		Size: 3.9 KB (3940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00c3f60827996df5d7871fe08adbbff9791371cf329fec661818b1782329da`  
		Last Modified: Fri, 11 Sep 2020 05:49:30 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f426165c88c4f688b22dbae86d6e8f93eb94028c33457cb7e525d908ee0f225`  
		Last Modified: Fri, 11 Sep 2020 05:50:13 GMT  
		Size: 148.9 MB (148936386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38ca0ab5fcb0370dcc883c56af596750de0fc74d29827b575efe5f1416f7c4a`  
		Last Modified: Fri, 11 Sep 2020 05:49:31 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; 386

```console
$ docker pull plone@sha256:74dae2a340501d74b181e6f810bcc5987c5100d435af746737c7cd0228deea0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191123328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6446e55c7fa3222601f6ce73289c88370dc91240430988053f72b10cecd98b4`
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
# Thu, 10 Sep 2020 12:08:17 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 12:37:25 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 12:50:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 12:50:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 12:50:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 12:50:46 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:38:43 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:38:44 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:38:44 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:38:45 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:42:19 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:42:20 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:42:20 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:42:20 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:42:20 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:42:21 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:42:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:42:21 GMT
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
	-	`sha256:9f8d61ae8767c42662c4758765a4389aafccb33e94098c128d01e1436856e52a`  
		Last Modified: Thu, 10 Sep 2020 15:18:10 GMT  
		Size: 10.5 MB (10532513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fa521131d6f14a06ff5a2ba860f47bc766c993ceeacd79a375a2f8aaf1b970`  
		Last Modified: Thu, 10 Sep 2020 15:18:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b31a66bd5005cb79acf880a9bd8e2446aaa63a0e6a12ca44b136526373f7a6f`  
		Last Modified: Thu, 10 Sep 2020 15:18:06 GMT  
		Size: 2.4 MB (2407674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549278a7ff3477d1945b1c6c146a7886ea07a6e80eef07fab39ab361547ce5`  
		Last Modified: Sat, 19 Sep 2020 00:01:42 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921c0542d2620f8af6980da808c1cb6275509da47bcd7b7d17dcf0b53537c9b`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a986571b35c520ca4a2ac4d08cd48b1c84845ca0481766a1701911d257c9fe60`  
		Last Modified: Sat, 19 Sep 2020 00:02:17 GMT  
		Size: 147.7 MB (147660673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649957d7f083af5b1197f2a13e28fefffb9d9e28e07c525e8907479caf613aa`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; ppc64le

```console
$ docker pull plone@sha256:c3c2b4338c89e4b0dc0ebf0d2e7adbaaeba330d601d4ec045cd4b61db5a1b407
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197172893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c73e6fb8803df461bdc412f5b0178f5c2999e3996822554ff3965f1db75dc6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 19:31:59 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 19:32:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 19:32:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 19:33:02 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 30 Jun 2020 19:03:08 GMT
ENV PYTHON_VERSION=3.7.8
# Tue, 30 Jun 2020 19:23:23 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 30 Jun 2020 19:23:36 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 30 Jun 2020 19:23:41 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Tue, 30 Jun 2020 19:23:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Tue, 30 Jun 2020 19:23:55 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Tue, 30 Jun 2020 19:25:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 30 Jun 2020 19:25:56 GMT
CMD ["python3"]
# Tue, 30 Jun 2020 22:42:09 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Tue, 30 Jun 2020 22:42:11 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Tue, 30 Jun 2020 22:42:20 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Tue, 30 Jun 2020 22:42:22 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Tue, 30 Jun 2020 23:05:01 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Tue, 30 Jun 2020 23:05:09 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:05:10 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Tue, 30 Jun 2020 23:05:13 GMT
EXPOSE 8080
# Tue, 30 Jun 2020 23:05:19 GMT
WORKDIR /plone/instance
# Tue, 30 Jun 2020 23:05:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Tue, 30 Jun 2020 23:05:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 30 Jun 2020 23:05:31 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65db400552099f2d550e694f8b2c4585a9241771c3888459e95933e3952c00a2`  
		Last Modified: Tue, 09 Jun 2020 22:04:50 GMT  
		Size: 2.1 MB (2149602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08384149d3416d25ce4786393ffc43365435b8ee5abe3a9b312b54e165b338b`  
		Last Modified: Tue, 30 Jun 2020 21:03:12 GMT  
		Size: 19.7 MB (19714165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5889ef0bc0f687b9775913850358909987604b1b5d929b521c1ed81b9fb3e679`  
		Last Modified: Tue, 30 Jun 2020 21:03:05 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b9d713da50b69b94f1ac3a37593022c77b377fb92afa52673934aa329b289`  
		Last Modified: Tue, 30 Jun 2020 21:03:06 GMT  
		Size: 2.2 MB (2216976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b3530a849735869c2a1882cba7beda7a6fee1202289f9c121d1ec39ec3d94e`  
		Last Modified: Tue, 30 Jun 2020 23:25:33 GMT  
		Size: 3.9 KB (3942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd61c145fe975fa9ac1f3222cd64a118b9553bf87c70a56d6602c1c7134443e8`  
		Last Modified: Tue, 30 Jun 2020 23:25:32 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc23229b857f88f77670bce57410e2d75ee5cf23cdd61013b64e37d3cd424ad6`  
		Last Modified: Tue, 30 Jun 2020 23:26:05 GMT  
		Size: 150.3 MB (150292808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382269925414c1f4ccc45274913d6519255ceefabd509d702ab18e80b1100219`  
		Last Modified: Tue, 30 Jun 2020 23:25:32 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; s390x

```console
$ docker pull plone@sha256:2d15e6aa00ff378d2b1c5ea04fca06fce7564ddd991740a237282575c440a1b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180905670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6cc06ff3ca729bed0d018430778a47ff947f360d63b0e54044544f456f417f0`
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
# Thu, 10 Sep 2020 02:08:45 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 02:18:52 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 02:23:40 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:23:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:23:42 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:23:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:23:51 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:43:00 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:43:00 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:43:01 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:43:01 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:48:14 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:48:22 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:48:22 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:48:22 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:48:23 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:48:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:48:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:48:23 GMT
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
	-	`sha256:b7a30ebb749e95a6400495190e32c5b98f37145cc1741244dd3975f759240137`  
		Last Modified: Thu, 10 Sep 2020 02:53:24 GMT  
		Size: 10.3 MB (10274354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9331aa7a0a92e572dee8bf61940f31b2a95c5096898cb20f1592c6e7149db9`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465df3edf63ab70b456383487b281eec77a1064cc829206ac8fd4a9a5b77e0a2`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 2.4 MB (2407622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46fa9d8ec0f2f24706bd965bfcf0afdecd54e6df8bf5df97ae4567053cb3225`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274569e67c881a677c19e6c191f41a2ac47154ec5053ed091e4c33e6347cc6eb`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4b6a40bcb4cc4d2062a10c6aef8541998d6d36cf3acab5c17d269045be4ba`  
		Last Modified: Sat, 19 Sep 2020 00:06:46 GMT  
		Size: 140.1 MB (140063970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8675018f02a5e0a640222ef7297d4581a6cd3f0a81b53d05be3af657cafc95e1`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2.2`

```console
$ docker pull plone@sha256:df29336b72bd033353b7ca4d4f5f84e900b9abdf1dae32c45ba007eca9832a01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:5.2.2` - linux; 386

```console
$ docker pull plone@sha256:74dae2a340501d74b181e6f810bcc5987c5100d435af746737c7cd0228deea0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191123328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6446e55c7fa3222601f6ce73289c88370dc91240430988053f72b10cecd98b4`
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
# Thu, 10 Sep 2020 12:08:17 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 12:37:25 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 12:50:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 12:50:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 12:50:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 12:50:46 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:38:43 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:38:44 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:38:44 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:38:45 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:42:19 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:42:20 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:42:20 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:42:20 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:42:20 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:42:21 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:42:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:42:21 GMT
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
	-	`sha256:9f8d61ae8767c42662c4758765a4389aafccb33e94098c128d01e1436856e52a`  
		Last Modified: Thu, 10 Sep 2020 15:18:10 GMT  
		Size: 10.5 MB (10532513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fa521131d6f14a06ff5a2ba860f47bc766c993ceeacd79a375a2f8aaf1b970`  
		Last Modified: Thu, 10 Sep 2020 15:18:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b31a66bd5005cb79acf880a9bd8e2446aaa63a0e6a12ca44b136526373f7a6f`  
		Last Modified: Thu, 10 Sep 2020 15:18:06 GMT  
		Size: 2.4 MB (2407674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549278a7ff3477d1945b1c6c146a7886ea07a6e80eef07fab39ab361547ce5`  
		Last Modified: Sat, 19 Sep 2020 00:01:42 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921c0542d2620f8af6980da808c1cb6275509da47bcd7b7d17dcf0b53537c9b`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a986571b35c520ca4a2ac4d08cd48b1c84845ca0481766a1701911d257c9fe60`  
		Last Modified: Sat, 19 Sep 2020 00:02:17 GMT  
		Size: 147.7 MB (147660673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649957d7f083af5b1197f2a13e28fefffb9d9e28e07c525e8907479caf613aa`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.2` - linux; s390x

```console
$ docker pull plone@sha256:2d15e6aa00ff378d2b1c5ea04fca06fce7564ddd991740a237282575c440a1b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180905670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6cc06ff3ca729bed0d018430778a47ff947f360d63b0e54044544f456f417f0`
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
# Thu, 10 Sep 2020 02:08:45 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 02:18:52 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 02:23:40 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:23:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:23:42 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:23:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:23:51 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:43:00 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:43:00 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:43:01 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:43:01 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:48:14 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:48:22 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:48:22 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:48:22 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:48:23 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:48:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:48:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:48:23 GMT
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
	-	`sha256:b7a30ebb749e95a6400495190e32c5b98f37145cc1741244dd3975f759240137`  
		Last Modified: Thu, 10 Sep 2020 02:53:24 GMT  
		Size: 10.3 MB (10274354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9331aa7a0a92e572dee8bf61940f31b2a95c5096898cb20f1592c6e7149db9`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465df3edf63ab70b456383487b281eec77a1064cc829206ac8fd4a9a5b77e0a2`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 2.4 MB (2407622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46fa9d8ec0f2f24706bd965bfcf0afdecd54e6df8bf5df97ae4567053cb3225`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274569e67c881a677c19e6c191f41a2ac47154ec5053ed091e4c33e6347cc6eb`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4b6a40bcb4cc4d2062a10c6aef8541998d6d36cf3acab5c17d269045be4ba`  
		Last Modified: Sat, 19 Sep 2020 00:06:46 GMT  
		Size: 140.1 MB (140063970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8675018f02a5e0a640222ef7297d4581a6cd3f0a81b53d05be3af657cafc95e1`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2.2-alpine`

```console
$ docker pull plone@sha256:da41dbfa5c88761ef24695f1d1253a87ab262aec06df20ff570826480e3f2f5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:5.2.2-alpine` - linux; 386

```console
$ docker pull plone@sha256:5a1bc721327cd7c21f7ff344c884dcb46d61600d3d55d607777c664b0cc1c7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132819099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eebbca9ecebfd286c5613dfb2d0c529b996af4f86ae08f3a355ef1c09ca8005`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 18:45:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:45:48 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:45:49 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 18:45:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Jul 2020 18:45:24 GMT
ENV PYTHON_VERSION=3.8.5
# Tue, 04 Aug 2020 00:48:58 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 04 Aug 2020 00:48:59 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 20:19:31 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:19:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:19:32 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:19:39 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:19:39 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:50:37 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:50:37 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:50:38 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:50:38 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 00:01:24 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 00:01:25 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 00:01:25 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Sat, 19 Sep 2020 00:01:26 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 00:01:26 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 00:01:26 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 00:01:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 00:01:26 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded523869d7b2121c2a5838365e9f75504b850ecae6661c940242d3456bd53d7`  
		Last Modified: Wed, 03 Jun 2020 19:28:31 GMT  
		Size: 281.4 KB (281373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918a14653b9dca240ca4d776e8e26326fe1fc8913e2f0a5f294e78a47d492527`  
		Last Modified: Tue, 04 Aug 2020 03:33:25 GMT  
		Size: 11.6 MB (11640740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e582739a3cef82c8012814c112b5ce44b8821ed1191d47884ea5f6faf87354a4`  
		Last Modified: Tue, 04 Aug 2020 03:33:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacf94730cf258787add53ecd2b8540d6b6c2e40e873ebca559d196a85144bac`  
		Last Modified: Tue, 08 Sep 2020 21:21:09 GMT  
		Size: 2.1 MB (2119311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1eaa1f2c0627567de9fd8d8a1d4e74d689837959b8677fbd13763de637c30`  
		Last Modified: Sat, 19 Sep 2020 00:03:55 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01733d323fd86c8c1f8d282960f04a14f7e737b16aa0cb0f3c5cb137619a118a`  
		Last Modified: Sat, 19 Sep 2020 00:03:55 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd009a6477d2a964c8572b059ef5555c61aeaa8c81003413be77ec0a15f4c3e`  
		Last Modified: Sat, 19 Sep 2020 00:04:43 GMT  
		Size: 116.0 MB (115979957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98991b6623467c3f68c18b3bd335cadb11cdabe2d4c711b9c66c2042f7fb4c08`  
		Last Modified: Sat, 19 Sep 2020 00:03:55 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.2-alpine` - linux; s390x

```console
$ docker pull plone@sha256:1406a74a9fa6e5a9b1cc63d67aaaf39e401e718750c520edd0129e9383a28beb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (131951362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bba8939e08af189d27667e90bf90ff4996d8b36f9ce149bd3d2810bc095b90c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 19:13:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:13:11 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:13:14 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:13:14 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Jul 2020 18:13:49 GMT
ENV PYTHON_VERSION=3.8.5
# Tue, 04 Aug 2020 00:11:00 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 04 Aug 2020 00:11:01 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 20:18:05 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:18:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:18:05 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:18:10 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:18:10 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:59:24 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:59:24 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:59:25 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:59:25 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 00:05:56 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 00:06:03 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 00:06:04 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Sat, 19 Sep 2020 00:06:04 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 00:06:04 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 00:06:04 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 00:06:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 00:06:05 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b76e1d722a55ff4f330c758d9814944d8ab0c8761b42febad3c13edcbc7d4f`  
		Last Modified: Wed, 03 Jun 2020 22:40:13 GMT  
		Size: 281.4 KB (281387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cf7186a29294842bc660960abd2809bdcd0271e3ae914b83984ef083d00d78`  
		Last Modified: Tue, 04 Aug 2020 01:14:01 GMT  
		Size: 11.4 MB (11441200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6034b2e6ffbdcc74a2853d09090c84865ee9e7e21a33b945dcdfe53636c60bec`  
		Last Modified: Tue, 04 Aug 2020 01:14:00 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffd5d6fa0f52f2db805d45392fb0e6f47b96dfa61e55b17532e19f56ba696d8`  
		Last Modified: Tue, 08 Sep 2020 20:38:18 GMT  
		Size: 2.1 MB (2119320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714f0030dbd3d72437800281a70e48ccd72132e8848a1575ad3a447b6c80441`  
		Last Modified: Sat, 19 Sep 2020 00:07:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b738e0f383738ee67cbec1bb743c128dea90b5727cc38175f00b03e33ad90`  
		Last Modified: Sat, 19 Sep 2020 00:07:52 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19084bd995188fe20396f258b742cbc0ac5ccbb8835941d9409d80f0d3227add`  
		Last Modified: Sat, 19 Sep 2020 00:08:07 GMT  
		Size: 115.5 MB (115537782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cbb51fb1560a971a9f004beb916f71462b9eb4f993ca8ccc6c8926c7a9d798`  
		Last Modified: Sat, 19 Sep 2020 00:07:52 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2.2-python36`

```console
$ docker pull plone@sha256:a2ebdd38d97be21752d8d004bac60ad9d3177bee8bc531b249a54057a3312c96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:5.2.2-python36` - linux; 386

```console
$ docker pull plone@sha256:c009706f351a0758693b4fa34b1c70e928136dcef51c46b5e47ddbc2d4473ad5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.0 MB (189984339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55bd17803580a91d78624be33e46791fa9462b8792e59c0c661a3ff103da5724`
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
# Thu, 10 Sep 2020 13:56:58 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 10 Sep 2020 14:10:19 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 14:10:19 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 14:10:20 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 14:10:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 14:10:20 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 14:10:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 14:10:42 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:46:34 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:46:34 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:46:35 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:46:35 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:50:19 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:50:21 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:50:21 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:50:21 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:50:21 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:50:22 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:50:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:50:22 GMT
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
	-	`sha256:c5811e4a19b8908528b06e1780be3c531a34613499c58be290e7c559261fef52`  
		Last Modified: Thu, 10 Sep 2020 15:19:26 GMT  
		Size: 9.8 MB (9780518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f556bb98a43b664a6d700f148d204a93d94e87f8d76b1d69b9a4fe0aadddde`  
		Last Modified: Thu, 10 Sep 2020 15:19:23 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb36eba2fe2fc3b3f3bee649c64b96d9ec7c8b9fe5baa197b2927282de53a71`  
		Last Modified: Thu, 10 Sep 2020 15:19:24 GMT  
		Size: 2.4 MB (2407802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baeec906bc5130be0d5f38a06c502ffe76466489c72e984f7334a31ec783d6b`  
		Last Modified: Sat, 19 Sep 2020 00:03:13 GMT  
		Size: 3.9 KB (3892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cd72de142ba9330c267027c28a707647a65de4151001a48ca92df916e91bf`  
		Last Modified: Sat, 19 Sep 2020 00:03:13 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c5792fc1bde4723c80c21dd3ec6061e34dcb0aa112d09487d3b586ec04d57e`  
		Last Modified: Sat, 19 Sep 2020 00:03:49 GMT  
		Size: 147.3 MB (147273555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae731a9ad6b30b57c7fab7c10ab1a92719cca1208bb8e9e430f22b00e68357`  
		Last Modified: Sat, 19 Sep 2020 00:03:13 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.2-python36` - linux; s390x

```console
$ docker pull plone@sha256:fbd3b0ab694c3ec04dd1ea737d4c70f6242e057ad9282daa02540d3bb0219f8e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.0 MB (179980261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c914fd66f05d111b83c25da1e3e2069d580b4b7acaa25ebb002233d0964614c8`
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
# Thu, 10 Sep 2020 02:39:23 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 10 Sep 2020 02:43:22 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:43:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:43:23 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:43:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:43:24 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:43:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:43:34 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:54:01 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:54:01 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:54:02 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:54:02 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:59:07 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:59:15 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:59:15 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:59:15 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:59:16 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:59:16 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:59:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:59:16 GMT
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
	-	`sha256:c1297fe51a7a4e624059ae60fb8d5aa6836a977f1afe776fe8bd18884f3f2fbe`  
		Last Modified: Thu, 10 Sep 2020 02:54:06 GMT  
		Size: 9.6 MB (9565972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f25ae5f7b5ef39e22975547a201ce4b9d385c55b4570ad583eafb2e646127a1`  
		Last Modified: Thu, 10 Sep 2020 02:54:05 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee1104daf6f35ff379bb4059fce361ea82be478c1b462da304ba0cf9e1d8548`  
		Last Modified: Thu, 10 Sep 2020 02:54:05 GMT  
		Size: 2.4 MB (2407761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9b0414301d20f3499e7a50dbcd63734d291cd28deaba4e205f9a7771afe131`  
		Last Modified: Sat, 19 Sep 2020 00:07:26 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa20e556f792f8871aa2d142b4f4ef75c8298493f3f81586f3e8e70fa24d3f3`  
		Last Modified: Sat, 19 Sep 2020 00:07:26 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b1c3a8a197509f51971148bce94e710c9c2cf9fa6eb4597ebbe42706e02a20`  
		Last Modified: Sat, 19 Sep 2020 00:07:44 GMT  
		Size: 139.8 MB (139846804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7de228ceaba39ab0c4ce189e67585eb5344670ad4e660fb19bb0b7c4f9c394`  
		Last Modified: Sat, 19 Sep 2020 00:07:26 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2.2-python37`

```console
$ docker pull plone@sha256:1d0c0680b18a1cdbd245c30a2f98994cdbcd885f6f1a58c321728ec784f61705
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:5.2.2-python37` - linux; 386

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

### `plone:5.2.2-python37` - linux; s390x

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

## `plone:5.2.2-python38`

```console
$ docker pull plone@sha256:df29336b72bd033353b7ca4d4f5f84e900b9abdf1dae32c45ba007eca9832a01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:5.2.2-python38` - linux; 386

```console
$ docker pull plone@sha256:74dae2a340501d74b181e6f810bcc5987c5100d435af746737c7cd0228deea0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191123328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6446e55c7fa3222601f6ce73289c88370dc91240430988053f72b10cecd98b4`
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
# Thu, 10 Sep 2020 12:08:17 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 12:37:25 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 12:50:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 12:50:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 12:50:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 12:50:46 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:38:43 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:38:44 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:38:44 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:38:45 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:42:19 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:42:20 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:42:20 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:42:20 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:42:20 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:42:21 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:42:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:42:21 GMT
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
	-	`sha256:9f8d61ae8767c42662c4758765a4389aafccb33e94098c128d01e1436856e52a`  
		Last Modified: Thu, 10 Sep 2020 15:18:10 GMT  
		Size: 10.5 MB (10532513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fa521131d6f14a06ff5a2ba860f47bc766c993ceeacd79a375a2f8aaf1b970`  
		Last Modified: Thu, 10 Sep 2020 15:18:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b31a66bd5005cb79acf880a9bd8e2446aaa63a0e6a12ca44b136526373f7a6f`  
		Last Modified: Thu, 10 Sep 2020 15:18:06 GMT  
		Size: 2.4 MB (2407674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549278a7ff3477d1945b1c6c146a7886ea07a6e80eef07fab39ab361547ce5`  
		Last Modified: Sat, 19 Sep 2020 00:01:42 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921c0542d2620f8af6980da808c1cb6275509da47bcd7b7d17dcf0b53537c9b`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a986571b35c520ca4a2ac4d08cd48b1c84845ca0481766a1701911d257c9fe60`  
		Last Modified: Sat, 19 Sep 2020 00:02:17 GMT  
		Size: 147.7 MB (147660673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649957d7f083af5b1197f2a13e28fefffb9d9e28e07c525e8907479caf613aa`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.2-python38` - linux; s390x

```console
$ docker pull plone@sha256:2d15e6aa00ff378d2b1c5ea04fca06fce7564ddd991740a237282575c440a1b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180905670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6cc06ff3ca729bed0d018430778a47ff947f360d63b0e54044544f456f417f0`
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
# Thu, 10 Sep 2020 02:08:45 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 02:18:52 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 02:23:40 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:23:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:23:42 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:23:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:23:51 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:43:00 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:43:00 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:43:01 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:43:01 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:48:14 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:48:22 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:48:22 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:48:22 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:48:23 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:48:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:48:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:48:23 GMT
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
	-	`sha256:b7a30ebb749e95a6400495190e32c5b98f37145cc1741244dd3975f759240137`  
		Last Modified: Thu, 10 Sep 2020 02:53:24 GMT  
		Size: 10.3 MB (10274354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9331aa7a0a92e572dee8bf61940f31b2a95c5096898cb20f1592c6e7149db9`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465df3edf63ab70b456383487b281eec77a1064cc829206ac8fd4a9a5b77e0a2`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 2.4 MB (2407622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46fa9d8ec0f2f24706bd965bfcf0afdecd54e6df8bf5df97ae4567053cb3225`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274569e67c881a677c19e6c191f41a2ac47154ec5053ed091e4c33e6347cc6eb`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4b6a40bcb4cc4d2062a10c6aef8541998d6d36cf3acab5c17d269045be4ba`  
		Last Modified: Sat, 19 Sep 2020 00:06:46 GMT  
		Size: 140.1 MB (140063970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8675018f02a5e0a640222ef7297d4581a6cd3f0a81b53d05be3af657cafc95e1`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2-alpine`

```console
$ docker pull plone@sha256:b89e51df688bf3daa67443a35e78b7cecd7c59d56d5ea1da009804bbe668b296
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `plone:5.2-alpine` - linux; amd64

```console
$ docker pull plone@sha256:c788f9a14c643721f3787afba98489fbd2f49e58a8cee87658dbfcac4affd7fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141391142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e056171b31cd3fa10da6a9bb64ae9c45a6b8201571432a29a4823b71e97358`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:48:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:36:53 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:36:54 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:51:35 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 18 Aug 2020 03:55:10 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 18 Aug 2020 04:03:54 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 18 Aug 2020 04:03:56 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 20:34:03 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:34:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:34:03 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:34:14 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:34:14 GMT
CMD ["python3"]
# Wed, 09 Sep 2020 01:23:38 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 09 Sep 2020 01:23:38 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 09 Sep 2020 01:23:39 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 09 Sep 2020 01:23:39 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 09 Sep 2020 01:32:39 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 09 Sep 2020 01:32:40 GMT
VOLUME [/data]
# Wed, 09 Sep 2020 01:32:40 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Wed, 09 Sep 2020 01:32:40 GMT
EXPOSE 8080
# Wed, 09 Sep 2020 01:32:41 GMT
WORKDIR /plone/instance
# Wed, 09 Sep 2020 01:32:41 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 09 Sep 2020 01:32:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Sep 2020 01:32:41 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b3adc4ff6ffb76ae233f0a92177205845aaf3e9a39e0f96405dabd1423edc9`  
		Last Modified: Wed, 03 Jun 2020 20:14:46 GMT  
		Size: 280.8 KB (280840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db9de03f49990c0ad8d9e2b3bdcbed147dae39c2c6434029bf3cce610f244e2`  
		Last Modified: Tue, 18 Aug 2020 07:53:31 GMT  
		Size: 11.1 MB (11099566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd38a04a61f4179d0fcf8a931a569a515ea435e61865341a9d8aa96d8115d006`  
		Last Modified: Tue, 18 Aug 2020 07:53:29 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3838385f133785631b680aa48443a64e140452a4aacc6ad7319bf9c38f88a0`  
		Last Modified: Wed, 09 Sep 2020 00:16:41 GMT  
		Size: 2.1 MB (2119310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83bc062a1d54fbdfb69b3b7e297afdc0dd7f6bf330607abf8c0ba2e58bb575a`  
		Last Modified: Wed, 09 Sep 2020 01:33:30 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3165309979eec98cddfa51cdd8a69e97a2992a04c44b140ea94928f9abf05e59`  
		Last Modified: Wed, 09 Sep 2020 01:33:29 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f2e75568df5ff44b8f8fcb0b9ac3c0ccb18cbafed035ba2e42e1c29821767f`  
		Last Modified: Wed, 09 Sep 2020 01:33:52 GMT  
		Size: 125.1 MB (125088464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247e4fbbce4d30b9fed96e2ab28917d456b45c704ebcf2d229dbacd8073417f`  
		Last Modified: Wed, 09 Sep 2020 01:33:30 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:b945d50a8d39dd46f3174106c2a4f1c056444c0bf9bf3acbe5f14800eb779830
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140564978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d32c3fd2ed6235cf81077e31d187119ec000dd23c3311177842ebb70c6c2091`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 18:59:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:59:56 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:59:59 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:20:17 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 18 Aug 2020 03:51:14 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 18 Aug 2020 04:07:07 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 18 Aug 2020 04:07:11 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 21:20:25 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 21:20:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 21:20:44 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 21:21:36 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 21:21:45 GMT
CMD ["python3"]
# Tue, 08 Sep 2020 22:30:25 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Tue, 08 Sep 2020 22:30:30 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Tue, 08 Sep 2020 22:30:58 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Tue, 08 Sep 2020 22:31:11 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Tue, 08 Sep 2020 22:51:44 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Tue, 08 Sep 2020 22:51:57 GMT
VOLUME [/data]
# Tue, 08 Sep 2020 22:51:59 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Tue, 08 Sep 2020 22:52:00 GMT
EXPOSE 8080
# Tue, 08 Sep 2020 22:52:01 GMT
WORKDIR /plone/instance
# Tue, 08 Sep 2020 22:52:03 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Tue, 08 Sep 2020 22:52:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Sep 2020 22:52:06 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba84132d8cf30d261b7b1e4e503e67af8ea432e7f530a830161cc1b1bd53e82`  
		Last Modified: Wed, 03 Jun 2020 19:55:42 GMT  
		Size: 281.0 KB (281040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4c50c433d35c45efb946f9c323c99a91c21a9b8f9e386d4a33a33f8070af70`  
		Last Modified: Tue, 18 Aug 2020 04:43:43 GMT  
		Size: 10.8 MB (10754912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e74ed1e7879f5e938736f55e8c7e86f3873f71f5947354a0abf4a15a93461a`  
		Last Modified: Tue, 18 Aug 2020 04:43:39 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13de131ee1b5e933c989f2d300870b32f775152d55e375044682826086d044c0`  
		Last Modified: Tue, 08 Sep 2020 21:51:55 GMT  
		Size: 2.1 MB (2119572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f3f9a9febef519dd65bbc7032abfe4d2abaa9dac2f568527f5182fc18c6f5c`  
		Last Modified: Tue, 08 Sep 2020 22:52:15 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251d05fb68e7c38c3e6918a9c9eb1c835caee3b26ea48c7112ef98cf731e0f7b`  
		Last Modified: Tue, 08 Sep 2020 22:52:15 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00676cf88f7bfd7b68e2179094c6c4f7cf465bc8cd439186fd0ff49c5c3b83ae`  
		Last Modified: Tue, 08 Sep 2020 22:54:00 GMT  
		Size: 124.8 MB (124800681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a3f26e30d95abe1406ce51a2e7d74b59d309527b6fd6533435bc63c79cefe9`  
		Last Modified: Tue, 08 Sep 2020 22:52:15 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:03af3a948c891a0e82a3f9fc2126e31fb8b8d8704e1d1df4ba49f7840fee467a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141200830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5475cab3bc01cb21f1736b9275655c956dc874215fbadac47b7a1f26f92ba3f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:35:35 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:57:57 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:58:00 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:14:44 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 18 Aug 2020 04:32:35 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 18 Aug 2020 04:46:24 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 18 Aug 2020 04:46:26 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 21:48:18 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 21:48:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 21:48:35 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 21:49:00 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 21:49:03 GMT
CMD ["python3"]
# Wed, 09 Sep 2020 00:12:23 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 09 Sep 2020 00:12:24 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 09 Sep 2020 00:12:26 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 09 Sep 2020 00:12:26 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 09 Sep 2020 00:30:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 09 Sep 2020 00:30:55 GMT
VOLUME [/data]
# Wed, 09 Sep 2020 00:30:56 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Wed, 09 Sep 2020 00:30:57 GMT
EXPOSE 8080
# Wed, 09 Sep 2020 00:30:58 GMT
WORKDIR /plone/instance
# Wed, 09 Sep 2020 00:30:58 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 09 Sep 2020 00:30:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Sep 2020 00:31:00 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d489d24c26399308b276dfa175c049e531d2686fb99e250ad3ede210fd01e9e`  
		Last Modified: Wed, 03 Jun 2020 19:46:54 GMT  
		Size: 281.3 KB (281267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b544f7dc429981fa9ee341d8c569955e5f5d86e52f2b9fe1f1836becff40c2`  
		Last Modified: Tue, 18 Aug 2020 05:53:54 GMT  
		Size: 11.2 MB (11232298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01499c5624ba20bf921e0849806a106eb7f28b5700f53b21bc54213b05b2374`  
		Last Modified: Tue, 18 Aug 2020 05:53:51 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29795334e8c6c0a67c138e66172c6c16143e3e5ec2a5ee6a9b0f1a7e2f4e58ef`  
		Last Modified: Tue, 08 Sep 2020 22:54:12 GMT  
		Size: 2.1 MB (2119543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06c6a5907fe96d854e304bf6a5d2bb34c10a328f1f8567519196fa2e33e276`  
		Last Modified: Wed, 09 Sep 2020 00:32:16 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea0e54505d6010b2694baa41866abe38ac8118de0208c30c3f9a0a3ee62901b`  
		Last Modified: Wed, 09 Sep 2020 00:32:17 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdc9f324eac5ca3df1c1e70cf850605613db00f3d3f57e3960ee793b55be76d`  
		Last Modified: Wed, 09 Sep 2020 00:32:54 GMT  
		Size: 124.9 MB (124854274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8af7e8431b4fc913663a083b5e8c729ba38104b46162f0b1127a2f6ace1d0a`  
		Last Modified: Wed, 09 Sep 2020 00:32:17 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; 386

```console
$ docker pull plone@sha256:5a1bc721327cd7c21f7ff344c884dcb46d61600d3d55d607777c664b0cc1c7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132819099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eebbca9ecebfd286c5613dfb2d0c529b996af4f86ae08f3a355ef1c09ca8005`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 18:45:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:45:48 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:45:49 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 18:45:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Jul 2020 18:45:24 GMT
ENV PYTHON_VERSION=3.8.5
# Tue, 04 Aug 2020 00:48:58 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 04 Aug 2020 00:48:59 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 20:19:31 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:19:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:19:32 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:19:39 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:19:39 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:50:37 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:50:37 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:50:38 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:50:38 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 00:01:24 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 00:01:25 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 00:01:25 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Sat, 19 Sep 2020 00:01:26 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 00:01:26 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 00:01:26 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 00:01:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 00:01:26 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded523869d7b2121c2a5838365e9f75504b850ecae6661c940242d3456bd53d7`  
		Last Modified: Wed, 03 Jun 2020 19:28:31 GMT  
		Size: 281.4 KB (281373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918a14653b9dca240ca4d776e8e26326fe1fc8913e2f0a5f294e78a47d492527`  
		Last Modified: Tue, 04 Aug 2020 03:33:25 GMT  
		Size: 11.6 MB (11640740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e582739a3cef82c8012814c112b5ce44b8821ed1191d47884ea5f6faf87354a4`  
		Last Modified: Tue, 04 Aug 2020 03:33:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacf94730cf258787add53ecd2b8540d6b6c2e40e873ebca559d196a85144bac`  
		Last Modified: Tue, 08 Sep 2020 21:21:09 GMT  
		Size: 2.1 MB (2119311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1eaa1f2c0627567de9fd8d8a1d4e74d689837959b8677fbd13763de637c30`  
		Last Modified: Sat, 19 Sep 2020 00:03:55 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01733d323fd86c8c1f8d282960f04a14f7e737b16aa0cb0f3c5cb137619a118a`  
		Last Modified: Sat, 19 Sep 2020 00:03:55 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd009a6477d2a964c8572b059ef5555c61aeaa8c81003413be77ec0a15f4c3e`  
		Last Modified: Sat, 19 Sep 2020 00:04:43 GMT  
		Size: 116.0 MB (115979957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98991b6623467c3f68c18b3bd335cadb11cdabe2d4c711b9c66c2042f7fb4c08`  
		Last Modified: Sat, 19 Sep 2020 00:03:55 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:c7928333e944658a6a74bea1775fbb2cfd32d9a9af29f1aa513b637dc39b5f29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142404280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bebe4df1eeb07427610e2db3f85897b4cea48a75c7b008c40781623b6740957`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 19:35:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:35:58 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:36:09 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:54:46 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 18 Aug 2020 03:55:19 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 18 Aug 2020 04:07:24 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 18 Aug 2020 04:07:37 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 21:43:31 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 21:43:37 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 21:43:45 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 21:44:28 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 21:44:31 GMT
CMD ["python3"]
# Wed, 09 Sep 2020 00:17:03 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 09 Sep 2020 00:17:13 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 09 Sep 2020 00:17:34 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 09 Sep 2020 00:17:36 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 09 Sep 2020 00:35:27 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 09 Sep 2020 00:35:36 GMT
VOLUME [/data]
# Wed, 09 Sep 2020 00:35:39 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Wed, 09 Sep 2020 00:35:45 GMT
EXPOSE 8080
# Wed, 09 Sep 2020 00:35:53 GMT
WORKDIR /plone/instance
# Wed, 09 Sep 2020 00:35:57 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 09 Sep 2020 00:36:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Sep 2020 00:36:15 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c9759563702d3bc987f9dad6559da6de6fa68093dc6b51fb097c1c4abc1876`  
		Last Modified: Wed, 03 Jun 2020 20:26:29 GMT  
		Size: 285.0 KB (285014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235ded95fa3dbd96f689d2bb2cd7f573ba7186db2b8b754d7fd3683f44b91c65`  
		Last Modified: Tue, 18 Aug 2020 05:08:05 GMT  
		Size: 11.8 MB (11823450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f8a3859d9618409e9e46f9bd51ccaa75bd591c1e28e013fa5a84ca2c7725cf`  
		Last Modified: Tue, 18 Aug 2020 05:08:03 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc20dbfb21bc0e17844f123bc4e33982f6fd90490928fd18b55a09c95f439db0`  
		Last Modified: Tue, 08 Sep 2020 22:51:45 GMT  
		Size: 2.1 MB (2119592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a19d1953fe926f318261fcc0d8495412d1515db44893ea937d2c5bf3563e6b6`  
		Last Modified: Wed, 09 Sep 2020 00:36:47 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188ae4b204f9df81a1a311f37200cbe1f6b5d78e73b439a679211ba447ec2ee4`  
		Last Modified: Wed, 09 Sep 2020 00:36:47 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4704e8af23153091364bd81a0b95376da26ba22b51ea3c99137e46e80b6d721b`  
		Last Modified: Wed, 09 Sep 2020 00:37:18 GMT  
		Size: 125.4 MB (125365539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bc94ba37e70d07d6e730b9a881b73f62484a48bf2b78270ab111467a1f743`  
		Last Modified: Wed, 09 Sep 2020 00:36:47 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; s390x

```console
$ docker pull plone@sha256:1406a74a9fa6e5a9b1cc63d67aaaf39e401e718750c520edd0129e9383a28beb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (131951362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bba8939e08af189d27667e90bf90ff4996d8b36f9ce149bd3d2810bc095b90c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 19:13:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:13:11 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:13:14 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:13:14 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Jul 2020 18:13:49 GMT
ENV PYTHON_VERSION=3.8.5
# Tue, 04 Aug 2020 00:11:00 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 04 Aug 2020 00:11:01 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 20:18:05 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:18:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:18:05 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:18:10 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:18:10 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:59:24 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:59:24 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:59:25 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:59:25 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 00:05:56 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 00:06:03 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 00:06:04 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Sat, 19 Sep 2020 00:06:04 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 00:06:04 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 00:06:04 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 00:06:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 00:06:05 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b76e1d722a55ff4f330c758d9814944d8ab0c8761b42febad3c13edcbc7d4f`  
		Last Modified: Wed, 03 Jun 2020 22:40:13 GMT  
		Size: 281.4 KB (281387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cf7186a29294842bc660960abd2809bdcd0271e3ae914b83984ef083d00d78`  
		Last Modified: Tue, 04 Aug 2020 01:14:01 GMT  
		Size: 11.4 MB (11441200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6034b2e6ffbdcc74a2853d09090c84865ee9e7e21a33b945dcdfe53636c60bec`  
		Last Modified: Tue, 04 Aug 2020 01:14:00 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffd5d6fa0f52f2db805d45392fb0e6f47b96dfa61e55b17532e19f56ba696d8`  
		Last Modified: Tue, 08 Sep 2020 20:38:18 GMT  
		Size: 2.1 MB (2119320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714f0030dbd3d72437800281a70e48ccd72132e8848a1575ad3a447b6c80441`  
		Last Modified: Sat, 19 Sep 2020 00:07:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b738e0f383738ee67cbec1bb743c128dea90b5727cc38175f00b03e33ad90`  
		Last Modified: Sat, 19 Sep 2020 00:07:52 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19084bd995188fe20396f258b742cbc0ac5ccbb8835941d9409d80f0d3227add`  
		Last Modified: Sat, 19 Sep 2020 00:08:07 GMT  
		Size: 115.5 MB (115537782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cbb51fb1560a971a9f004beb916f71462b9eb4f993ca8ccc6c8926c7a9d798`  
		Last Modified: Sat, 19 Sep 2020 00:07:52 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2-python36`

```console
$ docker pull plone@sha256:a2ebdd38d97be21752d8d004bac60ad9d3177bee8bc531b249a54057a3312c96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:5.2-python36` - linux; 386

```console
$ docker pull plone@sha256:c009706f351a0758693b4fa34b1c70e928136dcef51c46b5e47ddbc2d4473ad5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.0 MB (189984339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55bd17803580a91d78624be33e46791fa9462b8792e59c0c661a3ff103da5724`
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
# Thu, 10 Sep 2020 13:56:58 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 10 Sep 2020 14:10:19 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 14:10:19 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 14:10:20 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 14:10:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 14:10:20 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 14:10:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 14:10:42 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:46:34 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:46:34 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:46:35 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:46:35 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:50:19 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:50:21 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:50:21 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:50:21 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:50:21 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:50:22 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:50:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:50:22 GMT
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
	-	`sha256:c5811e4a19b8908528b06e1780be3c531a34613499c58be290e7c559261fef52`  
		Last Modified: Thu, 10 Sep 2020 15:19:26 GMT  
		Size: 9.8 MB (9780518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f556bb98a43b664a6d700f148d204a93d94e87f8d76b1d69b9a4fe0aadddde`  
		Last Modified: Thu, 10 Sep 2020 15:19:23 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb36eba2fe2fc3b3f3bee649c64b96d9ec7c8b9fe5baa197b2927282de53a71`  
		Last Modified: Thu, 10 Sep 2020 15:19:24 GMT  
		Size: 2.4 MB (2407802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baeec906bc5130be0d5f38a06c502ffe76466489c72e984f7334a31ec783d6b`  
		Last Modified: Sat, 19 Sep 2020 00:03:13 GMT  
		Size: 3.9 KB (3892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cd72de142ba9330c267027c28a707647a65de4151001a48ca92df916e91bf`  
		Last Modified: Sat, 19 Sep 2020 00:03:13 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c5792fc1bde4723c80c21dd3ec6061e34dcb0aa112d09487d3b586ec04d57e`  
		Last Modified: Sat, 19 Sep 2020 00:03:49 GMT  
		Size: 147.3 MB (147273555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae731a9ad6b30b57c7fab7c10ab1a92719cca1208bb8e9e430f22b00e68357`  
		Last Modified: Sat, 19 Sep 2020 00:03:13 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-python36` - linux; s390x

```console
$ docker pull plone@sha256:fbd3b0ab694c3ec04dd1ea737d4c70f6242e057ad9282daa02540d3bb0219f8e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.0 MB (179980261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c914fd66f05d111b83c25da1e3e2069d580b4b7acaa25ebb002233d0964614c8`
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
# Thu, 10 Sep 2020 02:39:23 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 10 Sep 2020 02:43:22 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:43:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:43:23 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:43:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:43:24 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:43:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:43:34 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:54:01 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:54:01 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:54:02 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:54:02 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:59:07 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:59:15 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:59:15 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:59:15 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:59:16 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:59:16 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:59:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:59:16 GMT
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
	-	`sha256:c1297fe51a7a4e624059ae60fb8d5aa6836a977f1afe776fe8bd18884f3f2fbe`  
		Last Modified: Thu, 10 Sep 2020 02:54:06 GMT  
		Size: 9.6 MB (9565972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f25ae5f7b5ef39e22975547a201ce4b9d385c55b4570ad583eafb2e646127a1`  
		Last Modified: Thu, 10 Sep 2020 02:54:05 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee1104daf6f35ff379bb4059fce361ea82be478c1b462da304ba0cf9e1d8548`  
		Last Modified: Thu, 10 Sep 2020 02:54:05 GMT  
		Size: 2.4 MB (2407761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9b0414301d20f3499e7a50dbcd63734d291cd28deaba4e205f9a7771afe131`  
		Last Modified: Sat, 19 Sep 2020 00:07:26 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa20e556f792f8871aa2d142b4f4ef75c8298493f3f81586f3e8e70fa24d3f3`  
		Last Modified: Sat, 19 Sep 2020 00:07:26 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b1c3a8a197509f51971148bce94e710c9c2cf9fa6eb4597ebbe42706e02a20`  
		Last Modified: Sat, 19 Sep 2020 00:07:44 GMT  
		Size: 139.8 MB (139846804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7de228ceaba39ab0c4ce189e67585eb5344670ad4e660fb19bb0b7c4f9c394`  
		Last Modified: Sat, 19 Sep 2020 00:07:26 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2-python37`

```console
$ docker pull plone@sha256:1d0c0680b18a1cdbd245c30a2f98994cdbcd885f6f1a58c321728ec784f61705
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:5.2-python37` - linux; 386

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

### `plone:5.2-python37` - linux; s390x

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

## `plone:5.2-python38`

```console
$ docker pull plone@sha256:df29336b72bd033353b7ca4d4f5f84e900b9abdf1dae32c45ba007eca9832a01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:5.2-python38` - linux; 386

```console
$ docker pull plone@sha256:74dae2a340501d74b181e6f810bcc5987c5100d435af746737c7cd0228deea0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191123328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6446e55c7fa3222601f6ce73289c88370dc91240430988053f72b10cecd98b4`
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
# Thu, 10 Sep 2020 12:08:17 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 12:37:25 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 12:50:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 12:50:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 12:50:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 12:50:46 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:38:43 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:38:44 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:38:44 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:38:45 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:42:19 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:42:20 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:42:20 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:42:20 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:42:20 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:42:21 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:42:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:42:21 GMT
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
	-	`sha256:9f8d61ae8767c42662c4758765a4389aafccb33e94098c128d01e1436856e52a`  
		Last Modified: Thu, 10 Sep 2020 15:18:10 GMT  
		Size: 10.5 MB (10532513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fa521131d6f14a06ff5a2ba860f47bc766c993ceeacd79a375a2f8aaf1b970`  
		Last Modified: Thu, 10 Sep 2020 15:18:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b31a66bd5005cb79acf880a9bd8e2446aaa63a0e6a12ca44b136526373f7a6f`  
		Last Modified: Thu, 10 Sep 2020 15:18:06 GMT  
		Size: 2.4 MB (2407674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549278a7ff3477d1945b1c6c146a7886ea07a6e80eef07fab39ab361547ce5`  
		Last Modified: Sat, 19 Sep 2020 00:01:42 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921c0542d2620f8af6980da808c1cb6275509da47bcd7b7d17dcf0b53537c9b`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a986571b35c520ca4a2ac4d08cd48b1c84845ca0481766a1701911d257c9fe60`  
		Last Modified: Sat, 19 Sep 2020 00:02:17 GMT  
		Size: 147.7 MB (147660673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649957d7f083af5b1197f2a13e28fefffb9d9e28e07c525e8907479caf613aa`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-python38` - linux; s390x

```console
$ docker pull plone@sha256:2d15e6aa00ff378d2b1c5ea04fca06fce7564ddd991740a237282575c440a1b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180905670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6cc06ff3ca729bed0d018430778a47ff947f360d63b0e54044544f456f417f0`
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
# Thu, 10 Sep 2020 02:08:45 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 02:18:52 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 02:23:40 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:23:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:23:42 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:23:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:23:51 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:43:00 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:43:00 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:43:01 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:43:01 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:48:14 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:48:22 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:48:22 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:48:22 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:48:23 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:48:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:48:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:48:23 GMT
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
	-	`sha256:b7a30ebb749e95a6400495190e32c5b98f37145cc1741244dd3975f759240137`  
		Last Modified: Thu, 10 Sep 2020 02:53:24 GMT  
		Size: 10.3 MB (10274354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9331aa7a0a92e572dee8bf61940f31b2a95c5096898cb20f1592c6e7149db9`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465df3edf63ab70b456383487b281eec77a1064cc829206ac8fd4a9a5b77e0a2`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 2.4 MB (2407622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46fa9d8ec0f2f24706bd965bfcf0afdecd54e6df8bf5df97ae4567053cb3225`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274569e67c881a677c19e6c191f41a2ac47154ec5053ed091e4c33e6347cc6eb`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4b6a40bcb4cc4d2062a10c6aef8541998d6d36cf3acab5c17d269045be4ba`  
		Last Modified: Sat, 19 Sep 2020 00:06:46 GMT  
		Size: 140.1 MB (140063970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8675018f02a5e0a640222ef7297d4581a6cd3f0a81b53d05be3af657cafc95e1`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5-alpine`

```console
$ docker pull plone@sha256:b89e51df688bf3daa67443a35e78b7cecd7c59d56d5ea1da009804bbe668b296
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `plone:5-alpine` - linux; amd64

```console
$ docker pull plone@sha256:c788f9a14c643721f3787afba98489fbd2f49e58a8cee87658dbfcac4affd7fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141391142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e056171b31cd3fa10da6a9bb64ae9c45a6b8201571432a29a4823b71e97358`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:48:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:36:53 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:36:54 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:51:35 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 18 Aug 2020 03:55:10 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 18 Aug 2020 04:03:54 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 18 Aug 2020 04:03:56 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 20:34:03 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:34:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:34:03 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:34:14 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:34:14 GMT
CMD ["python3"]
# Wed, 09 Sep 2020 01:23:38 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 09 Sep 2020 01:23:38 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 09 Sep 2020 01:23:39 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 09 Sep 2020 01:23:39 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 09 Sep 2020 01:32:39 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 09 Sep 2020 01:32:40 GMT
VOLUME [/data]
# Wed, 09 Sep 2020 01:32:40 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Wed, 09 Sep 2020 01:32:40 GMT
EXPOSE 8080
# Wed, 09 Sep 2020 01:32:41 GMT
WORKDIR /plone/instance
# Wed, 09 Sep 2020 01:32:41 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 09 Sep 2020 01:32:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Sep 2020 01:32:41 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b3adc4ff6ffb76ae233f0a92177205845aaf3e9a39e0f96405dabd1423edc9`  
		Last Modified: Wed, 03 Jun 2020 20:14:46 GMT  
		Size: 280.8 KB (280840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db9de03f49990c0ad8d9e2b3bdcbed147dae39c2c6434029bf3cce610f244e2`  
		Last Modified: Tue, 18 Aug 2020 07:53:31 GMT  
		Size: 11.1 MB (11099566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd38a04a61f4179d0fcf8a931a569a515ea435e61865341a9d8aa96d8115d006`  
		Last Modified: Tue, 18 Aug 2020 07:53:29 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3838385f133785631b680aa48443a64e140452a4aacc6ad7319bf9c38f88a0`  
		Last Modified: Wed, 09 Sep 2020 00:16:41 GMT  
		Size: 2.1 MB (2119310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83bc062a1d54fbdfb69b3b7e297afdc0dd7f6bf330607abf8c0ba2e58bb575a`  
		Last Modified: Wed, 09 Sep 2020 01:33:30 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3165309979eec98cddfa51cdd8a69e97a2992a04c44b140ea94928f9abf05e59`  
		Last Modified: Wed, 09 Sep 2020 01:33:29 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f2e75568df5ff44b8f8fcb0b9ac3c0ccb18cbafed035ba2e42e1c29821767f`  
		Last Modified: Wed, 09 Sep 2020 01:33:52 GMT  
		Size: 125.1 MB (125088464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247e4fbbce4d30b9fed96e2ab28917d456b45c704ebcf2d229dbacd8073417f`  
		Last Modified: Wed, 09 Sep 2020 01:33:30 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:b945d50a8d39dd46f3174106c2a4f1c056444c0bf9bf3acbe5f14800eb779830
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140564978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d32c3fd2ed6235cf81077e31d187119ec000dd23c3311177842ebb70c6c2091`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 18:59:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:59:56 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:59:59 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:20:17 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 18 Aug 2020 03:51:14 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 18 Aug 2020 04:07:07 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 18 Aug 2020 04:07:11 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 21:20:25 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 21:20:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 21:20:44 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 21:21:36 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 21:21:45 GMT
CMD ["python3"]
# Tue, 08 Sep 2020 22:30:25 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Tue, 08 Sep 2020 22:30:30 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Tue, 08 Sep 2020 22:30:58 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Tue, 08 Sep 2020 22:31:11 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Tue, 08 Sep 2020 22:51:44 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Tue, 08 Sep 2020 22:51:57 GMT
VOLUME [/data]
# Tue, 08 Sep 2020 22:51:59 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Tue, 08 Sep 2020 22:52:00 GMT
EXPOSE 8080
# Tue, 08 Sep 2020 22:52:01 GMT
WORKDIR /plone/instance
# Tue, 08 Sep 2020 22:52:03 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Tue, 08 Sep 2020 22:52:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Sep 2020 22:52:06 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba84132d8cf30d261b7b1e4e503e67af8ea432e7f530a830161cc1b1bd53e82`  
		Last Modified: Wed, 03 Jun 2020 19:55:42 GMT  
		Size: 281.0 KB (281040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4c50c433d35c45efb946f9c323c99a91c21a9b8f9e386d4a33a33f8070af70`  
		Last Modified: Tue, 18 Aug 2020 04:43:43 GMT  
		Size: 10.8 MB (10754912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e74ed1e7879f5e938736f55e8c7e86f3873f71f5947354a0abf4a15a93461a`  
		Last Modified: Tue, 18 Aug 2020 04:43:39 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13de131ee1b5e933c989f2d300870b32f775152d55e375044682826086d044c0`  
		Last Modified: Tue, 08 Sep 2020 21:51:55 GMT  
		Size: 2.1 MB (2119572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f3f9a9febef519dd65bbc7032abfe4d2abaa9dac2f568527f5182fc18c6f5c`  
		Last Modified: Tue, 08 Sep 2020 22:52:15 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251d05fb68e7c38c3e6918a9c9eb1c835caee3b26ea48c7112ef98cf731e0f7b`  
		Last Modified: Tue, 08 Sep 2020 22:52:15 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00676cf88f7bfd7b68e2179094c6c4f7cf465bc8cd439186fd0ff49c5c3b83ae`  
		Last Modified: Tue, 08 Sep 2020 22:54:00 GMT  
		Size: 124.8 MB (124800681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a3f26e30d95abe1406ce51a2e7d74b59d309527b6fd6533435bc63c79cefe9`  
		Last Modified: Tue, 08 Sep 2020 22:52:15 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:03af3a948c891a0e82a3f9fc2126e31fb8b8d8704e1d1df4ba49f7840fee467a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141200830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5475cab3bc01cb21f1736b9275655c956dc874215fbadac47b7a1f26f92ba3f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:35:35 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:57:57 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:58:00 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:14:44 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 18 Aug 2020 04:32:35 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 18 Aug 2020 04:46:24 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 18 Aug 2020 04:46:26 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 21:48:18 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 21:48:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 21:48:35 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 21:49:00 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 21:49:03 GMT
CMD ["python3"]
# Wed, 09 Sep 2020 00:12:23 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 09 Sep 2020 00:12:24 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 09 Sep 2020 00:12:26 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 09 Sep 2020 00:12:26 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 09 Sep 2020 00:30:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 09 Sep 2020 00:30:55 GMT
VOLUME [/data]
# Wed, 09 Sep 2020 00:30:56 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Wed, 09 Sep 2020 00:30:57 GMT
EXPOSE 8080
# Wed, 09 Sep 2020 00:30:58 GMT
WORKDIR /plone/instance
# Wed, 09 Sep 2020 00:30:58 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 09 Sep 2020 00:30:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Sep 2020 00:31:00 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d489d24c26399308b276dfa175c049e531d2686fb99e250ad3ede210fd01e9e`  
		Last Modified: Wed, 03 Jun 2020 19:46:54 GMT  
		Size: 281.3 KB (281267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b544f7dc429981fa9ee341d8c569955e5f5d86e52f2b9fe1f1836becff40c2`  
		Last Modified: Tue, 18 Aug 2020 05:53:54 GMT  
		Size: 11.2 MB (11232298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01499c5624ba20bf921e0849806a106eb7f28b5700f53b21bc54213b05b2374`  
		Last Modified: Tue, 18 Aug 2020 05:53:51 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29795334e8c6c0a67c138e66172c6c16143e3e5ec2a5ee6a9b0f1a7e2f4e58ef`  
		Last Modified: Tue, 08 Sep 2020 22:54:12 GMT  
		Size: 2.1 MB (2119543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06c6a5907fe96d854e304bf6a5d2bb34c10a328f1f8567519196fa2e33e276`  
		Last Modified: Wed, 09 Sep 2020 00:32:16 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea0e54505d6010b2694baa41866abe38ac8118de0208c30c3f9a0a3ee62901b`  
		Last Modified: Wed, 09 Sep 2020 00:32:17 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdc9f324eac5ca3df1c1e70cf850605613db00f3d3f57e3960ee793b55be76d`  
		Last Modified: Wed, 09 Sep 2020 00:32:54 GMT  
		Size: 124.9 MB (124854274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8af7e8431b4fc913663a083b5e8c729ba38104b46162f0b1127a2f6ace1d0a`  
		Last Modified: Wed, 09 Sep 2020 00:32:17 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; 386

```console
$ docker pull plone@sha256:5a1bc721327cd7c21f7ff344c884dcb46d61600d3d55d607777c664b0cc1c7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132819099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eebbca9ecebfd286c5613dfb2d0c529b996af4f86ae08f3a355ef1c09ca8005`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 18:45:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:45:48 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:45:49 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 18:45:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Jul 2020 18:45:24 GMT
ENV PYTHON_VERSION=3.8.5
# Tue, 04 Aug 2020 00:48:58 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 04 Aug 2020 00:48:59 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 20:19:31 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:19:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:19:32 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:19:39 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:19:39 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:50:37 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:50:37 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:50:38 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:50:38 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 00:01:24 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 00:01:25 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 00:01:25 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Sat, 19 Sep 2020 00:01:26 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 00:01:26 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 00:01:26 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 00:01:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 00:01:26 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded523869d7b2121c2a5838365e9f75504b850ecae6661c940242d3456bd53d7`  
		Last Modified: Wed, 03 Jun 2020 19:28:31 GMT  
		Size: 281.4 KB (281373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918a14653b9dca240ca4d776e8e26326fe1fc8913e2f0a5f294e78a47d492527`  
		Last Modified: Tue, 04 Aug 2020 03:33:25 GMT  
		Size: 11.6 MB (11640740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e582739a3cef82c8012814c112b5ce44b8821ed1191d47884ea5f6faf87354a4`  
		Last Modified: Tue, 04 Aug 2020 03:33:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacf94730cf258787add53ecd2b8540d6b6c2e40e873ebca559d196a85144bac`  
		Last Modified: Tue, 08 Sep 2020 21:21:09 GMT  
		Size: 2.1 MB (2119311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1eaa1f2c0627567de9fd8d8a1d4e74d689837959b8677fbd13763de637c30`  
		Last Modified: Sat, 19 Sep 2020 00:03:55 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01733d323fd86c8c1f8d282960f04a14f7e737b16aa0cb0f3c5cb137619a118a`  
		Last Modified: Sat, 19 Sep 2020 00:03:55 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd009a6477d2a964c8572b059ef5555c61aeaa8c81003413be77ec0a15f4c3e`  
		Last Modified: Sat, 19 Sep 2020 00:04:43 GMT  
		Size: 116.0 MB (115979957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98991b6623467c3f68c18b3bd335cadb11cdabe2d4c711b9c66c2042f7fb4c08`  
		Last Modified: Sat, 19 Sep 2020 00:03:55 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:c7928333e944658a6a74bea1775fbb2cfd32d9a9af29f1aa513b637dc39b5f29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142404280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bebe4df1eeb07427610e2db3f85897b4cea48a75c7b008c40781623b6740957`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 19:35:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:35:58 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:36:09 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:54:46 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 18 Aug 2020 03:55:19 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 18 Aug 2020 04:07:24 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 18 Aug 2020 04:07:37 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 21:43:31 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 21:43:37 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 21:43:45 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 21:44:28 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 21:44:31 GMT
CMD ["python3"]
# Wed, 09 Sep 2020 00:17:03 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 09 Sep 2020 00:17:13 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 09 Sep 2020 00:17:34 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 09 Sep 2020 00:17:36 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 09 Sep 2020 00:35:27 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 09 Sep 2020 00:35:36 GMT
VOLUME [/data]
# Wed, 09 Sep 2020 00:35:39 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Wed, 09 Sep 2020 00:35:45 GMT
EXPOSE 8080
# Wed, 09 Sep 2020 00:35:53 GMT
WORKDIR /plone/instance
# Wed, 09 Sep 2020 00:35:57 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 09 Sep 2020 00:36:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Sep 2020 00:36:15 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c9759563702d3bc987f9dad6559da6de6fa68093dc6b51fb097c1c4abc1876`  
		Last Modified: Wed, 03 Jun 2020 20:26:29 GMT  
		Size: 285.0 KB (285014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235ded95fa3dbd96f689d2bb2cd7f573ba7186db2b8b754d7fd3683f44b91c65`  
		Last Modified: Tue, 18 Aug 2020 05:08:05 GMT  
		Size: 11.8 MB (11823450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f8a3859d9618409e9e46f9bd51ccaa75bd591c1e28e013fa5a84ca2c7725cf`  
		Last Modified: Tue, 18 Aug 2020 05:08:03 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc20dbfb21bc0e17844f123bc4e33982f6fd90490928fd18b55a09c95f439db0`  
		Last Modified: Tue, 08 Sep 2020 22:51:45 GMT  
		Size: 2.1 MB (2119592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a19d1953fe926f318261fcc0d8495412d1515db44893ea937d2c5bf3563e6b6`  
		Last Modified: Wed, 09 Sep 2020 00:36:47 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188ae4b204f9df81a1a311f37200cbe1f6b5d78e73b439a679211ba447ec2ee4`  
		Last Modified: Wed, 09 Sep 2020 00:36:47 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4704e8af23153091364bd81a0b95376da26ba22b51ea3c99137e46e80b6d721b`  
		Last Modified: Wed, 09 Sep 2020 00:37:18 GMT  
		Size: 125.4 MB (125365539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bc94ba37e70d07d6e730b9a881b73f62484a48bf2b78270ab111467a1f743`  
		Last Modified: Wed, 09 Sep 2020 00:36:47 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; s390x

```console
$ docker pull plone@sha256:1406a74a9fa6e5a9b1cc63d67aaaf39e401e718750c520edd0129e9383a28beb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (131951362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bba8939e08af189d27667e90bf90ff4996d8b36f9ce149bd3d2810bc095b90c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 19:13:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:13:11 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:13:14 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:13:14 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Jul 2020 18:13:49 GMT
ENV PYTHON_VERSION=3.8.5
# Tue, 04 Aug 2020 00:11:00 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 04 Aug 2020 00:11:01 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 20:18:05 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:18:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:18:05 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:18:10 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:18:10 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:59:24 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:59:24 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:59:25 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:59:25 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 00:05:56 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 00:06:03 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 00:06:04 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Sat, 19 Sep 2020 00:06:04 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 00:06:04 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 00:06:04 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 00:06:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 00:06:05 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b76e1d722a55ff4f330c758d9814944d8ab0c8761b42febad3c13edcbc7d4f`  
		Last Modified: Wed, 03 Jun 2020 22:40:13 GMT  
		Size: 281.4 KB (281387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cf7186a29294842bc660960abd2809bdcd0271e3ae914b83984ef083d00d78`  
		Last Modified: Tue, 04 Aug 2020 01:14:01 GMT  
		Size: 11.4 MB (11441200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6034b2e6ffbdcc74a2853d09090c84865ee9e7e21a33b945dcdfe53636c60bec`  
		Last Modified: Tue, 04 Aug 2020 01:14:00 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffd5d6fa0f52f2db805d45392fb0e6f47b96dfa61e55b17532e19f56ba696d8`  
		Last Modified: Tue, 08 Sep 2020 20:38:18 GMT  
		Size: 2.1 MB (2119320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714f0030dbd3d72437800281a70e48ccd72132e8848a1575ad3a447b6c80441`  
		Last Modified: Sat, 19 Sep 2020 00:07:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b738e0f383738ee67cbec1bb743c128dea90b5727cc38175f00b03e33ad90`  
		Last Modified: Sat, 19 Sep 2020 00:07:52 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19084bd995188fe20396f258b742cbc0ac5ccbb8835941d9409d80f0d3227add`  
		Last Modified: Sat, 19 Sep 2020 00:08:07 GMT  
		Size: 115.5 MB (115537782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cbb51fb1560a971a9f004beb916f71462b9eb4f993ca8ccc6c8926c7a9d798`  
		Last Modified: Sat, 19 Sep 2020 00:07:52 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5-python36`

```console
$ docker pull plone@sha256:a2ebdd38d97be21752d8d004bac60ad9d3177bee8bc531b249a54057a3312c96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:5-python36` - linux; 386

```console
$ docker pull plone@sha256:c009706f351a0758693b4fa34b1c70e928136dcef51c46b5e47ddbc2d4473ad5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.0 MB (189984339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55bd17803580a91d78624be33e46791fa9462b8792e59c0c661a3ff103da5724`
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
# Thu, 10 Sep 2020 13:56:58 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 10 Sep 2020 14:10:19 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 14:10:19 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 14:10:20 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 14:10:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 14:10:20 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 14:10:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 14:10:42 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:46:34 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:46:34 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:46:35 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:46:35 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:50:19 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:50:21 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:50:21 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:50:21 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:50:21 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:50:22 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:50:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:50:22 GMT
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
	-	`sha256:c5811e4a19b8908528b06e1780be3c531a34613499c58be290e7c559261fef52`  
		Last Modified: Thu, 10 Sep 2020 15:19:26 GMT  
		Size: 9.8 MB (9780518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f556bb98a43b664a6d700f148d204a93d94e87f8d76b1d69b9a4fe0aadddde`  
		Last Modified: Thu, 10 Sep 2020 15:19:23 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb36eba2fe2fc3b3f3bee649c64b96d9ec7c8b9fe5baa197b2927282de53a71`  
		Last Modified: Thu, 10 Sep 2020 15:19:24 GMT  
		Size: 2.4 MB (2407802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baeec906bc5130be0d5f38a06c502ffe76466489c72e984f7334a31ec783d6b`  
		Last Modified: Sat, 19 Sep 2020 00:03:13 GMT  
		Size: 3.9 KB (3892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cd72de142ba9330c267027c28a707647a65de4151001a48ca92df916e91bf`  
		Last Modified: Sat, 19 Sep 2020 00:03:13 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c5792fc1bde4723c80c21dd3ec6061e34dcb0aa112d09487d3b586ec04d57e`  
		Last Modified: Sat, 19 Sep 2020 00:03:49 GMT  
		Size: 147.3 MB (147273555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae731a9ad6b30b57c7fab7c10ab1a92719cca1208bb8e9e430f22b00e68357`  
		Last Modified: Sat, 19 Sep 2020 00:03:13 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-python36` - linux; s390x

```console
$ docker pull plone@sha256:fbd3b0ab694c3ec04dd1ea737d4c70f6242e057ad9282daa02540d3bb0219f8e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.0 MB (179980261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c914fd66f05d111b83c25da1e3e2069d580b4b7acaa25ebb002233d0964614c8`
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
# Thu, 10 Sep 2020 02:39:23 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 10 Sep 2020 02:43:22 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:43:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:43:23 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:43:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:43:24 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:43:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:43:34 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:54:01 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:54:01 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:54:02 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:54:02 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:59:07 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:59:15 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:59:15 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:59:15 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:59:16 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:59:16 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:59:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:59:16 GMT
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
	-	`sha256:c1297fe51a7a4e624059ae60fb8d5aa6836a977f1afe776fe8bd18884f3f2fbe`  
		Last Modified: Thu, 10 Sep 2020 02:54:06 GMT  
		Size: 9.6 MB (9565972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f25ae5f7b5ef39e22975547a201ce4b9d385c55b4570ad583eafb2e646127a1`  
		Last Modified: Thu, 10 Sep 2020 02:54:05 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee1104daf6f35ff379bb4059fce361ea82be478c1b462da304ba0cf9e1d8548`  
		Last Modified: Thu, 10 Sep 2020 02:54:05 GMT  
		Size: 2.4 MB (2407761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9b0414301d20f3499e7a50dbcd63734d291cd28deaba4e205f9a7771afe131`  
		Last Modified: Sat, 19 Sep 2020 00:07:26 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa20e556f792f8871aa2d142b4f4ef75c8298493f3f81586f3e8e70fa24d3f3`  
		Last Modified: Sat, 19 Sep 2020 00:07:26 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b1c3a8a197509f51971148bce94e710c9c2cf9fa6eb4597ebbe42706e02a20`  
		Last Modified: Sat, 19 Sep 2020 00:07:44 GMT  
		Size: 139.8 MB (139846804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7de228ceaba39ab0c4ce189e67585eb5344670ad4e660fb19bb0b7c4f9c394`  
		Last Modified: Sat, 19 Sep 2020 00:07:26 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5-python37`

```console
$ docker pull plone@sha256:1d0c0680b18a1cdbd245c30a2f98994cdbcd885f6f1a58c321728ec784f61705
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:5-python37` - linux; 386

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

### `plone:5-python37` - linux; s390x

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

## `plone:5-python38`

```console
$ docker pull plone@sha256:df29336b72bd033353b7ca4d4f5f84e900b9abdf1dae32c45ba007eca9832a01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:5-python38` - linux; 386

```console
$ docker pull plone@sha256:74dae2a340501d74b181e6f810bcc5987c5100d435af746737c7cd0228deea0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191123328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6446e55c7fa3222601f6ce73289c88370dc91240430988053f72b10cecd98b4`
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
# Thu, 10 Sep 2020 12:08:17 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 12:37:25 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 12:50:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 12:50:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 12:50:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 12:50:46 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:38:43 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:38:44 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:38:44 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:38:45 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:42:19 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:42:20 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:42:20 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:42:20 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:42:20 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:42:21 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:42:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:42:21 GMT
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
	-	`sha256:9f8d61ae8767c42662c4758765a4389aafccb33e94098c128d01e1436856e52a`  
		Last Modified: Thu, 10 Sep 2020 15:18:10 GMT  
		Size: 10.5 MB (10532513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fa521131d6f14a06ff5a2ba860f47bc766c993ceeacd79a375a2f8aaf1b970`  
		Last Modified: Thu, 10 Sep 2020 15:18:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b31a66bd5005cb79acf880a9bd8e2446aaa63a0e6a12ca44b136526373f7a6f`  
		Last Modified: Thu, 10 Sep 2020 15:18:06 GMT  
		Size: 2.4 MB (2407674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549278a7ff3477d1945b1c6c146a7886ea07a6e80eef07fab39ab361547ce5`  
		Last Modified: Sat, 19 Sep 2020 00:01:42 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921c0542d2620f8af6980da808c1cb6275509da47bcd7b7d17dcf0b53537c9b`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a986571b35c520ca4a2ac4d08cd48b1c84845ca0481766a1701911d257c9fe60`  
		Last Modified: Sat, 19 Sep 2020 00:02:17 GMT  
		Size: 147.7 MB (147660673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649957d7f083af5b1197f2a13e28fefffb9d9e28e07c525e8907479caf613aa`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-python38` - linux; s390x

```console
$ docker pull plone@sha256:2d15e6aa00ff378d2b1c5ea04fca06fce7564ddd991740a237282575c440a1b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180905670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6cc06ff3ca729bed0d018430778a47ff947f360d63b0e54044544f456f417f0`
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
# Thu, 10 Sep 2020 02:08:45 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 02:18:52 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 02:23:40 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:23:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:23:42 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:23:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:23:51 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:43:00 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:43:00 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:43:01 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:43:01 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:48:14 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:48:22 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:48:22 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:48:22 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:48:23 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:48:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:48:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:48:23 GMT
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
	-	`sha256:b7a30ebb749e95a6400495190e32c5b98f37145cc1741244dd3975f759240137`  
		Last Modified: Thu, 10 Sep 2020 02:53:24 GMT  
		Size: 10.3 MB (10274354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9331aa7a0a92e572dee8bf61940f31b2a95c5096898cb20f1592c6e7149db9`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465df3edf63ab70b456383487b281eec77a1064cc829206ac8fd4a9a5b77e0a2`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 2.4 MB (2407622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46fa9d8ec0f2f24706bd965bfcf0afdecd54e6df8bf5df97ae4567053cb3225`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274569e67c881a677c19e6c191f41a2ac47154ec5053ed091e4c33e6347cc6eb`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4b6a40bcb4cc4d2062a10c6aef8541998d6d36cf3acab5c17d269045be4ba`  
		Last Modified: Sat, 19 Sep 2020 00:06:46 GMT  
		Size: 140.1 MB (140063970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8675018f02a5e0a640222ef7297d4581a6cd3f0a81b53d05be3af657cafc95e1`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:alpine`

```console
$ docker pull plone@sha256:b89e51df688bf3daa67443a35e78b7cecd7c59d56d5ea1da009804bbe668b296
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `plone:alpine` - linux; amd64

```console
$ docker pull plone@sha256:c788f9a14c643721f3787afba98489fbd2f49e58a8cee87658dbfcac4affd7fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141391142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e056171b31cd3fa10da6a9bb64ae9c45a6b8201571432a29a4823b71e97358`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:48:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:36:53 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:36:54 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:51:35 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 18 Aug 2020 03:55:10 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 18 Aug 2020 04:03:54 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 18 Aug 2020 04:03:56 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 20:34:03 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:34:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:34:03 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:34:14 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:34:14 GMT
CMD ["python3"]
# Wed, 09 Sep 2020 01:23:38 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 09 Sep 2020 01:23:38 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 09 Sep 2020 01:23:39 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 09 Sep 2020 01:23:39 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 09 Sep 2020 01:32:39 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 09 Sep 2020 01:32:40 GMT
VOLUME [/data]
# Wed, 09 Sep 2020 01:32:40 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Wed, 09 Sep 2020 01:32:40 GMT
EXPOSE 8080
# Wed, 09 Sep 2020 01:32:41 GMT
WORKDIR /plone/instance
# Wed, 09 Sep 2020 01:32:41 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 09 Sep 2020 01:32:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Sep 2020 01:32:41 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b3adc4ff6ffb76ae233f0a92177205845aaf3e9a39e0f96405dabd1423edc9`  
		Last Modified: Wed, 03 Jun 2020 20:14:46 GMT  
		Size: 280.8 KB (280840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db9de03f49990c0ad8d9e2b3bdcbed147dae39c2c6434029bf3cce610f244e2`  
		Last Modified: Tue, 18 Aug 2020 07:53:31 GMT  
		Size: 11.1 MB (11099566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd38a04a61f4179d0fcf8a931a569a515ea435e61865341a9d8aa96d8115d006`  
		Last Modified: Tue, 18 Aug 2020 07:53:29 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3838385f133785631b680aa48443a64e140452a4aacc6ad7319bf9c38f88a0`  
		Last Modified: Wed, 09 Sep 2020 00:16:41 GMT  
		Size: 2.1 MB (2119310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83bc062a1d54fbdfb69b3b7e297afdc0dd7f6bf330607abf8c0ba2e58bb575a`  
		Last Modified: Wed, 09 Sep 2020 01:33:30 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3165309979eec98cddfa51cdd8a69e97a2992a04c44b140ea94928f9abf05e59`  
		Last Modified: Wed, 09 Sep 2020 01:33:29 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f2e75568df5ff44b8f8fcb0b9ac3c0ccb18cbafed035ba2e42e1c29821767f`  
		Last Modified: Wed, 09 Sep 2020 01:33:52 GMT  
		Size: 125.1 MB (125088464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247e4fbbce4d30b9fed96e2ab28917d456b45c704ebcf2d229dbacd8073417f`  
		Last Modified: Wed, 09 Sep 2020 01:33:30 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:b945d50a8d39dd46f3174106c2a4f1c056444c0bf9bf3acbe5f14800eb779830
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140564978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d32c3fd2ed6235cf81077e31d187119ec000dd23c3311177842ebb70c6c2091`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 18:59:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:59:56 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:59:59 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:20:17 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 18 Aug 2020 03:51:14 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 18 Aug 2020 04:07:07 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 18 Aug 2020 04:07:11 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 21:20:25 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 21:20:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 21:20:44 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 21:21:36 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 21:21:45 GMT
CMD ["python3"]
# Tue, 08 Sep 2020 22:30:25 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Tue, 08 Sep 2020 22:30:30 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Tue, 08 Sep 2020 22:30:58 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Tue, 08 Sep 2020 22:31:11 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Tue, 08 Sep 2020 22:51:44 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Tue, 08 Sep 2020 22:51:57 GMT
VOLUME [/data]
# Tue, 08 Sep 2020 22:51:59 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Tue, 08 Sep 2020 22:52:00 GMT
EXPOSE 8080
# Tue, 08 Sep 2020 22:52:01 GMT
WORKDIR /plone/instance
# Tue, 08 Sep 2020 22:52:03 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Tue, 08 Sep 2020 22:52:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Sep 2020 22:52:06 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba84132d8cf30d261b7b1e4e503e67af8ea432e7f530a830161cc1b1bd53e82`  
		Last Modified: Wed, 03 Jun 2020 19:55:42 GMT  
		Size: 281.0 KB (281040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4c50c433d35c45efb946f9c323c99a91c21a9b8f9e386d4a33a33f8070af70`  
		Last Modified: Tue, 18 Aug 2020 04:43:43 GMT  
		Size: 10.8 MB (10754912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e74ed1e7879f5e938736f55e8c7e86f3873f71f5947354a0abf4a15a93461a`  
		Last Modified: Tue, 18 Aug 2020 04:43:39 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13de131ee1b5e933c989f2d300870b32f775152d55e375044682826086d044c0`  
		Last Modified: Tue, 08 Sep 2020 21:51:55 GMT  
		Size: 2.1 MB (2119572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f3f9a9febef519dd65bbc7032abfe4d2abaa9dac2f568527f5182fc18c6f5c`  
		Last Modified: Tue, 08 Sep 2020 22:52:15 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251d05fb68e7c38c3e6918a9c9eb1c835caee3b26ea48c7112ef98cf731e0f7b`  
		Last Modified: Tue, 08 Sep 2020 22:52:15 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00676cf88f7bfd7b68e2179094c6c4f7cf465bc8cd439186fd0ff49c5c3b83ae`  
		Last Modified: Tue, 08 Sep 2020 22:54:00 GMT  
		Size: 124.8 MB (124800681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a3f26e30d95abe1406ce51a2e7d74b59d309527b6fd6533435bc63c79cefe9`  
		Last Modified: Tue, 08 Sep 2020 22:52:15 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:03af3a948c891a0e82a3f9fc2126e31fb8b8d8704e1d1df4ba49f7840fee467a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141200830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5475cab3bc01cb21f1736b9275655c956dc874215fbadac47b7a1f26f92ba3f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:35:35 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:57:57 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:58:00 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:14:44 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 18 Aug 2020 04:32:35 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 18 Aug 2020 04:46:24 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 18 Aug 2020 04:46:26 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 21:48:18 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 21:48:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 21:48:35 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 21:49:00 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 21:49:03 GMT
CMD ["python3"]
# Wed, 09 Sep 2020 00:12:23 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 09 Sep 2020 00:12:24 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 09 Sep 2020 00:12:26 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 09 Sep 2020 00:12:26 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 09 Sep 2020 00:30:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 09 Sep 2020 00:30:55 GMT
VOLUME [/data]
# Wed, 09 Sep 2020 00:30:56 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Wed, 09 Sep 2020 00:30:57 GMT
EXPOSE 8080
# Wed, 09 Sep 2020 00:30:58 GMT
WORKDIR /plone/instance
# Wed, 09 Sep 2020 00:30:58 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 09 Sep 2020 00:30:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Sep 2020 00:31:00 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d489d24c26399308b276dfa175c049e531d2686fb99e250ad3ede210fd01e9e`  
		Last Modified: Wed, 03 Jun 2020 19:46:54 GMT  
		Size: 281.3 KB (281267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b544f7dc429981fa9ee341d8c569955e5f5d86e52f2b9fe1f1836becff40c2`  
		Last Modified: Tue, 18 Aug 2020 05:53:54 GMT  
		Size: 11.2 MB (11232298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01499c5624ba20bf921e0849806a106eb7f28b5700f53b21bc54213b05b2374`  
		Last Modified: Tue, 18 Aug 2020 05:53:51 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29795334e8c6c0a67c138e66172c6c16143e3e5ec2a5ee6a9b0f1a7e2f4e58ef`  
		Last Modified: Tue, 08 Sep 2020 22:54:12 GMT  
		Size: 2.1 MB (2119543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06c6a5907fe96d854e304bf6a5d2bb34c10a328f1f8567519196fa2e33e276`  
		Last Modified: Wed, 09 Sep 2020 00:32:16 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea0e54505d6010b2694baa41866abe38ac8118de0208c30c3f9a0a3ee62901b`  
		Last Modified: Wed, 09 Sep 2020 00:32:17 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdc9f324eac5ca3df1c1e70cf850605613db00f3d3f57e3960ee793b55be76d`  
		Last Modified: Wed, 09 Sep 2020 00:32:54 GMT  
		Size: 124.9 MB (124854274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8af7e8431b4fc913663a083b5e8c729ba38104b46162f0b1127a2f6ace1d0a`  
		Last Modified: Wed, 09 Sep 2020 00:32:17 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; 386

```console
$ docker pull plone@sha256:5a1bc721327cd7c21f7ff344c884dcb46d61600d3d55d607777c664b0cc1c7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132819099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eebbca9ecebfd286c5613dfb2d0c529b996af4f86ae08f3a355ef1c09ca8005`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 18:45:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:45:48 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:45:49 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 18:45:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Jul 2020 18:45:24 GMT
ENV PYTHON_VERSION=3.8.5
# Tue, 04 Aug 2020 00:48:58 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 04 Aug 2020 00:48:59 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 20:19:31 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:19:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:19:32 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:19:39 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:19:39 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:50:37 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:50:37 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:50:38 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:50:38 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 00:01:24 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 00:01:25 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 00:01:25 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Sat, 19 Sep 2020 00:01:26 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 00:01:26 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 00:01:26 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 00:01:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 00:01:26 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded523869d7b2121c2a5838365e9f75504b850ecae6661c940242d3456bd53d7`  
		Last Modified: Wed, 03 Jun 2020 19:28:31 GMT  
		Size: 281.4 KB (281373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918a14653b9dca240ca4d776e8e26326fe1fc8913e2f0a5f294e78a47d492527`  
		Last Modified: Tue, 04 Aug 2020 03:33:25 GMT  
		Size: 11.6 MB (11640740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e582739a3cef82c8012814c112b5ce44b8821ed1191d47884ea5f6faf87354a4`  
		Last Modified: Tue, 04 Aug 2020 03:33:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacf94730cf258787add53ecd2b8540d6b6c2e40e873ebca559d196a85144bac`  
		Last Modified: Tue, 08 Sep 2020 21:21:09 GMT  
		Size: 2.1 MB (2119311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1eaa1f2c0627567de9fd8d8a1d4e74d689837959b8677fbd13763de637c30`  
		Last Modified: Sat, 19 Sep 2020 00:03:55 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01733d323fd86c8c1f8d282960f04a14f7e737b16aa0cb0f3c5cb137619a118a`  
		Last Modified: Sat, 19 Sep 2020 00:03:55 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd009a6477d2a964c8572b059ef5555c61aeaa8c81003413be77ec0a15f4c3e`  
		Last Modified: Sat, 19 Sep 2020 00:04:43 GMT  
		Size: 116.0 MB (115979957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98991b6623467c3f68c18b3bd335cadb11cdabe2d4c711b9c66c2042f7fb4c08`  
		Last Modified: Sat, 19 Sep 2020 00:03:55 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:c7928333e944658a6a74bea1775fbb2cfd32d9a9af29f1aa513b637dc39b5f29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142404280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bebe4df1eeb07427610e2db3f85897b4cea48a75c7b008c40781623b6740957`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 19:35:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:35:58 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:36:09 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:54:46 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 18 Aug 2020 03:55:19 GMT
ENV PYTHON_VERSION=3.7.9
# Tue, 18 Aug 2020 04:07:24 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 18 Aug 2020 04:07:37 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 21:43:31 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 21:43:37 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 21:43:45 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 21:44:28 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 21:44:31 GMT
CMD ["python3"]
# Wed, 09 Sep 2020 00:17:03 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 09 Sep 2020 00:17:13 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 09 Sep 2020 00:17:34 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 09 Sep 2020 00:17:36 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 09 Sep 2020 00:35:27 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 09 Sep 2020 00:35:36 GMT
VOLUME [/data]
# Wed, 09 Sep 2020 00:35:39 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Wed, 09 Sep 2020 00:35:45 GMT
EXPOSE 8080
# Wed, 09 Sep 2020 00:35:53 GMT
WORKDIR /plone/instance
# Wed, 09 Sep 2020 00:35:57 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 09 Sep 2020 00:36:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Sep 2020 00:36:15 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c9759563702d3bc987f9dad6559da6de6fa68093dc6b51fb097c1c4abc1876`  
		Last Modified: Wed, 03 Jun 2020 20:26:29 GMT  
		Size: 285.0 KB (285014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235ded95fa3dbd96f689d2bb2cd7f573ba7186db2b8b754d7fd3683f44b91c65`  
		Last Modified: Tue, 18 Aug 2020 05:08:05 GMT  
		Size: 11.8 MB (11823450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f8a3859d9618409e9e46f9bd51ccaa75bd591c1e28e013fa5a84ca2c7725cf`  
		Last Modified: Tue, 18 Aug 2020 05:08:03 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc20dbfb21bc0e17844f123bc4e33982f6fd90490928fd18b55a09c95f439db0`  
		Last Modified: Tue, 08 Sep 2020 22:51:45 GMT  
		Size: 2.1 MB (2119592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a19d1953fe926f318261fcc0d8495412d1515db44893ea937d2c5bf3563e6b6`  
		Last Modified: Wed, 09 Sep 2020 00:36:47 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188ae4b204f9df81a1a311f37200cbe1f6b5d78e73b439a679211ba447ec2ee4`  
		Last Modified: Wed, 09 Sep 2020 00:36:47 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4704e8af23153091364bd81a0b95376da26ba22b51ea3c99137e46e80b6d721b`  
		Last Modified: Wed, 09 Sep 2020 00:37:18 GMT  
		Size: 125.4 MB (125365539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7bc94ba37e70d07d6e730b9a881b73f62484a48bf2b78270ab111467a1f743`  
		Last Modified: Wed, 09 Sep 2020 00:36:47 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; s390x

```console
$ docker pull plone@sha256:1406a74a9fa6e5a9b1cc63d67aaaf39e401e718750c520edd0129e9383a28beb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (131951362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bba8939e08af189d27667e90bf90ff4996d8b36f9ce149bd3d2810bc095b90c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 19:13:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:13:11 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:13:14 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:13:14 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 21 Jul 2020 18:13:49 GMT
ENV PYTHON_VERSION=3.8.5
# Tue, 04 Aug 2020 00:11:00 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 04 Aug 2020 00:11:01 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 08 Sep 2020 20:18:05 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 08 Sep 2020 20:18:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 08 Sep 2020 20:18:05 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 08 Sep 2020 20:18:10 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Sep 2020 20:18:10 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:59:24 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:59:24 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:59:25 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:59:25 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Sat, 19 Sep 2020 00:05:56 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Sat, 19 Sep 2020 00:06:03 GMT
VOLUME [/data]
# Sat, 19 Sep 2020 00:06:04 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Sat, 19 Sep 2020 00:06:04 GMT
EXPOSE 8080
# Sat, 19 Sep 2020 00:06:04 GMT
WORKDIR /plone/instance
# Sat, 19 Sep 2020 00:06:04 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 19 Sep 2020 00:06:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Sep 2020 00:06:05 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b76e1d722a55ff4f330c758d9814944d8ab0c8761b42febad3c13edcbc7d4f`  
		Last Modified: Wed, 03 Jun 2020 22:40:13 GMT  
		Size: 281.4 KB (281387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cf7186a29294842bc660960abd2809bdcd0271e3ae914b83984ef083d00d78`  
		Last Modified: Tue, 04 Aug 2020 01:14:01 GMT  
		Size: 11.4 MB (11441200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6034b2e6ffbdcc74a2853d09090c84865ee9e7e21a33b945dcdfe53636c60bec`  
		Last Modified: Tue, 04 Aug 2020 01:14:00 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffd5d6fa0f52f2db805d45392fb0e6f47b96dfa61e55b17532e19f56ba696d8`  
		Last Modified: Tue, 08 Sep 2020 20:38:18 GMT  
		Size: 2.1 MB (2119320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714f0030dbd3d72437800281a70e48ccd72132e8848a1575ad3a447b6c80441`  
		Last Modified: Sat, 19 Sep 2020 00:07:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b738e0f383738ee67cbec1bb743c128dea90b5727cc38175f00b03e33ad90`  
		Last Modified: Sat, 19 Sep 2020 00:07:52 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19084bd995188fe20396f258b742cbc0ac5ccbb8835941d9409d80f0d3227add`  
		Last Modified: Sat, 19 Sep 2020 00:08:07 GMT  
		Size: 115.5 MB (115537782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cbb51fb1560a971a9f004beb916f71462b9eb4f993ca8ccc6c8926c7a9d798`  
		Last Modified: Sat, 19 Sep 2020 00:07:52 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:latest`

```console
$ docker pull plone@sha256:6b6714d5cc9e2d01fee3724de3081f7458d31d41d85829fa758497f6cdf54144
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

### `plone:latest` - linux; amd64

```console
$ docker pull plone@sha256:ebdc38c5e493734989f7406c8549e8a8e93e0d5168711dfd6dfa48098fc4fe10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.9 MB (194934892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90313b8c04128be8ac3abbda43a853a92942ffd279c266a03e11bb2b5cfa5dd3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:37 GMT
ADD file:83fbd2352bbac612c7a954e19abd295607cea4482c556c225308e0241b58e2bf in / 
# Thu, 10 Sep 2020 00:30:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 17:34:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 17:34:09 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 17:34:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 17:34:20 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 17:34:21 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 17:45:06 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 17:45:08 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 17:45:08 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 17:45:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 17:45:09 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 17:45:30 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 17:45:30 GMT
CMD ["python3"]
# Fri, 11 Sep 2020 09:23:11 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 11 Sep 2020 09:23:11 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 11 Sep 2020 09:23:12 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 11 Sep 2020 09:23:12 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 11 Sep 2020 09:26:41 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 11 Sep 2020 09:26:42 GMT
VOLUME [/data]
# Fri, 11 Sep 2020 09:26:42 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 11 Sep 2020 09:26:42 GMT
EXPOSE 8080
# Fri, 11 Sep 2020 09:26:42 GMT
WORKDIR /plone/instance
# Fri, 11 Sep 2020 09:26:43 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 11 Sep 2020 09:26:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 09:26:43 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:abb454610128b028301ee40af387d31111a1e699e4ea424fd53186ff77067402`  
		Last Modified: Thu, 10 Sep 2020 00:37:40 GMT  
		Size: 22.5 MB (22522274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cca7c254bca20c23c661af2a80a9f2d26c1473a9fce0c4e7df958610e5125`  
		Last Modified: Thu, 10 Sep 2020 18:58:07 GMT  
		Size: 2.5 MB (2485508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09bd87eaacd2564a11aded5f30cdeb6f48fb6f0ede1e828f9ca1cb52c76a93`  
		Last Modified: Thu, 10 Sep 2020 18:58:09 GMT  
		Size: 10.0 MB (10001970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789a5a11aeffb2eca696932509ac931d098c347d5d4f76bfb854c3b094ef244b`  
		Last Modified: Thu, 10 Sep 2020 18:58:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c332a8eb758e8effc070d08aedc7897f523c1d278f86e45bb35ec19e7f177b51`  
		Last Modified: Thu, 10 Sep 2020 18:58:07 GMT  
		Size: 2.4 MB (2403392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bce5ab678c23e78b108965d3a61c3c48f7e7c07a9400e320ba9e75f83e4874e`  
		Last Modified: Fri, 11 Sep 2020 09:27:07 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d5dcf5c8e86e0104491f41454f0b87662688a91b5407e7bd3278c62eb81d84`  
		Last Modified: Fri, 11 Sep 2020 09:27:07 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee1a5781ad28ed02807ce2b28a303542c1715c0c2ef6af3d1b501369273f6b2`  
		Last Modified: Fri, 11 Sep 2020 09:27:35 GMT  
		Size: 157.5 MB (157513738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a359a8a5b787f8bb19700bb2d05fdff702bc88d675103ea127fba012ee46dc`  
		Last Modified: Fri, 11 Sep 2020 09:27:07 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; arm variant v5

```console
$ docker pull plone@sha256:55fc5ce26d1c18a9f41d85bc7ccae2d67d77e2c05cd5922583c20bf350709645
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.8 MB (184750879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f651fc0f3ff0e19b19a06bd28a0424b80472e6ad864fe4c607fcc9eec98f209`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 09 Sep 2020 23:58:43 GMT
ADD file:696a886e620f9d4e01408d475f27ce43a516a44e3689fd1bd6fa9452e27b9672 in / 
# Wed, 09 Sep 2020 23:58:46 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 08:58:06 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 08:58:10 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 08:58:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 08:59:03 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 08:59:07 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 09:09:54 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 09:10:10 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 09:10:12 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 09:10:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 09:10:17 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 09:11:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 09:11:12 GMT
CMD ["python3"]
# Thu, 10 Sep 2020 19:15:10 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 10 Sep 2020 19:15:17 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 10 Sep 2020 19:15:47 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 10 Sep 2020 19:15:59 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 10 Sep 2020 19:32:08 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 10 Sep 2020 19:32:17 GMT
VOLUME [/data]
# Thu, 10 Sep 2020 19:32:28 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Thu, 10 Sep 2020 19:32:28 GMT
EXPOSE 8080
# Thu, 10 Sep 2020 19:32:31 GMT
WORKDIR /plone/instance
# Thu, 10 Sep 2020 19:32:32 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 10 Sep 2020 19:32:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 10 Sep 2020 19:32:36 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:90bb53eced8a0fc6f31bd3ebc211839305505d162e0df809dfd951cf263f765d`  
		Last Modified: Thu, 10 Sep 2020 00:07:19 GMT  
		Size: 21.2 MB (21194357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9cf59ab1cb8914a632bf6b662cee76a27d3fb7f167e3b50abe6b956af56aab`  
		Last Modified: Thu, 10 Sep 2020 10:39:07 GMT  
		Size: 2.2 MB (2216188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f969f0e2e34b8d1e1ddee7594c94d4992977aac6eee5f40c933e5874a44942`  
		Last Modified: Thu, 10 Sep 2020 10:39:07 GMT  
		Size: 9.3 MB (9349487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56387498a6686b53e8df6491d6a8a5f550681416c6bb394c685f4fbfa2d562f`  
		Last Modified: Thu, 10 Sep 2020 10:39:04 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fe0317644c554fae33bacb2798457d2800a811ec1192ca32387d197a304f00`  
		Last Modified: Thu, 10 Sep 2020 10:39:05 GMT  
		Size: 2.4 MB (2403383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eabec6799d345384ed00826b8f6a3bc9c885e008c4752fa530cf0a3a972fd59`  
		Last Modified: Thu, 10 Sep 2020 19:32:59 GMT  
		Size: 3.9 KB (3925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a0dcee0ed0a1f60cca259c8ca72e3ad39544757270af99dc3a5f015f75366a`  
		Last Modified: Thu, 10 Sep 2020 19:32:59 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37195679d86a086c24f48d2311172303814536a04691696e10dd30ed98ebf43c`  
		Last Modified: Thu, 10 Sep 2020 19:34:00 GMT  
		Size: 149.6 MB (149579408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eb429f60a5e40315c870c33511a46bf8bf7fffb1742e006f3826351d366706`  
		Last Modified: Thu, 10 Sep 2020 19:32:59 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; arm variant v7

```console
$ docker pull plone@sha256:e7e4a86cd6cbb7d3bea3c938a0c10b902bdd7d4beec8dd0979c0de0b4abb9468
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.3 MB (181345132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90b04dd3423b22037aadf7ebe870b682f63e9990dea3cbcbd995e2d331c96e23`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 10 Sep 2020 00:13:48 GMT
ADD file:01ae1c10181763bd674d028f8ce4e5e3bf24c400e60a76fa6bfb43dfba07a0c6 in / 
# Thu, 10 Sep 2020 00:13:49 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 16:14:36 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 16:14:38 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 16:15:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 16:15:04 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 16:15:11 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 16:28:12 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 16:28:18 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 16:28:20 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 16:28:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 16:28:22 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 16:28:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 16:28:53 GMT
CMD ["python3"]
# Fri, 11 Sep 2020 04:51:12 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 11 Sep 2020 04:51:13 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 11 Sep 2020 04:51:17 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 11 Sep 2020 04:51:18 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 11 Sep 2020 05:07:57 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 11 Sep 2020 05:08:05 GMT
VOLUME [/data]
# Fri, 11 Sep 2020 05:08:14 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 11 Sep 2020 05:08:19 GMT
EXPOSE 8080
# Fri, 11 Sep 2020 05:08:22 GMT
WORKDIR /plone/instance
# Fri, 11 Sep 2020 05:08:24 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 11 Sep 2020 05:08:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 05:08:30 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:a1f2bf709796106dda8cc033b6c173e05f0838e1cf4fca653453e2999db8ba3d`  
		Last Modified: Thu, 10 Sep 2020 00:21:34 GMT  
		Size: 19.3 MB (19304627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c541d096a8ce835222b7505b2199a2fd665a67869c8b9f2b755129cb51b196b`  
		Last Modified: Thu, 10 Sep 2020 17:56:46 GMT  
		Size: 2.1 MB (2137387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed09475193f741bd43d93b83b2444cd94399ddcb2227a975304d68a02739e9d`  
		Last Modified: Thu, 10 Sep 2020 17:56:49 GMT  
		Size: 9.3 MB (9293956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d92008ba9651d6514e888d47be1fc262c6865cea3ec182df358577122da74`  
		Last Modified: Thu, 10 Sep 2020 17:56:45 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c12dad74ce56058362a96366b340dc87dc49f87db04e8d14246e63c4ad595a`  
		Last Modified: Thu, 10 Sep 2020 17:56:46 GMT  
		Size: 2.4 MB (2403222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b12d2097cddc00d8db45b6d11749e79e017704fb550fc0ab5c4d151b3dafdc3`  
		Last Modified: Fri, 11 Sep 2020 05:08:57 GMT  
		Size: 3.9 KB (3929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31af93954426c019718919233f3eb15206a5604cc98413e48cfdec64cdabda5`  
		Last Modified: Fri, 11 Sep 2020 05:08:57 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbcda2cc2eed5bbdea9a6c0752685ecdacb64742ca600ccd87b8ea556d8bcc8`  
		Last Modified: Fri, 11 Sep 2020 05:09:50 GMT  
		Size: 148.2 MB (148197887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c852bedef85ad01caf0e6adeec2050bfe963ac73e101e5e111ee34064b1bf6c`  
		Last Modified: Fri, 11 Sep 2020 05:08:57 GMT  
		Size: 2.8 KB (2842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:51a5ef5b8e0a46874b7d0c346711b28142cdb2d1bc4464925d46008c2087714a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183646561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5530a8485ac8504e02417863492f96199338b356dc633935263d903ffc48f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 09 Sep 2020 23:54:57 GMT
ADD file:fe3fc1ceb78e0b280e8429ba94710b765701de58e9958d27e9bcb8af97084f1b in / 
# Wed, 09 Sep 2020 23:55:02 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 15:58:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 15:58:53 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 15:59:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 15:59:13 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Thu, 10 Sep 2020 15:59:15 GMT
ENV PYTHON_VERSION=3.7.9
# Thu, 10 Sep 2020 16:11:48 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 16:11:51 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 16:11:52 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 16:11:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 16:11:53 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 16:12:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 16:12:27 GMT
CMD ["python3"]
# Fri, 11 Sep 2020 05:34:51 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 11 Sep 2020 05:34:52 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 11 Sep 2020 05:34:54 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 11 Sep 2020 05:34:55 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 11 Sep 2020 05:48:37 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 11 Sep 2020 05:48:53 GMT
VOLUME [/data]
# Fri, 11 Sep 2020 05:48:55 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 11 Sep 2020 05:48:56 GMT
EXPOSE 8080
# Fri, 11 Sep 2020 05:48:57 GMT
WORKDIR /plone/instance
# Fri, 11 Sep 2020 05:48:58 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 11 Sep 2020 05:48:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 05:48:59 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:852f38eca5e441cf6f4d6130ee167637bc8117d57f8f0156f5e489e8c3dd8f17`  
		Last Modified: Thu, 10 Sep 2020 00:01:56 GMT  
		Size: 20.4 MB (20377071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f37090d4a5cb835b768bdf2699c911f0d448d9c2ca155d22255740e1ed5eecb`  
		Last Modified: Thu, 10 Sep 2020 17:27:27 GMT  
		Size: 2.2 MB (2199149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a13a01028a219e1cf6f205fffbe7c8710d3b9fa672a17e292b9beae219621f`  
		Last Modified: Thu, 10 Sep 2020 17:27:28 GMT  
		Size: 9.7 MB (9722632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1604b0bb945c7009c3415dc70b9f5c77788464915e5e66ae28849eebc00f1b`  
		Last Modified: Thu, 10 Sep 2020 17:27:27 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd33a7d62112a6c753efacdcd14552b92159c77e934e8a618c50b69f80ac5dc`  
		Last Modified: Thu, 10 Sep 2020 17:27:27 GMT  
		Size: 2.4 MB (2403257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747938999dff604308ed02632aded572c40d7283f6e6c5bc012669a32f68621e`  
		Last Modified: Fri, 11 Sep 2020 05:49:30 GMT  
		Size: 3.9 KB (3940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00c3f60827996df5d7871fe08adbbff9791371cf329fec661818b1782329da`  
		Last Modified: Fri, 11 Sep 2020 05:49:30 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f426165c88c4f688b22dbae86d6e8f93eb94028c33457cb7e525d908ee0f225`  
		Last Modified: Fri, 11 Sep 2020 05:50:13 GMT  
		Size: 148.9 MB (148936386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38ca0ab5fcb0370dcc883c56af596750de0fc74d29827b575efe5f1416f7c4a`  
		Last Modified: Fri, 11 Sep 2020 05:49:31 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; 386

```console
$ docker pull plone@sha256:74dae2a340501d74b181e6f810bcc5987c5100d435af746737c7cd0228deea0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191123328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6446e55c7fa3222601f6ce73289c88370dc91240430988053f72b10cecd98b4`
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
# Thu, 10 Sep 2020 12:08:17 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 12:37:25 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 12:50:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 12:50:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 12:50:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 12:50:46 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:38:43 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:38:44 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:38:44 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:38:45 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:42:19 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:42:20 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:42:20 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:42:20 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:42:20 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:42:21 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:42:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:42:21 GMT
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
	-	`sha256:9f8d61ae8767c42662c4758765a4389aafccb33e94098c128d01e1436856e52a`  
		Last Modified: Thu, 10 Sep 2020 15:18:10 GMT  
		Size: 10.5 MB (10532513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fa521131d6f14a06ff5a2ba860f47bc766c993ceeacd79a375a2f8aaf1b970`  
		Last Modified: Thu, 10 Sep 2020 15:18:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b31a66bd5005cb79acf880a9bd8e2446aaa63a0e6a12ca44b136526373f7a6f`  
		Last Modified: Thu, 10 Sep 2020 15:18:06 GMT  
		Size: 2.4 MB (2407674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549278a7ff3477d1945b1c6c146a7886ea07a6e80eef07fab39ab361547ce5`  
		Last Modified: Sat, 19 Sep 2020 00:01:42 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921c0542d2620f8af6980da808c1cb6275509da47bcd7b7d17dcf0b53537c9b`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a986571b35c520ca4a2ac4d08cd48b1c84845ca0481766a1701911d257c9fe60`  
		Last Modified: Sat, 19 Sep 2020 00:02:17 GMT  
		Size: 147.7 MB (147660673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649957d7f083af5b1197f2a13e28fefffb9d9e28e07c525e8907479caf613aa`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; ppc64le

```console
$ docker pull plone@sha256:c3c2b4338c89e4b0dc0ebf0d2e7adbaaeba330d601d4ec045cd4b61db5a1b407
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197172893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c73e6fb8803df461bdc412f5b0178f5c2999e3996822554ff3965f1db75dc6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 19:31:59 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 19:32:07 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 19:32:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 19:33:02 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 30 Jun 2020 19:03:08 GMT
ENV PYTHON_VERSION=3.7.8
# Tue, 30 Jun 2020 19:23:23 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Tue, 30 Jun 2020 19:23:36 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 30 Jun 2020 19:23:41 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Tue, 30 Jun 2020 19:23:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Tue, 30 Jun 2020 19:23:55 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Tue, 30 Jun 2020 19:25:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 30 Jun 2020 19:25:56 GMT
CMD ["python3"]
# Tue, 30 Jun 2020 22:42:09 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Tue, 30 Jun 2020 22:42:11 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Tue, 30 Jun 2020 22:42:20 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Tue, 30 Jun 2020 22:42:22 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Tue, 30 Jun 2020 23:05:01 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Tue, 30 Jun 2020 23:05:09 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:05:10 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Tue, 30 Jun 2020 23:05:13 GMT
EXPOSE 8080
# Tue, 30 Jun 2020 23:05:19 GMT
WORKDIR /plone/instance
# Tue, 30 Jun 2020 23:05:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Tue, 30 Jun 2020 23:05:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 30 Jun 2020 23:05:31 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65db400552099f2d550e694f8b2c4585a9241771c3888459e95933e3952c00a2`  
		Last Modified: Tue, 09 Jun 2020 22:04:50 GMT  
		Size: 2.1 MB (2149602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08384149d3416d25ce4786393ffc43365435b8ee5abe3a9b312b54e165b338b`  
		Last Modified: Tue, 30 Jun 2020 21:03:12 GMT  
		Size: 19.7 MB (19714165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5889ef0bc0f687b9775913850358909987604b1b5d929b521c1ed81b9fb3e679`  
		Last Modified: Tue, 30 Jun 2020 21:03:05 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b9d713da50b69b94f1ac3a37593022c77b377fb92afa52673934aa329b289`  
		Last Modified: Tue, 30 Jun 2020 21:03:06 GMT  
		Size: 2.2 MB (2216976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b3530a849735869c2a1882cba7beda7a6fee1202289f9c121d1ec39ec3d94e`  
		Last Modified: Tue, 30 Jun 2020 23:25:33 GMT  
		Size: 3.9 KB (3942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd61c145fe975fa9ac1f3222cd64a118b9553bf87c70a56d6602c1c7134443e8`  
		Last Modified: Tue, 30 Jun 2020 23:25:32 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc23229b857f88f77670bce57410e2d75ee5cf23cdd61013b64e37d3cd424ad6`  
		Last Modified: Tue, 30 Jun 2020 23:26:05 GMT  
		Size: 150.3 MB (150292808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382269925414c1f4ccc45274913d6519255ceefabd509d702ab18e80b1100219`  
		Last Modified: Tue, 30 Jun 2020 23:25:32 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; s390x

```console
$ docker pull plone@sha256:2d15e6aa00ff378d2b1c5ea04fca06fce7564ddd991740a237282575c440a1b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180905670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6cc06ff3ca729bed0d018430778a47ff947f360d63b0e54044544f456f417f0`
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
# Thu, 10 Sep 2020 02:08:45 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 02:18:52 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 02:23:40 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:23:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:23:42 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:23:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:23:51 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:43:00 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:43:00 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:43:01 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:43:01 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:48:14 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:48:22 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:48:22 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:48:22 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:48:23 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:48:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:48:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:48:23 GMT
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
	-	`sha256:b7a30ebb749e95a6400495190e32c5b98f37145cc1741244dd3975f759240137`  
		Last Modified: Thu, 10 Sep 2020 02:53:24 GMT  
		Size: 10.3 MB (10274354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9331aa7a0a92e572dee8bf61940f31b2a95c5096898cb20f1592c6e7149db9`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465df3edf63ab70b456383487b281eec77a1064cc829206ac8fd4a9a5b77e0a2`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 2.4 MB (2407622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46fa9d8ec0f2f24706bd965bfcf0afdecd54e6df8bf5df97ae4567053cb3225`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274569e67c881a677c19e6c191f41a2ac47154ec5053ed091e4c33e6347cc6eb`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4b6a40bcb4cc4d2062a10c6aef8541998d6d36cf3acab5c17d269045be4ba`  
		Last Modified: Sat, 19 Sep 2020 00:06:46 GMT  
		Size: 140.1 MB (140063970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8675018f02a5e0a640222ef7297d4581a6cd3f0a81b53d05be3af657cafc95e1`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:python36`

```console
$ docker pull plone@sha256:a2ebdd38d97be21752d8d004bac60ad9d3177bee8bc531b249a54057a3312c96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:python36` - linux; 386

```console
$ docker pull plone@sha256:c009706f351a0758693b4fa34b1c70e928136dcef51c46b5e47ddbc2d4473ad5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.0 MB (189984339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55bd17803580a91d78624be33e46791fa9462b8792e59c0c661a3ff103da5724`
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
# Thu, 10 Sep 2020 13:56:58 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 10 Sep 2020 14:10:19 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 14:10:19 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 14:10:20 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 14:10:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 14:10:20 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 14:10:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 14:10:42 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:46:34 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:46:34 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:46:35 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:46:35 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:50:19 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:50:21 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:50:21 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:50:21 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:50:21 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:50:22 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:50:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:50:22 GMT
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
	-	`sha256:c5811e4a19b8908528b06e1780be3c531a34613499c58be290e7c559261fef52`  
		Last Modified: Thu, 10 Sep 2020 15:19:26 GMT  
		Size: 9.8 MB (9780518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f556bb98a43b664a6d700f148d204a93d94e87f8d76b1d69b9a4fe0aadddde`  
		Last Modified: Thu, 10 Sep 2020 15:19:23 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb36eba2fe2fc3b3f3bee649c64b96d9ec7c8b9fe5baa197b2927282de53a71`  
		Last Modified: Thu, 10 Sep 2020 15:19:24 GMT  
		Size: 2.4 MB (2407802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baeec906bc5130be0d5f38a06c502ffe76466489c72e984f7334a31ec783d6b`  
		Last Modified: Sat, 19 Sep 2020 00:03:13 GMT  
		Size: 3.9 KB (3892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cd72de142ba9330c267027c28a707647a65de4151001a48ca92df916e91bf`  
		Last Modified: Sat, 19 Sep 2020 00:03:13 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c5792fc1bde4723c80c21dd3ec6061e34dcb0aa112d09487d3b586ec04d57e`  
		Last Modified: Sat, 19 Sep 2020 00:03:49 GMT  
		Size: 147.3 MB (147273555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae731a9ad6b30b57c7fab7c10ab1a92719cca1208bb8e9e430f22b00e68357`  
		Last Modified: Sat, 19 Sep 2020 00:03:13 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python36` - linux; s390x

```console
$ docker pull plone@sha256:fbd3b0ab694c3ec04dd1ea737d4c70f6242e057ad9282daa02540d3bb0219f8e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.0 MB (179980261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c914fd66f05d111b83c25da1e3e2069d580b4b7acaa25ebb002233d0964614c8`
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
# Thu, 10 Sep 2020 02:39:23 GMT
ENV PYTHON_VERSION=3.6.12
# Thu, 10 Sep 2020 02:43:22 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:43:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:43:23 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:43:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:43:24 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:43:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:43:34 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:54:01 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:54:01 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:54:02 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:54:02 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:59:07 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:59:15 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:59:15 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:59:15 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:59:16 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:59:16 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:59:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:59:16 GMT
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
	-	`sha256:c1297fe51a7a4e624059ae60fb8d5aa6836a977f1afe776fe8bd18884f3f2fbe`  
		Last Modified: Thu, 10 Sep 2020 02:54:06 GMT  
		Size: 9.6 MB (9565972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f25ae5f7b5ef39e22975547a201ce4b9d385c55b4570ad583eafb2e646127a1`  
		Last Modified: Thu, 10 Sep 2020 02:54:05 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee1104daf6f35ff379bb4059fce361ea82be478c1b462da304ba0cf9e1d8548`  
		Last Modified: Thu, 10 Sep 2020 02:54:05 GMT  
		Size: 2.4 MB (2407761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9b0414301d20f3499e7a50dbcd63734d291cd28deaba4e205f9a7771afe131`  
		Last Modified: Sat, 19 Sep 2020 00:07:26 GMT  
		Size: 4.0 KB (3956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa20e556f792f8871aa2d142b4f4ef75c8298493f3f81586f3e8e70fa24d3f3`  
		Last Modified: Sat, 19 Sep 2020 00:07:26 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b1c3a8a197509f51971148bce94e710c9c2cf9fa6eb4597ebbe42706e02a20`  
		Last Modified: Sat, 19 Sep 2020 00:07:44 GMT  
		Size: 139.8 MB (139846804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7de228ceaba39ab0c4ce189e67585eb5344670ad4e660fb19bb0b7c4f9c394`  
		Last Modified: Sat, 19 Sep 2020 00:07:26 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:python37`

```console
$ docker pull plone@sha256:1d0c0680b18a1cdbd245c30a2f98994cdbcd885f6f1a58c321728ec784f61705
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

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

## `plone:python38`

```console
$ docker pull plone@sha256:df29336b72bd033353b7ca4d4f5f84e900b9abdf1dae32c45ba007eca9832a01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; 386
	-	linux; s390x

### `plone:python38` - linux; 386

```console
$ docker pull plone@sha256:74dae2a340501d74b181e6f810bcc5987c5100d435af746737c7cd0228deea0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191123328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6446e55c7fa3222601f6ce73289c88370dc91240430988053f72b10cecd98b4`
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
# Thu, 10 Sep 2020 12:08:17 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 12:37:25 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 12:50:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 12:50:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 12:50:29 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 12:50:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 12:50:46 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:38:43 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:38:44 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:38:44 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:38:45 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:42:19 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:42:20 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:42:20 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:42:20 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:42:20 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:42:21 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:42:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:42:21 GMT
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
	-	`sha256:9f8d61ae8767c42662c4758765a4389aafccb33e94098c128d01e1436856e52a`  
		Last Modified: Thu, 10 Sep 2020 15:18:10 GMT  
		Size: 10.5 MB (10532513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fa521131d6f14a06ff5a2ba860f47bc766c993ceeacd79a375a2f8aaf1b970`  
		Last Modified: Thu, 10 Sep 2020 15:18:04 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b31a66bd5005cb79acf880a9bd8e2446aaa63a0e6a12ca44b136526373f7a6f`  
		Last Modified: Thu, 10 Sep 2020 15:18:06 GMT  
		Size: 2.4 MB (2407674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549278a7ff3477d1945b1c6c146a7886ea07a6e80eef07fab39ab361547ce5`  
		Last Modified: Sat, 19 Sep 2020 00:01:42 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921c0542d2620f8af6980da808c1cb6275509da47bcd7b7d17dcf0b53537c9b`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a986571b35c520ca4a2ac4d08cd48b1c84845ca0481766a1701911d257c9fe60`  
		Last Modified: Sat, 19 Sep 2020 00:02:17 GMT  
		Size: 147.7 MB (147660673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649957d7f083af5b1197f2a13e28fefffb9d9e28e07c525e8907479caf613aa`  
		Last Modified: Sat, 19 Sep 2020 00:01:41 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python38` - linux; s390x

```console
$ docker pull plone@sha256:2d15e6aa00ff378d2b1c5ea04fca06fce7564ddd991740a237282575c440a1b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180905670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6cc06ff3ca729bed0d018430778a47ff947f360d63b0e54044544f456f417f0`
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
# Thu, 10 Sep 2020 02:08:45 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 10 Sep 2020 02:18:52 GMT
ENV PYTHON_VERSION=3.8.5
# Thu, 10 Sep 2020 02:23:40 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& python3 --version
# Thu, 10 Sep 2020 02:23:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 10 Sep 2020 02:23:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 10 Sep 2020 02:23:42 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 10 Sep 2020 02:23:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 10 Sep 2020 02:23:51 GMT
CMD ["python3"]
# Fri, 18 Sep 2020 23:43:00 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 18 Sep 2020 23:43:00 GMT
LABEL plone=5.2.2 os=debian os.version=10 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 18 Sep 2020 23:43:01 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Fri, 18 Sep 2020 23:43:01 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 18 Sep 2020 23:48:14 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Fri, 18 Sep 2020 23:48:22 GMT
VOLUME [/data]
# Fri, 18 Sep 2020 23:48:22 GMT
COPY multi:99d5444b921eba56bcc323ee0a105beca3daad69ba31693c8eb837fa5d34211d in / 
# Fri, 18 Sep 2020 23:48:22 GMT
EXPOSE 8080
# Fri, 18 Sep 2020 23:48:23 GMT
WORKDIR /plone/instance
# Fri, 18 Sep 2020 23:48:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 18 Sep 2020 23:48:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Sep 2020 23:48:23 GMT
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
	-	`sha256:b7a30ebb749e95a6400495190e32c5b98f37145cc1741244dd3975f759240137`  
		Last Modified: Thu, 10 Sep 2020 02:53:24 GMT  
		Size: 10.3 MB (10274354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9331aa7a0a92e572dee8bf61940f31b2a95c5096898cb20f1592c6e7149db9`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465df3edf63ab70b456383487b281eec77a1064cc829206ac8fd4a9a5b77e0a2`  
		Last Modified: Thu, 10 Sep 2020 02:53:23 GMT  
		Size: 2.4 MB (2407622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46fa9d8ec0f2f24706bd965bfcf0afdecd54e6df8bf5df97ae4567053cb3225`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274569e67c881a677c19e6c191f41a2ac47154ec5053ed091e4c33e6347cc6eb`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4b6a40bcb4cc4d2062a10c6aef8541998d6d36cf3acab5c17d269045be4ba`  
		Last Modified: Sat, 19 Sep 2020 00:06:46 GMT  
		Size: 140.1 MB (140063970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8675018f02a5e0a640222ef7297d4581a6cd3f0a81b53d05be3af657cafc95e1`  
		Last Modified: Sat, 19 Sep 2020 00:06:28 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
