<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `plone`

-	[`plone:5`](#plone5)
-	[`plone:5.2`](#plone52)
-	[`plone:5.2.1`](#plone521)
-	[`plone:5.2.1-alpine`](#plone521-alpine)
-	[`plone:5.2.1-python2`](#plone521-python2)
-	[`plone:5.2-alpine`](#plone52-alpine)
-	[`plone:5.2-python2`](#plone52-python2)
-	[`plone:5-alpine`](#plone5-alpine)
-	[`plone:5-python2`](#plone5-python2)
-	[`plone:alpine`](#plonealpine)
-	[`plone:latest`](#plonelatest)
-	[`plone:python2`](#plonepython2)

## `plone:5`

```console
$ docker pull plone@sha256:c583cb291d96e07260995ecdf50728fd44e7ac8a53d6bea2e53aaa7ce1222aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `plone:5` - linux; amd64

```console
$ docker pull plone@sha256:0cb3178ff05119e305704fb1b3718000ca517e7a531968bcac3a3e519005f195
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211253085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe96873b433705c1595266384781fc091c2122377a84e205e4f0529935cd4b42`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:35:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:35:17 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 15:55:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 15:55:25 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:45:41 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:53:40 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:53:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:53:41 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:53:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:53:41 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:54:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:54:02 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:32:15 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:32:15 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:32:16 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:32:16 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:36:21 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:36:22 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:36:23 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 01:36:23 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:36:23 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:36:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:36:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:36:24 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87645a1e5dc6a7cce4b4059148c822ef0bfac62508e535151f34fd7ef2ff0be`  
		Last Modified: Wed, 26 Feb 2020 17:48:38 GMT  
		Size: 2.5 MB (2531205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b2a106525c16b953cfac555f4bd97f1158ee7ecd291c534b4d7ea8c62530d`  
		Last Modified: Wed, 11 Mar 2020 01:16:27 GMT  
		Size: 25.8 MB (25814054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2caaa87d8571682506fceb34dc423a115adafac19e7c26ddf48ac5c524afba`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7523def2decc1a9122ef74d34ed1d23a7e3afdd75c918d37afc4662be769ae31`  
		Last Modified: Wed, 11 Mar 2020 01:16:22 GMT  
		Size: 2.2 MB (2174480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c989baa44940ac8f4f3f0ba3a7571aeb38be8d60c5ac1b126e634f8fe0ada5f4`  
		Last Modified: Wed, 11 Mar 2020 01:47:00 GMT  
		Size: 3.9 KB (3882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d018905dbfdfac4b268d87683be09e4c0a8413931c9a1d5f7065c96296dbcea9`  
		Last Modified: Wed, 11 Mar 2020 01:47:00 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6d9ea7bdb2987d14a9675c8d91025dbebf5662169e4895e4d1ab8bb579480c`  
		Last Modified: Wed, 11 Mar 2020 01:47:30 GMT  
		Size: 158.2 MB (158212196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98abd9fa4b73bdf091c75d5aca4a7e6913b94d6754e67e51ca54c6fd5d3ad589`  
		Last Modified: Wed, 11 Mar 2020 01:47:00 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; arm variant v5

```console
$ docker pull plone@sha256:6d098653440cb9c09ee4078a6d6376de8c638d37978df489383ceda59aece7a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.2 MB (204161309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81312fdd64b21072ec52cd402403ae7a20fe5294f04b7275056a8535f39264e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:53:47 GMT
ADD file:3fa7d31ad19db7be28acd7abacb98667f814acaf8ef495a9abb855abe19c351d in / 
# Wed, 26 Feb 2020 00:53:52 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:42:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 07:42:51 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 07:43:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 07:43:10 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:45:47 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:55:56 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:55:59 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:55:59 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:56:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:56:02 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:56:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:56:35 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:14:51 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:14:52 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:14:54 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:14:54 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:29:36 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:29:41 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:29:41 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 01:29:42 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:29:43 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:29:43 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:29:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:29:45 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8b6b97522cf0c1b41e02f7a9de64e8eb22bf8ff5c5ae70bbb46c20761af19aff`  
		Last Modified: Wed, 26 Feb 2020 01:03:39 GMT  
		Size: 21.2 MB (21190915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9992cac12f0e315e738b1de5043f1f997260800f3db4354158b7c6f8167a59d6`  
		Last Modified: Wed, 26 Feb 2020 09:52:31 GMT  
		Size: 2.3 MB (2256558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92c89a1c809c7e2e06de3f9b74e3477e19a8c7e1476c323435e70dd0af7a14`  
		Last Modified: Wed, 11 Mar 2020 00:59:09 GMT  
		Size: 22.8 MB (22774720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208971892dd05fdf86f76efc76041389fa5b1ccc9d61f3a01e3f42e718ddcf17`  
		Last Modified: Wed, 11 Mar 2020 00:59:01 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35230a6c8743392e9e2a71494f96888fe7c3c2adeaf01f994e345fe8a4f87f5a`  
		Last Modified: Wed, 11 Mar 2020 00:59:02 GMT  
		Size: 2.2 MB (2174471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e561d6b0e2609ad719f94ea798b4268e2c134de85a65ee5bfdf94abddf8274aa`  
		Last Modified: Wed, 11 Mar 2020 01:30:14 GMT  
		Size: 3.9 KB (3927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc51c443208a1e2450955b4dd9317f517255a5f7d6b9989b9f08b2642b40dc0`  
		Last Modified: Wed, 11 Mar 2020 01:30:14 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b86bfd9a64793b4c244055f0d2e3df61fae1fe93c63d6d7045aa134736f9d9e`  
		Last Modified: Wed, 11 Mar 2020 01:31:13 GMT  
		Size: 155.8 MB (155756814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5e9a5787f7acfecfe4a0adb5f67f2a9dd93db677352a85ac8347356bda19bd`  
		Last Modified: Wed, 11 Mar 2020 01:30:15 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; arm variant v7

```console
$ docker pull plone@sha256:53abb10dca0476d722cf7340a88ded5fc1de0ecaff947764d7a31b9d2636c5bb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201410579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4b6de4f8793d6fb85b3e886eb49cbb537e8f2ce8daeae8ce46105e4167ea63`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 10:10:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 10:10:05 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 10:10:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 10:10:23 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:41:57 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:55:00 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:55:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:55:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:55:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:55:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:55:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:55:36 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:40:25 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:40:25 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:40:27 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:40:28 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:53:34 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:53:40 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:53:41 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 01:53:41 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:53:42 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:53:42 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:53:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:53:44 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a1abc64420e94f85d5deba6b89198f83ed3b269e0396792a904f32d4c1b41a`  
		Last Modified: Wed, 26 Feb 2020 12:27:50 GMT  
		Size: 2.2 MB (2177910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45e41c6e2f8aaef75d598dea9eca9d40f4fcda2a0901582aebe6d306ee50efe`  
		Last Modified: Wed, 11 Mar 2020 01:24:13 GMT  
		Size: 23.3 MB (23309168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607048708c96e44149035b34a2ed5a3e87628ebec4c259dfec7b9db0e26cb3e8`  
		Last Modified: Wed, 11 Mar 2020 01:24:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2640e593c8f87c8624e2b11445083bdec9c44c44b299b19b4204bb86b76524`  
		Last Modified: Wed, 11 Mar 2020 01:24:06 GMT  
		Size: 2.2 MB (2174477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951a3359b1f20d805716e61fdb3006312addf55d34a6a694e85ab91f417d0a4f`  
		Last Modified: Wed, 11 Mar 2020 01:54:02 GMT  
		Size: 3.9 KB (3923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8787cfaf46151cc05c3cb8bfac270908dfd3de1c64b943126e70b51dc2798273`  
		Last Modified: Wed, 11 Mar 2020 01:54:03 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa725bb12cf10f82e4d4cf5669b08c5da3c39c07b3f35fad64fcd8996b7c6b58`  
		Last Modified: Wed, 11 Mar 2020 01:55:02 GMT  
		Size: 154.4 MB (154442850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dd734c260cb9196caf7cfc4d256bb7f8d3c5c7f5b0b56ca1e8772d273e81bb`  
		Last Modified: Wed, 11 Mar 2020 01:54:02 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:00fef410ced7c8124ba6679e6660210ab431894e06d6b508678d1a497c40ee12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.7 MB (204729108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9713e846490b44dc73dd613f727365112ac269982773eddfc85f587164850cde`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 06:49:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 06:49:15 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 16:31:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 16:31:06 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:19:30 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:32:02 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:32:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:32:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:32:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:32:07 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:32:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:32:35 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:20:07 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:20:08 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:20:10 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:20:11 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:33:22 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:33:27 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:33:28 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 02:33:28 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:33:29 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:33:30 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:33:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:33:31 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa16eb173765dedf5be678e2f52fa830e07c02f08b04230546c226c1c8e3713`  
		Last Modified: Wed, 26 Feb 2020 18:37:39 GMT  
		Size: 2.2 MB (2239022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fe0ef4f061e52c5a449e99af521a6b39c95f8ecb9ac72e7c623cb3d9bf295a`  
		Last Modified: Wed, 11 Mar 2020 02:03:52 GMT  
		Size: 24.6 MB (24648861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99758f14acfef3b5933115eb26e06f8affc666dc4896cbe24251ed44133a99f7`  
		Last Modified: Wed, 11 Mar 2020 02:03:43 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c23db0034242e225d54e2cbf7e896b6ffea4de1a525d6c012248d723beac99`  
		Last Modified: Wed, 11 Mar 2020 02:03:44 GMT  
		Size: 2.2 MB (2174412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fcc65b631d5d768adbf8410f52baba0b32b21c35b43d49f97135ad38151972`  
		Last Modified: Wed, 11 Mar 2020 02:52:34 GMT  
		Size: 3.9 KB (3939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa31b0e87a19054d3aa9a02db510d6a3bc2a3ba1cc602082a551694ef2e45b`  
		Last Modified: Wed, 11 Mar 2020 02:52:34 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902b44f6b903a62d9a139788a4816cadba1acdc844468829dc774bfb30a488`  
		Last Modified: Wed, 11 Mar 2020 02:53:24 GMT  
		Size: 155.3 MB (155288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95b07b6eb49fc08a26cbe7babedb15ff2ba1e6bf4de0160e78517e2d6eee82b`  
		Last Modified: Wed, 11 Mar 2020 02:52:34 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; 386

```console
$ docker pull plone@sha256:65146f9148ef1bc03b555311f39768a00aa2bf62b20120586a43c278a289d0e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.5 MB (210459204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5de6f5d69682704a07fa9cfd305dd4fd27b8f014cba0a4c845a680de6d567e8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:35:41 GMT
ADD file:7d77438aab7eb35501c0d27bd4350a3a9b4fd1988ce7e7fc0670a570b3112590 in / 
# Wed, 26 Feb 2020 00:35:42 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:25:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 11:25:58 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 13:32:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 13:32:29 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:17:17 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:26:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:26:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:26:29 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:26:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:26:29 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:26:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:26:44 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:05:50 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:05:50 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:05:51 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:05:51 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:09:48 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:09:50 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:09:50 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 02:09:50 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:09:50 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:09:51 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:09:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:09:51 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:5cf237473070a9ef7639307699a23bb6c32cd8321bf84c0cf61b6f9c32b44341`  
		Last Modified: Wed, 26 Feb 2020 00:42:02 GMT  
		Size: 23.1 MB (23141399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4967a9ed267c1255b8f9d33516517d50eb0555c2653a3353f92d04d1dc57d4f`  
		Last Modified: Wed, 26 Feb 2020 15:50:10 GMT  
		Size: 2.5 MB (2532885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac247d2b4799c201a9d2b9df26abe8d3d4963053c341fb070ed0c5273667515`  
		Last Modified: Wed, 11 Mar 2020 01:50:00 GMT  
		Size: 24.2 MB (24181838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703246de72ee13411ff22ede73d86fdb2b75f50d0f75a865ea7dddc686ca30cf`  
		Last Modified: Wed, 11 Mar 2020 01:49:53 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cec631a0546598549f0b296cfed4f22a1f8c0be3be5b37eb827e14a5c26390`  
		Last Modified: Wed, 11 Mar 2020 01:49:54 GMT  
		Size: 2.2 MB (2173881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f91b8fd3c30527357ff6e91a32ea02107902cbd9792e23fe1a4650bf4a884b3`  
		Last Modified: Wed, 11 Mar 2020 02:20:34 GMT  
		Size: 3.9 KB (3875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e435f995303fafcf9a2cda29a1c614bc6099c69c1aba2f567204ee271be18a`  
		Last Modified: Wed, 11 Mar 2020 02:20:34 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4e51d9c776bb1628133878b3190f1cda8cb6b911f92517dfd0f8ca092cd27`  
		Last Modified: Wed, 11 Mar 2020 02:21:15 GMT  
		Size: 158.4 MB (158421426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2077f302ac4bd347f71e254a371a7879ef941d0cae2dcf00876ae88f6028df`  
		Last Modified: Wed, 11 Mar 2020 02:20:34 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; ppc64le

```console
$ docker pull plone@sha256:00d6f420c63806681956a9226fa3ed2228656330898a515abe576d0542201e0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.7 MB (209731614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d633a48efffd457506814ee7f55acacb206adec5798ea69bb4180f7b599db55c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:37:18 GMT
ADD file:661513607cf6a4c5038d6048ea16a04dedb05c03ce6c0e33e409f51510562e11 in / 
# Wed, 26 Feb 2020 01:37:25 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:01:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 04:02:01 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 04:02:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:02:36 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:07:30 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:21:49 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:21:55 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:21:57 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:21:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:22:01 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:22:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:22:49 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:13:26 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:13:29 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:13:40 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:13:41 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:34:53 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:35:00 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:35:01 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 02:35:03 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:35:07 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:35:11 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:35:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:35:18 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:21d148b1dce5a6179231486bac7845a111bbaba4fcaf4232bbc39842bf6c5366`  
		Last Modified: Wed, 26 Feb 2020 02:04:13 GMT  
		Size: 22.8 MB (22785269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04588e26d3c0ec872194ff5ef594823fcf086866a0ec8f2d5a6eeddd987ed841`  
		Last Modified: Wed, 26 Feb 2020 06:05:23 GMT  
		Size: 2.2 MB (2192705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd168104b4b256e82aacc6ed232d1568f33b1e93a094780a12e92564cb7da8`  
		Last Modified: Wed, 11 Mar 2020 01:52:19 GMT  
		Size: 25.9 MB (25853125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f1050b97275cfe94c058bf8f2ea59586046a45a8bc3c5ca46d8994d43ac035`  
		Last Modified: Wed, 11 Mar 2020 01:52:11 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be261a9444d3fba5dc1a3bd9a97b796835615927636aee545115461247a7f02`  
		Last Modified: Wed, 11 Mar 2020 01:52:12 GMT  
		Size: 2.2 MB (2175332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d5b0650bdae6cc629411942f8996e26cd0f0ad4cef676d8144c46a49a527fa`  
		Last Modified: Wed, 11 Mar 2020 02:54:30 GMT  
		Size: 3.9 KB (3935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7573258eb31ff044d820fb7d687da62edd99dff534c759fd3799b0601ea0a89`  
		Last Modified: Wed, 11 Mar 2020 02:54:41 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fb8f493563d5a382df2a8a844e8d407278432a5739ec90c38ab3ee1676a217`  
		Last Modified: Wed, 11 Mar 2020 02:55:41 GMT  
		Size: 156.7 MB (156717344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bc946735b67e3cb0651e21d3ee7391eaaf81b9634cb3fe0914e938a0d0c14d`  
		Last Modified: Wed, 11 Mar 2020 02:54:30 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2`

```console
$ docker pull plone@sha256:c583cb291d96e07260995ecdf50728fd44e7ac8a53d6bea2e53aaa7ce1222aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `plone:5.2` - linux; amd64

```console
$ docker pull plone@sha256:0cb3178ff05119e305704fb1b3718000ca517e7a531968bcac3a3e519005f195
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211253085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe96873b433705c1595266384781fc091c2122377a84e205e4f0529935cd4b42`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:35:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:35:17 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 15:55:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 15:55:25 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:45:41 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:53:40 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:53:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:53:41 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:53:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:53:41 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:54:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:54:02 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:32:15 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:32:15 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:32:16 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:32:16 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:36:21 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:36:22 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:36:23 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 01:36:23 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:36:23 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:36:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:36:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:36:24 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87645a1e5dc6a7cce4b4059148c822ef0bfac62508e535151f34fd7ef2ff0be`  
		Last Modified: Wed, 26 Feb 2020 17:48:38 GMT  
		Size: 2.5 MB (2531205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b2a106525c16b953cfac555f4bd97f1158ee7ecd291c534b4d7ea8c62530d`  
		Last Modified: Wed, 11 Mar 2020 01:16:27 GMT  
		Size: 25.8 MB (25814054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2caaa87d8571682506fceb34dc423a115adafac19e7c26ddf48ac5c524afba`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7523def2decc1a9122ef74d34ed1d23a7e3afdd75c918d37afc4662be769ae31`  
		Last Modified: Wed, 11 Mar 2020 01:16:22 GMT  
		Size: 2.2 MB (2174480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c989baa44940ac8f4f3f0ba3a7571aeb38be8d60c5ac1b126e634f8fe0ada5f4`  
		Last Modified: Wed, 11 Mar 2020 01:47:00 GMT  
		Size: 3.9 KB (3882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d018905dbfdfac4b268d87683be09e4c0a8413931c9a1d5f7065c96296dbcea9`  
		Last Modified: Wed, 11 Mar 2020 01:47:00 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6d9ea7bdb2987d14a9675c8d91025dbebf5662169e4895e4d1ab8bb579480c`  
		Last Modified: Wed, 11 Mar 2020 01:47:30 GMT  
		Size: 158.2 MB (158212196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98abd9fa4b73bdf091c75d5aca4a7e6913b94d6754e67e51ca54c6fd5d3ad589`  
		Last Modified: Wed, 11 Mar 2020 01:47:00 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; arm variant v5

```console
$ docker pull plone@sha256:6d098653440cb9c09ee4078a6d6376de8c638d37978df489383ceda59aece7a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.2 MB (204161309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81312fdd64b21072ec52cd402403ae7a20fe5294f04b7275056a8535f39264e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:53:47 GMT
ADD file:3fa7d31ad19db7be28acd7abacb98667f814acaf8ef495a9abb855abe19c351d in / 
# Wed, 26 Feb 2020 00:53:52 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:42:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 07:42:51 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 07:43:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 07:43:10 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:45:47 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:55:56 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:55:59 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:55:59 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:56:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:56:02 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:56:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:56:35 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:14:51 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:14:52 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:14:54 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:14:54 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:29:36 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:29:41 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:29:41 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 01:29:42 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:29:43 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:29:43 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:29:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:29:45 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8b6b97522cf0c1b41e02f7a9de64e8eb22bf8ff5c5ae70bbb46c20761af19aff`  
		Last Modified: Wed, 26 Feb 2020 01:03:39 GMT  
		Size: 21.2 MB (21190915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9992cac12f0e315e738b1de5043f1f997260800f3db4354158b7c6f8167a59d6`  
		Last Modified: Wed, 26 Feb 2020 09:52:31 GMT  
		Size: 2.3 MB (2256558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92c89a1c809c7e2e06de3f9b74e3477e19a8c7e1476c323435e70dd0af7a14`  
		Last Modified: Wed, 11 Mar 2020 00:59:09 GMT  
		Size: 22.8 MB (22774720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208971892dd05fdf86f76efc76041389fa5b1ccc9d61f3a01e3f42e718ddcf17`  
		Last Modified: Wed, 11 Mar 2020 00:59:01 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35230a6c8743392e9e2a71494f96888fe7c3c2adeaf01f994e345fe8a4f87f5a`  
		Last Modified: Wed, 11 Mar 2020 00:59:02 GMT  
		Size: 2.2 MB (2174471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e561d6b0e2609ad719f94ea798b4268e2c134de85a65ee5bfdf94abddf8274aa`  
		Last Modified: Wed, 11 Mar 2020 01:30:14 GMT  
		Size: 3.9 KB (3927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc51c443208a1e2450955b4dd9317f517255a5f7d6b9989b9f08b2642b40dc0`  
		Last Modified: Wed, 11 Mar 2020 01:30:14 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b86bfd9a64793b4c244055f0d2e3df61fae1fe93c63d6d7045aa134736f9d9e`  
		Last Modified: Wed, 11 Mar 2020 01:31:13 GMT  
		Size: 155.8 MB (155756814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5e9a5787f7acfecfe4a0adb5f67f2a9dd93db677352a85ac8347356bda19bd`  
		Last Modified: Wed, 11 Mar 2020 01:30:15 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; arm variant v7

```console
$ docker pull plone@sha256:53abb10dca0476d722cf7340a88ded5fc1de0ecaff947764d7a31b9d2636c5bb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201410579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4b6de4f8793d6fb85b3e886eb49cbb537e8f2ce8daeae8ce46105e4167ea63`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 10:10:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 10:10:05 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 10:10:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 10:10:23 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:41:57 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:55:00 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:55:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:55:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:55:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:55:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:55:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:55:36 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:40:25 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:40:25 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:40:27 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:40:28 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:53:34 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:53:40 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:53:41 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 01:53:41 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:53:42 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:53:42 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:53:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:53:44 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a1abc64420e94f85d5deba6b89198f83ed3b269e0396792a904f32d4c1b41a`  
		Last Modified: Wed, 26 Feb 2020 12:27:50 GMT  
		Size: 2.2 MB (2177910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45e41c6e2f8aaef75d598dea9eca9d40f4fcda2a0901582aebe6d306ee50efe`  
		Last Modified: Wed, 11 Mar 2020 01:24:13 GMT  
		Size: 23.3 MB (23309168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607048708c96e44149035b34a2ed5a3e87628ebec4c259dfec7b9db0e26cb3e8`  
		Last Modified: Wed, 11 Mar 2020 01:24:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2640e593c8f87c8624e2b11445083bdec9c44c44b299b19b4204bb86b76524`  
		Last Modified: Wed, 11 Mar 2020 01:24:06 GMT  
		Size: 2.2 MB (2174477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951a3359b1f20d805716e61fdb3006312addf55d34a6a694e85ab91f417d0a4f`  
		Last Modified: Wed, 11 Mar 2020 01:54:02 GMT  
		Size: 3.9 KB (3923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8787cfaf46151cc05c3cb8bfac270908dfd3de1c64b943126e70b51dc2798273`  
		Last Modified: Wed, 11 Mar 2020 01:54:03 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa725bb12cf10f82e4d4cf5669b08c5da3c39c07b3f35fad64fcd8996b7c6b58`  
		Last Modified: Wed, 11 Mar 2020 01:55:02 GMT  
		Size: 154.4 MB (154442850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dd734c260cb9196caf7cfc4d256bb7f8d3c5c7f5b0b56ca1e8772d273e81bb`  
		Last Modified: Wed, 11 Mar 2020 01:54:02 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:00fef410ced7c8124ba6679e6660210ab431894e06d6b508678d1a497c40ee12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.7 MB (204729108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9713e846490b44dc73dd613f727365112ac269982773eddfc85f587164850cde`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 06:49:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 06:49:15 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 16:31:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 16:31:06 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:19:30 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:32:02 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:32:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:32:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:32:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:32:07 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:32:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:32:35 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:20:07 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:20:08 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:20:10 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:20:11 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:33:22 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:33:27 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:33:28 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 02:33:28 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:33:29 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:33:30 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:33:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:33:31 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa16eb173765dedf5be678e2f52fa830e07c02f08b04230546c226c1c8e3713`  
		Last Modified: Wed, 26 Feb 2020 18:37:39 GMT  
		Size: 2.2 MB (2239022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fe0ef4f061e52c5a449e99af521a6b39c95f8ecb9ac72e7c623cb3d9bf295a`  
		Last Modified: Wed, 11 Mar 2020 02:03:52 GMT  
		Size: 24.6 MB (24648861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99758f14acfef3b5933115eb26e06f8affc666dc4896cbe24251ed44133a99f7`  
		Last Modified: Wed, 11 Mar 2020 02:03:43 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c23db0034242e225d54e2cbf7e896b6ffea4de1a525d6c012248d723beac99`  
		Last Modified: Wed, 11 Mar 2020 02:03:44 GMT  
		Size: 2.2 MB (2174412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fcc65b631d5d768adbf8410f52baba0b32b21c35b43d49f97135ad38151972`  
		Last Modified: Wed, 11 Mar 2020 02:52:34 GMT  
		Size: 3.9 KB (3939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa31b0e87a19054d3aa9a02db510d6a3bc2a3ba1cc602082a551694ef2e45b`  
		Last Modified: Wed, 11 Mar 2020 02:52:34 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902b44f6b903a62d9a139788a4816cadba1acdc844468829dc774bfb30a488`  
		Last Modified: Wed, 11 Mar 2020 02:53:24 GMT  
		Size: 155.3 MB (155288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95b07b6eb49fc08a26cbe7babedb15ff2ba1e6bf4de0160e78517e2d6eee82b`  
		Last Modified: Wed, 11 Mar 2020 02:52:34 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; 386

```console
$ docker pull plone@sha256:65146f9148ef1bc03b555311f39768a00aa2bf62b20120586a43c278a289d0e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.5 MB (210459204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5de6f5d69682704a07fa9cfd305dd4fd27b8f014cba0a4c845a680de6d567e8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:35:41 GMT
ADD file:7d77438aab7eb35501c0d27bd4350a3a9b4fd1988ce7e7fc0670a570b3112590 in / 
# Wed, 26 Feb 2020 00:35:42 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:25:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 11:25:58 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 13:32:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 13:32:29 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:17:17 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:26:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:26:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:26:29 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:26:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:26:29 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:26:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:26:44 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:05:50 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:05:50 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:05:51 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:05:51 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:09:48 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:09:50 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:09:50 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 02:09:50 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:09:50 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:09:51 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:09:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:09:51 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:5cf237473070a9ef7639307699a23bb6c32cd8321bf84c0cf61b6f9c32b44341`  
		Last Modified: Wed, 26 Feb 2020 00:42:02 GMT  
		Size: 23.1 MB (23141399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4967a9ed267c1255b8f9d33516517d50eb0555c2653a3353f92d04d1dc57d4f`  
		Last Modified: Wed, 26 Feb 2020 15:50:10 GMT  
		Size: 2.5 MB (2532885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac247d2b4799c201a9d2b9df26abe8d3d4963053c341fb070ed0c5273667515`  
		Last Modified: Wed, 11 Mar 2020 01:50:00 GMT  
		Size: 24.2 MB (24181838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703246de72ee13411ff22ede73d86fdb2b75f50d0f75a865ea7dddc686ca30cf`  
		Last Modified: Wed, 11 Mar 2020 01:49:53 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cec631a0546598549f0b296cfed4f22a1f8c0be3be5b37eb827e14a5c26390`  
		Last Modified: Wed, 11 Mar 2020 01:49:54 GMT  
		Size: 2.2 MB (2173881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f91b8fd3c30527357ff6e91a32ea02107902cbd9792e23fe1a4650bf4a884b3`  
		Last Modified: Wed, 11 Mar 2020 02:20:34 GMT  
		Size: 3.9 KB (3875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e435f995303fafcf9a2cda29a1c614bc6099c69c1aba2f567204ee271be18a`  
		Last Modified: Wed, 11 Mar 2020 02:20:34 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4e51d9c776bb1628133878b3190f1cda8cb6b911f92517dfd0f8ca092cd27`  
		Last Modified: Wed, 11 Mar 2020 02:21:15 GMT  
		Size: 158.4 MB (158421426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2077f302ac4bd347f71e254a371a7879ef941d0cae2dcf00876ae88f6028df`  
		Last Modified: Wed, 11 Mar 2020 02:20:34 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; ppc64le

```console
$ docker pull plone@sha256:00d6f420c63806681956a9226fa3ed2228656330898a515abe576d0542201e0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.7 MB (209731614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d633a48efffd457506814ee7f55acacb206adec5798ea69bb4180f7b599db55c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:37:18 GMT
ADD file:661513607cf6a4c5038d6048ea16a04dedb05c03ce6c0e33e409f51510562e11 in / 
# Wed, 26 Feb 2020 01:37:25 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:01:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 04:02:01 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 04:02:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:02:36 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:07:30 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:21:49 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:21:55 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:21:57 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:21:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:22:01 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:22:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:22:49 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:13:26 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:13:29 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:13:40 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:13:41 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:34:53 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:35:00 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:35:01 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 02:35:03 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:35:07 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:35:11 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:35:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:35:18 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:21d148b1dce5a6179231486bac7845a111bbaba4fcaf4232bbc39842bf6c5366`  
		Last Modified: Wed, 26 Feb 2020 02:04:13 GMT  
		Size: 22.8 MB (22785269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04588e26d3c0ec872194ff5ef594823fcf086866a0ec8f2d5a6eeddd987ed841`  
		Last Modified: Wed, 26 Feb 2020 06:05:23 GMT  
		Size: 2.2 MB (2192705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd168104b4b256e82aacc6ed232d1568f33b1e93a094780a12e92564cb7da8`  
		Last Modified: Wed, 11 Mar 2020 01:52:19 GMT  
		Size: 25.9 MB (25853125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f1050b97275cfe94c058bf8f2ea59586046a45a8bc3c5ca46d8994d43ac035`  
		Last Modified: Wed, 11 Mar 2020 01:52:11 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be261a9444d3fba5dc1a3bd9a97b796835615927636aee545115461247a7f02`  
		Last Modified: Wed, 11 Mar 2020 01:52:12 GMT  
		Size: 2.2 MB (2175332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d5b0650bdae6cc629411942f8996e26cd0f0ad4cef676d8144c46a49a527fa`  
		Last Modified: Wed, 11 Mar 2020 02:54:30 GMT  
		Size: 3.9 KB (3935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7573258eb31ff044d820fb7d687da62edd99dff534c759fd3799b0601ea0a89`  
		Last Modified: Wed, 11 Mar 2020 02:54:41 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fb8f493563d5a382df2a8a844e8d407278432a5739ec90c38ab3ee1676a217`  
		Last Modified: Wed, 11 Mar 2020 02:55:41 GMT  
		Size: 156.7 MB (156717344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bc946735b67e3cb0651e21d3ee7391eaaf81b9634cb3fe0914e938a0d0c14d`  
		Last Modified: Wed, 11 Mar 2020 02:54:30 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2.1`

```console
$ docker pull plone@sha256:c583cb291d96e07260995ecdf50728fd44e7ac8a53d6bea2e53aaa7ce1222aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `plone:5.2.1` - linux; amd64

```console
$ docker pull plone@sha256:0cb3178ff05119e305704fb1b3718000ca517e7a531968bcac3a3e519005f195
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211253085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe96873b433705c1595266384781fc091c2122377a84e205e4f0529935cd4b42`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:35:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:35:17 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 15:55:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 15:55:25 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:45:41 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:53:40 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:53:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:53:41 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:53:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:53:41 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:54:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:54:02 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:32:15 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:32:15 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:32:16 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:32:16 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:36:21 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:36:22 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:36:23 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 01:36:23 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:36:23 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:36:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:36:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:36:24 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87645a1e5dc6a7cce4b4059148c822ef0bfac62508e535151f34fd7ef2ff0be`  
		Last Modified: Wed, 26 Feb 2020 17:48:38 GMT  
		Size: 2.5 MB (2531205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b2a106525c16b953cfac555f4bd97f1158ee7ecd291c534b4d7ea8c62530d`  
		Last Modified: Wed, 11 Mar 2020 01:16:27 GMT  
		Size: 25.8 MB (25814054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2caaa87d8571682506fceb34dc423a115adafac19e7c26ddf48ac5c524afba`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7523def2decc1a9122ef74d34ed1d23a7e3afdd75c918d37afc4662be769ae31`  
		Last Modified: Wed, 11 Mar 2020 01:16:22 GMT  
		Size: 2.2 MB (2174480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c989baa44940ac8f4f3f0ba3a7571aeb38be8d60c5ac1b126e634f8fe0ada5f4`  
		Last Modified: Wed, 11 Mar 2020 01:47:00 GMT  
		Size: 3.9 KB (3882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d018905dbfdfac4b268d87683be09e4c0a8413931c9a1d5f7065c96296dbcea9`  
		Last Modified: Wed, 11 Mar 2020 01:47:00 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6d9ea7bdb2987d14a9675c8d91025dbebf5662169e4895e4d1ab8bb579480c`  
		Last Modified: Wed, 11 Mar 2020 01:47:30 GMT  
		Size: 158.2 MB (158212196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98abd9fa4b73bdf091c75d5aca4a7e6913b94d6754e67e51ca54c6fd5d3ad589`  
		Last Modified: Wed, 11 Mar 2020 01:47:00 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1` - linux; arm variant v5

```console
$ docker pull plone@sha256:6d098653440cb9c09ee4078a6d6376de8c638d37978df489383ceda59aece7a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.2 MB (204161309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81312fdd64b21072ec52cd402403ae7a20fe5294f04b7275056a8535f39264e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:53:47 GMT
ADD file:3fa7d31ad19db7be28acd7abacb98667f814acaf8ef495a9abb855abe19c351d in / 
# Wed, 26 Feb 2020 00:53:52 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:42:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 07:42:51 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 07:43:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 07:43:10 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:45:47 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:55:56 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:55:59 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:55:59 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:56:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:56:02 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:56:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:56:35 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:14:51 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:14:52 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:14:54 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:14:54 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:29:36 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:29:41 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:29:41 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 01:29:42 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:29:43 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:29:43 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:29:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:29:45 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8b6b97522cf0c1b41e02f7a9de64e8eb22bf8ff5c5ae70bbb46c20761af19aff`  
		Last Modified: Wed, 26 Feb 2020 01:03:39 GMT  
		Size: 21.2 MB (21190915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9992cac12f0e315e738b1de5043f1f997260800f3db4354158b7c6f8167a59d6`  
		Last Modified: Wed, 26 Feb 2020 09:52:31 GMT  
		Size: 2.3 MB (2256558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92c89a1c809c7e2e06de3f9b74e3477e19a8c7e1476c323435e70dd0af7a14`  
		Last Modified: Wed, 11 Mar 2020 00:59:09 GMT  
		Size: 22.8 MB (22774720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208971892dd05fdf86f76efc76041389fa5b1ccc9d61f3a01e3f42e718ddcf17`  
		Last Modified: Wed, 11 Mar 2020 00:59:01 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35230a6c8743392e9e2a71494f96888fe7c3c2adeaf01f994e345fe8a4f87f5a`  
		Last Modified: Wed, 11 Mar 2020 00:59:02 GMT  
		Size: 2.2 MB (2174471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e561d6b0e2609ad719f94ea798b4268e2c134de85a65ee5bfdf94abddf8274aa`  
		Last Modified: Wed, 11 Mar 2020 01:30:14 GMT  
		Size: 3.9 KB (3927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc51c443208a1e2450955b4dd9317f517255a5f7d6b9989b9f08b2642b40dc0`  
		Last Modified: Wed, 11 Mar 2020 01:30:14 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b86bfd9a64793b4c244055f0d2e3df61fae1fe93c63d6d7045aa134736f9d9e`  
		Last Modified: Wed, 11 Mar 2020 01:31:13 GMT  
		Size: 155.8 MB (155756814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5e9a5787f7acfecfe4a0adb5f67f2a9dd93db677352a85ac8347356bda19bd`  
		Last Modified: Wed, 11 Mar 2020 01:30:15 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1` - linux; arm variant v7

```console
$ docker pull plone@sha256:53abb10dca0476d722cf7340a88ded5fc1de0ecaff947764d7a31b9d2636c5bb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201410579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4b6de4f8793d6fb85b3e886eb49cbb537e8f2ce8daeae8ce46105e4167ea63`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 10:10:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 10:10:05 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 10:10:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 10:10:23 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:41:57 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:55:00 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:55:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:55:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:55:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:55:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:55:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:55:36 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:40:25 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:40:25 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:40:27 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:40:28 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:53:34 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:53:40 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:53:41 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 01:53:41 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:53:42 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:53:42 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:53:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:53:44 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a1abc64420e94f85d5deba6b89198f83ed3b269e0396792a904f32d4c1b41a`  
		Last Modified: Wed, 26 Feb 2020 12:27:50 GMT  
		Size: 2.2 MB (2177910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45e41c6e2f8aaef75d598dea9eca9d40f4fcda2a0901582aebe6d306ee50efe`  
		Last Modified: Wed, 11 Mar 2020 01:24:13 GMT  
		Size: 23.3 MB (23309168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607048708c96e44149035b34a2ed5a3e87628ebec4c259dfec7b9db0e26cb3e8`  
		Last Modified: Wed, 11 Mar 2020 01:24:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2640e593c8f87c8624e2b11445083bdec9c44c44b299b19b4204bb86b76524`  
		Last Modified: Wed, 11 Mar 2020 01:24:06 GMT  
		Size: 2.2 MB (2174477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951a3359b1f20d805716e61fdb3006312addf55d34a6a694e85ab91f417d0a4f`  
		Last Modified: Wed, 11 Mar 2020 01:54:02 GMT  
		Size: 3.9 KB (3923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8787cfaf46151cc05c3cb8bfac270908dfd3de1c64b943126e70b51dc2798273`  
		Last Modified: Wed, 11 Mar 2020 01:54:03 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa725bb12cf10f82e4d4cf5669b08c5da3c39c07b3f35fad64fcd8996b7c6b58`  
		Last Modified: Wed, 11 Mar 2020 01:55:02 GMT  
		Size: 154.4 MB (154442850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dd734c260cb9196caf7cfc4d256bb7f8d3c5c7f5b0b56ca1e8772d273e81bb`  
		Last Modified: Wed, 11 Mar 2020 01:54:02 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:00fef410ced7c8124ba6679e6660210ab431894e06d6b508678d1a497c40ee12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.7 MB (204729108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9713e846490b44dc73dd613f727365112ac269982773eddfc85f587164850cde`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 06:49:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 06:49:15 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 16:31:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 16:31:06 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:19:30 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:32:02 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:32:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:32:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:32:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:32:07 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:32:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:32:35 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:20:07 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:20:08 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:20:10 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:20:11 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:33:22 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:33:27 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:33:28 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 02:33:28 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:33:29 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:33:30 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:33:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:33:31 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa16eb173765dedf5be678e2f52fa830e07c02f08b04230546c226c1c8e3713`  
		Last Modified: Wed, 26 Feb 2020 18:37:39 GMT  
		Size: 2.2 MB (2239022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fe0ef4f061e52c5a449e99af521a6b39c95f8ecb9ac72e7c623cb3d9bf295a`  
		Last Modified: Wed, 11 Mar 2020 02:03:52 GMT  
		Size: 24.6 MB (24648861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99758f14acfef3b5933115eb26e06f8affc666dc4896cbe24251ed44133a99f7`  
		Last Modified: Wed, 11 Mar 2020 02:03:43 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c23db0034242e225d54e2cbf7e896b6ffea4de1a525d6c012248d723beac99`  
		Last Modified: Wed, 11 Mar 2020 02:03:44 GMT  
		Size: 2.2 MB (2174412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fcc65b631d5d768adbf8410f52baba0b32b21c35b43d49f97135ad38151972`  
		Last Modified: Wed, 11 Mar 2020 02:52:34 GMT  
		Size: 3.9 KB (3939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa31b0e87a19054d3aa9a02db510d6a3bc2a3ba1cc602082a551694ef2e45b`  
		Last Modified: Wed, 11 Mar 2020 02:52:34 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902b44f6b903a62d9a139788a4816cadba1acdc844468829dc774bfb30a488`  
		Last Modified: Wed, 11 Mar 2020 02:53:24 GMT  
		Size: 155.3 MB (155288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95b07b6eb49fc08a26cbe7babedb15ff2ba1e6bf4de0160e78517e2d6eee82b`  
		Last Modified: Wed, 11 Mar 2020 02:52:34 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1` - linux; 386

```console
$ docker pull plone@sha256:65146f9148ef1bc03b555311f39768a00aa2bf62b20120586a43c278a289d0e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.5 MB (210459204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5de6f5d69682704a07fa9cfd305dd4fd27b8f014cba0a4c845a680de6d567e8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:35:41 GMT
ADD file:7d77438aab7eb35501c0d27bd4350a3a9b4fd1988ce7e7fc0670a570b3112590 in / 
# Wed, 26 Feb 2020 00:35:42 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:25:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 11:25:58 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 13:32:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 13:32:29 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:17:17 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:26:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:26:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:26:29 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:26:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:26:29 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:26:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:26:44 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:05:50 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:05:50 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:05:51 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:05:51 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:09:48 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:09:50 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:09:50 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 02:09:50 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:09:50 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:09:51 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:09:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:09:51 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:5cf237473070a9ef7639307699a23bb6c32cd8321bf84c0cf61b6f9c32b44341`  
		Last Modified: Wed, 26 Feb 2020 00:42:02 GMT  
		Size: 23.1 MB (23141399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4967a9ed267c1255b8f9d33516517d50eb0555c2653a3353f92d04d1dc57d4f`  
		Last Modified: Wed, 26 Feb 2020 15:50:10 GMT  
		Size: 2.5 MB (2532885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac247d2b4799c201a9d2b9df26abe8d3d4963053c341fb070ed0c5273667515`  
		Last Modified: Wed, 11 Mar 2020 01:50:00 GMT  
		Size: 24.2 MB (24181838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703246de72ee13411ff22ede73d86fdb2b75f50d0f75a865ea7dddc686ca30cf`  
		Last Modified: Wed, 11 Mar 2020 01:49:53 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cec631a0546598549f0b296cfed4f22a1f8c0be3be5b37eb827e14a5c26390`  
		Last Modified: Wed, 11 Mar 2020 01:49:54 GMT  
		Size: 2.2 MB (2173881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f91b8fd3c30527357ff6e91a32ea02107902cbd9792e23fe1a4650bf4a884b3`  
		Last Modified: Wed, 11 Mar 2020 02:20:34 GMT  
		Size: 3.9 KB (3875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e435f995303fafcf9a2cda29a1c614bc6099c69c1aba2f567204ee271be18a`  
		Last Modified: Wed, 11 Mar 2020 02:20:34 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4e51d9c776bb1628133878b3190f1cda8cb6b911f92517dfd0f8ca092cd27`  
		Last Modified: Wed, 11 Mar 2020 02:21:15 GMT  
		Size: 158.4 MB (158421426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2077f302ac4bd347f71e254a371a7879ef941d0cae2dcf00876ae88f6028df`  
		Last Modified: Wed, 11 Mar 2020 02:20:34 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1` - linux; ppc64le

```console
$ docker pull plone@sha256:00d6f420c63806681956a9226fa3ed2228656330898a515abe576d0542201e0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.7 MB (209731614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d633a48efffd457506814ee7f55acacb206adec5798ea69bb4180f7b599db55c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:37:18 GMT
ADD file:661513607cf6a4c5038d6048ea16a04dedb05c03ce6c0e33e409f51510562e11 in / 
# Wed, 26 Feb 2020 01:37:25 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:01:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 04:02:01 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 04:02:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:02:36 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:07:30 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:21:49 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:21:55 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:21:57 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:21:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:22:01 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:22:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:22:49 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:13:26 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:13:29 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:13:40 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:13:41 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:34:53 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:35:00 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:35:01 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 02:35:03 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:35:07 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:35:11 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:35:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:35:18 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:21d148b1dce5a6179231486bac7845a111bbaba4fcaf4232bbc39842bf6c5366`  
		Last Modified: Wed, 26 Feb 2020 02:04:13 GMT  
		Size: 22.8 MB (22785269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04588e26d3c0ec872194ff5ef594823fcf086866a0ec8f2d5a6eeddd987ed841`  
		Last Modified: Wed, 26 Feb 2020 06:05:23 GMT  
		Size: 2.2 MB (2192705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd168104b4b256e82aacc6ed232d1568f33b1e93a094780a12e92564cb7da8`  
		Last Modified: Wed, 11 Mar 2020 01:52:19 GMT  
		Size: 25.9 MB (25853125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f1050b97275cfe94c058bf8f2ea59586046a45a8bc3c5ca46d8994d43ac035`  
		Last Modified: Wed, 11 Mar 2020 01:52:11 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be261a9444d3fba5dc1a3bd9a97b796835615927636aee545115461247a7f02`  
		Last Modified: Wed, 11 Mar 2020 01:52:12 GMT  
		Size: 2.2 MB (2175332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d5b0650bdae6cc629411942f8996e26cd0f0ad4cef676d8144c46a49a527fa`  
		Last Modified: Wed, 11 Mar 2020 02:54:30 GMT  
		Size: 3.9 KB (3935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7573258eb31ff044d820fb7d687da62edd99dff534c759fd3799b0601ea0a89`  
		Last Modified: Wed, 11 Mar 2020 02:54:41 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fb8f493563d5a382df2a8a844e8d407278432a5739ec90c38ab3ee1676a217`  
		Last Modified: Wed, 11 Mar 2020 02:55:41 GMT  
		Size: 156.7 MB (156717344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bc946735b67e3cb0651e21d3ee7391eaaf81b9634cb3fe0914e938a0d0c14d`  
		Last Modified: Wed, 11 Mar 2020 02:54:30 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2.1-alpine`

```console
$ docker pull plone@sha256:c8dc0c313bb90c1ea86d31758645c0b352053d9f1c316334580ee8faeb798e79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `plone:5.2.1-alpine` - linux; amd64

```console
$ docker pull plone@sha256:0c096be1cf04c60572e92f6e048d48bc06b7aaf10ffc7603bc074339a2cd1202
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167524259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d110dfe8b84924bb805ca859c08c3e31a8423095de96fdc510da999ba8f3cd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:42:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 02:37:13 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 02:37:14 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 02:43:48 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:54:17 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:03:22 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:03:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:03:29 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:03:29 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:36:31 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:36:31 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:36:32 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:36:32 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:46:32 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:46:33 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:46:33 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 01:46:33 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:46:34 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:46:34 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:46:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:46:34 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5ad85d9abaadf23d5ae53c3f32e7ccb2df1956869980bfd2491ff396d348a`  
		Last Modified: Sat, 18 Jan 2020 03:11:07 GMT  
		Size: 301.3 KB (301261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29edaae8dc30d7fc1e5c9c5a016e604e4b7cb4f6c5ecb9a3db52ebfc239db28e`  
		Last Modified: Wed, 11 Mar 2020 01:16:37 GMT  
		Size: 28.7 MB (28662304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b1dc8253c8ff1738172bc5fdd061c70e30c965e11fd50436c2de192b80aaf`  
		Last Modified: Wed, 11 Mar 2020 01:16:31 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf370601a519cbf3f23c20bd5324374f3298a016e528911400bbaf2fc9d9fc`  
		Last Modified: Wed, 11 Mar 2020 01:16:32 GMT  
		Size: 1.9 MB (1890930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a4b668572d274ff9367bfbef67a9bc3019ea12fc2a58ea82a0eea5b285eff6`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129d92a5515d89654fe39e14ae01a7ca45c43f3c384eda886f7cd4890a39aba4`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fedfc2f69a3a7fdcd3304d490f66dafb8a602d0237cc37115a420f3d0d1b39`  
		Last Modified: Wed, 11 Mar 2020 01:48:05 GMT  
		Size: 133.9 MB (133861603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2432ae9ed707294c44ebb22b4ae0a84dc1cea08f048c5bc14c6624d4b2491501`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:733ded7baf5291bcb8705d08b37c71dcd350b1908fafcc31b17da63810642269
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.8 MB (164753015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9ee5528cb767a9658228f1568269c7e9e1bd2c5988eed7626a141609dc784f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:38:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:38:59 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:39:06 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 04:50:08 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 10 Mar 2020 23:55:19 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:11:34 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:11:37 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:11:37 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:11:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:11:39 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:11:51 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:11:52 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 00:46:10 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 00:46:11 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 00:46:13 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 00:46:13 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:05:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:05:54 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:05:55 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 01:05:56 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:05:58 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:05:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:05:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:06:00 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a761fb3a5329492c5833bf26b25380ceb0c5243bea653014c9e329fd6901d4a`  
		Last Modified: Sat, 18 Jan 2020 05:43:45 GMT  
		Size: 301.6 KB (301623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ff232bcbce1b952dce3fb1514e26139d4b21a75ef45ab03adf8b3cf16267d9`  
		Last Modified: Wed, 11 Mar 2020 00:28:17 GMT  
		Size: 26.6 MB (26631625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f767fb3cf30af8ed99f6d09de819fa937560cbb3a6d9d9f529b14e4fd273861`  
		Last Modified: Wed, 11 Mar 2020 00:28:07 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e981cab0ab9d602e6cda10e0ebe660effacb6568e23deaaf3762f291e3f091`  
		Last Modified: Wed, 11 Mar 2020 00:28:08 GMT  
		Size: 1.9 MB (1891153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8b4e82b96c780400c428a78f8d81a94fc3ec626dd615eec7ce597bedae4662`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a17fa2cd2cece0abc3cda884ab354878c14621bf6b8723908915cf6f1145771`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aaaf98029b25c2b64b2489034ee2b4f43ddcafb223027120dcaacd032c47194`  
		Last Modified: Wed, 11 Mar 2020 01:07:13 GMT  
		Size: 133.3 MB (133305793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89ab1b02c65c97f665ba6c4ad2119f8425716d6fdc30f4eb946120536580252`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 2.6 KB (2623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:f3f037db79cf64c39db3d599890cbe45a8f8a7167b1634ea17f0a42d4c1b4105
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.7 MB (166671522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a31999e3cdd98ef95738ba5a22ba6e22d5c94e959a3ed4eeb5907168d686e71`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:23:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:23:12 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 03:23:14 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 03:31:26 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:32:45 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:46:21 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:46:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:46:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:46:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:46:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:46:35 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:46:36 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:33:49 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:33:50 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:33:52 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:33:52 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:52:02 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:52:10 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:52:11 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:52:12 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:52:13 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:52:14 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:52:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:52:15 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323ef8020b66a82bff905b3b8da692d6daf69a17f2740337bd5dde99dfe6da5`  
		Last Modified: Sat, 18 Jan 2020 04:18:27 GMT  
		Size: 301.8 KB (301758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ae6db3fff2d501fd9a1588acc79b2d1979a2a85c0dcd74a319491a1a58b7c6`  
		Last Modified: Wed, 11 Mar 2020 02:04:08 GMT  
		Size: 28.2 MB (28152901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45080882b2e9e075b004193066447a213219648430fa7e4c55b2ab9c6b9a3826`  
		Last Modified: Wed, 11 Mar 2020 02:03:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2e226b432b6eddbc490b8471084c95d5a59dae345fa3c2885fdb08d6a65433`  
		Last Modified: Wed, 11 Mar 2020 02:03:59 GMT  
		Size: 1.9 MB (1891200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e625dccbc4bcb58d7656906703e8e5f06d79429f7b81d2b96ff04cae9837732f`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c2281e9cd39ddddc9657eb2933dfe185eb25f55e43684895bd36e8a88c8583`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac109756fff8eaf85044f6b348e8b45a5eb69b8682427cdf4cca8964a289bb2a`  
		Last Modified: Wed, 11 Mar 2020 02:54:23 GMT  
		Size: 133.6 MB (133597324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffc241cb3a360c66b800938870f75ca9a93ea857c9167f64be480e2dfc8b356`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-alpine` - linux; 386

```console
$ docker pull plone@sha256:96eee82b92d5510c4995f0407bfdbfd0cfe125081a0627717fc2ae1b18f38aa9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.4 MB (165403033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6692c859cb160cb2c7f275d367a860b482904d3b2513e66796ac164b57ec94`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:56:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 01:56:40 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 01:56:42 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 02:07:04 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:26:52 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:36:43 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:36:44 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:36:44 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:36:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:36:45 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:36:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:36:53 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:10:06 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:10:06 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:10:07 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:10:07 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:20:18 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:20:19 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:20:20 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:20:20 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:20:20 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:20:20 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:20:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:20:21 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bb66073d5c36a76368a9927f9e38d96d7f925b38af3fb4396b94e6e7a3a309`  
		Last Modified: Sat, 18 Jan 2020 05:37:35 GMT  
		Size: 301.9 KB (301915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91978cf8e552dc424fe9c7a0e279d06d85b0d8cd8ecb407fcbf1d4e6a5dc743`  
		Last Modified: Wed, 11 Mar 2020 01:50:12 GMT  
		Size: 27.1 MB (27101747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07420e8869fa8e2b11ba9b9ab6a81c54856f9ed3b85f885ec3b9ecc919509da2`  
		Last Modified: Wed, 11 Mar 2020 01:50:06 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95c379d154581bc5f5429c792cb92f3a67c45bd027bf4130cb67a4e81ca90e7`  
		Last Modified: Wed, 11 Mar 2020 01:50:06 GMT  
		Size: 1.9 MB (1890900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc3dc2bbf9b0e01f46c33752dbbf0861abd02214f0fa4c0f527d43d3185957d`  
		Last Modified: Wed, 11 Mar 2020 02:21:22 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9ae7fdbd0b57d5d5fc3571571121f23c7a72fe7bfa8ea007eea322e83e4792`  
		Last Modified: Wed, 11 Mar 2020 02:21:23 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcca93f91c8cf90ee1468f466b73db05b55b09520a045b2843a4fdfd30710b93`  
		Last Modified: Wed, 11 Mar 2020 02:21:57 GMT  
		Size: 133.3 MB (133296714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47476cde9a33c03b602fee9920dfeeec484c0f4e36d7fe94421ec7bdfe33bec7`  
		Last Modified: Wed, 11 Mar 2020 02:21:22 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:5091df027d694226adf6599fa2b46749049efb65c6d0f421c54ed692a134b881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (168951697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50cb00ee5f8cd912f11c217ae2f432513342ed9c3d563ae94409789a384e5a2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:57:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:57:42 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:57:48 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 05:06:31 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:22:59 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:35:08 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:35:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:35:20 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:35:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:35:24 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:35:39 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:35:43 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:35:36 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:35:39 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:35:46 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:35:47 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:53:22 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:53:31 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:53:34 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:53:37 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:53:41 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:53:44 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:53:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:53:58 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83d4344e21f41e55783663900e987c11ef2a6b1168de19ae63f1e05009e4eae`  
		Last Modified: Sat, 18 Jan 2020 05:45:37 GMT  
		Size: 304.0 KB (303987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997052e9d9d744aba0e068db207eeb61eaa721ae09904ce3c203df4e1088408`  
		Last Modified: Wed, 11 Mar 2020 01:52:37 GMT  
		Size: 29.6 MB (29601503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76109d56f0386d8030cb0e3532a1aba32698bda6498c8b8f0e47b733d34b54`  
		Last Modified: Wed, 11 Mar 2020 01:52:29 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0027cf2e6261a311500aab624108c2403b01d6100404370e3b5cfa3e759597fd`  
		Last Modified: Wed, 11 Mar 2020 01:52:30 GMT  
		Size: 1.9 MB (1891099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5a4297dc1e9435d804b5af7fc2cbac58ddc1af9eeab0b3cb1b94369e440f97`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4951daf23dd61a7c9e21936160861cddcd504308e04a4ca81f9952abcc6814e3`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c9333a69e536301bd60e001f4e5b88c7fb88e7fa6bc624409395bb5a208fe4`  
		Last Modified: Wed, 11 Mar 2020 02:56:33 GMT  
		Size: 134.3 MB (134327723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b7eac9ab10fddc9dba9ec26c3cd340093aff28eac163a2cbe57067ebdbbabe`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-alpine` - linux; s390x

```console
$ docker pull plone@sha256:3589edb381d0570ac641b4a8d0a8cd0a493e7285eac9275e4e22a46da86ed2c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167893238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc12fdb7579ed701d648ffc9ea4636149346b699cc98589581a2769ffbfcae12`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:52:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 01:52:22 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 01:52:23 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 01:56:48 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 18 Jan 2020 01:56:48 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:02:26 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:02:26 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:52:22 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 00:49:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 00:49:26 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 00:49:30 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 00:49:31 GMT
CMD ["python3"]
# Fri, 06 Mar 2020 23:30:07 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 06 Mar 2020 23:30:07 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 06 Mar 2020 23:30:09 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 06 Mar 2020 23:30:10 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 06 Mar 2020 23:37:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Fri, 06 Mar 2020 23:38:23 GMT
VOLUME [/data]
# Fri, 06 Mar 2020 23:38:23 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Fri, 06 Mar 2020 23:38:24 GMT
EXPOSE 8080
# Fri, 06 Mar 2020 23:38:25 GMT
WORKDIR /plone/instance
# Fri, 06 Mar 2020 23:38:25 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 06 Mar 2020 23:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 06 Mar 2020 23:38:27 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2a03efad4a7a2934aa60870dd9847c7c02f10dcbbd1614ea32e83c78531ba2`  
		Last Modified: Sat, 18 Jan 2020 02:16:42 GMT  
		Size: 301.8 KB (301798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0627e873630aec7205c7b8e4f1025c14b29c11134532107ac214bb0646e89ad`  
		Last Modified: Sat, 18 Jan 2020 02:17:03 GMT  
		Size: 28.9 MB (28940433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1052253c74f387f87f6ac8e43dc4e0dbc66ee4ea50dc26d9b6bb9bce0415d7`  
		Last Modified: Sat, 18 Jan 2020 02:16:58 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406603440045cdce1ff839ea8eb3f9ebf716cd7daa1977ac349b7c8cbfd3098`  
		Last Modified: Thu, 06 Feb 2020 00:55:22 GMT  
		Size: 1.9 MB (1892187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89906eb9051286a6f61393b0fdc29cbe1a319a8e92321e967e25f372742aae6`  
		Last Modified: Fri, 06 Mar 2020 23:58:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071ee2dd5709fd6ed2a54c89001cf1f401de53a1c1dd8b885a37d59faa24a14c`  
		Last Modified: Fri, 06 Mar 2020 23:58:06 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f47382a3d80c83b2459b21f836eff7cbce5b520f1a972fbdf10d1bbf0f89f2`  
		Last Modified: Fri, 06 Mar 2020 23:58:42 GMT  
		Size: 134.2 MB (134171528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279fcc4ee668ab6054f985db3e9340958850e39f68c4384f63e86ce447df4a0b`  
		Last Modified: Fri, 06 Mar 2020 23:58:36 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2.1-python2`

```console
$ docker pull plone@sha256:aa15d492392c7f979a6fc51e6a45346c2efc99ca569901a77e8b366159752194
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `plone:5.2.1-python2` - linux; amd64

```console
$ docker pull plone@sha256:540d65605e99cbe77e3b24e19685caade491bbcf2bfa487b4518139926b1224d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.1 MB (204072220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da38b5ff841e0e4c692d310295c9067737225a614f460277a26956e93069524a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:35:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:35:17 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 17:36:54 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 17:37:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 17:37:03 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 17:37:03 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 17:44:49 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 17:44:49 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 17:44:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 17:44:50 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 17:45:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 17:45:11 GMT
CMD ["python2"]
# Thu, 27 Feb 2020 05:51:54 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 05:51:54 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 05:51:55 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 05:51:55 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 05:55:18 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 05:55:19 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 05:55:20 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 05:55:20 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 05:55:20 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 05:55:20 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 05:55:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 05:55:21 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc9812e632c6d6ab24bab1e95a31e23ab58ad0bf16eb02f0bfe83eedfde451`  
		Last Modified: Wed, 26 Feb 2020 17:51:28 GMT  
		Size: 2.5 MB (2531126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf60c41eb44a406e9849ec135ae509def6f28fb268aa804c27318320f5d1ad45`  
		Last Modified: Wed, 26 Feb 2020 17:51:33 GMT  
		Size: 18.3 MB (18299655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0afc907c6427941de6a92e5ed45ee6a85da6d712f797ccf9d82dc212d4871e`  
		Last Modified: Wed, 26 Feb 2020 17:51:29 GMT  
		Size: 2.2 MB (2171134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2714e3e3ecaf0cc6c8baedae8713b12db112272b8c0740ea93baa0d44de301ae`  
		Last Modified: Thu, 27 Feb 2020 05:56:04 GMT  
		Size: 3.9 KB (3881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3c44b94b47ff3a4e16f6ff5927c38957d1acd89db27beea470de0783f171f6`  
		Last Modified: Thu, 27 Feb 2020 05:56:04 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9900cabad2c07f45a974670fb9b1dd74765736780a88d86885ef7d5780654c0`  
		Last Modified: Thu, 27 Feb 2020 05:56:33 GMT  
		Size: 158.5 MB (158549398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f334620302933ae284104cb42c85092ec4a83bcf93491ca14061bc79547b3b76`  
		Last Modified: Thu, 27 Feb 2020 05:56:04 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-python2` - linux; arm variant v5

```console
$ docker pull plone@sha256:a1e8e5c5d0043c7abd4b3bf2f26f8abfca1c9b3c04161dda9486889e1d67a001
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198319056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23ae273d660f75adb8e9152eb0898d7d3b9d82a8f9f37c3aa0a497d9e97ebe44`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:53:47 GMT
ADD file:3fa7d31ad19db7be28acd7abacb98667f814acaf8ef495a9abb855abe19c351d in / 
# Wed, 26 Feb 2020 00:53:52 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:42:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 07:42:51 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 09:38:22 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 09:38:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 09:38:40 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 09:38:40 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 09:49:03 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 09:49:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 09:49:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 09:49:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 09:49:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 09:49:41 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 16:50:19 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 16:50:20 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 16:50:21 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 16:50:22 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 17:04:44 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 17:04:52 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 17:04:53 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 17:04:54 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 17:04:54 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 17:04:55 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 17:04:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 17:04:56 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8b6b97522cf0c1b41e02f7a9de64e8eb22bf8ff5c5ae70bbb46c20761af19aff`  
		Last Modified: Wed, 26 Feb 2020 01:03:39 GMT  
		Size: 21.2 MB (21190915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b73943cef5202f8e4dd87696f8e23ffcc73285ff563bd9d93225e77386cc22`  
		Last Modified: Wed, 26 Feb 2020 09:55:25 GMT  
		Size: 2.3 MB (2256550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4665b8b9f4fe07f77f52c530fb25596c8630a917915135e5bf49d8062c4642`  
		Last Modified: Wed, 26 Feb 2020 09:55:31 GMT  
		Size: 17.2 MB (17210295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50406ea4007f79f7a05b48720d7c9b304b6dbb8d098976d8d51da749c89fff9`  
		Last Modified: Wed, 26 Feb 2020 09:55:26 GMT  
		Size: 2.2 MB (2171005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058eac253fa9aad07df17afa5ac99a80770c0c81cc43d9b520a0da588d17d656`  
		Last Modified: Wed, 26 Feb 2020 17:06:17 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846a165f4392d0ea14c9b42704daee0fe3933c34c49606b314faf2deeb4fb57d`  
		Last Modified: Wed, 26 Feb 2020 17:06:17 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0ae4d84ddf208f6c23c317ed4dcde434a59ec79015798458584e1f6b2f0fc8`  
		Last Modified: Wed, 26 Feb 2020 17:07:18 GMT  
		Size: 155.5 MB (155482703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ad5352975d66571cbbdd6121f8af9ca22882ebbdca9b753e6aaa7bd9ace25b`  
		Last Modified: Wed, 26 Feb 2020 17:06:17 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-python2` - linux; arm variant v7

```console
$ docker pull plone@sha256:9e9a3ad31d4d07f21f25816373f818dc88f9edb02054f1a2f7e5f9a78bed80f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194582684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6bc4b60a8df1efaf7e4338984b96e952af03bd6f85d953de399e684460fd085`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 10:10:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 10:10:05 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 12:12:58 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 12:13:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 12:13:31 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 12:13:33 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 12:23:10 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 12:23:12 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 12:23:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 12:23:13 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 12:23:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 12:23:39 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 23:34:39 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 23:34:40 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 23:34:42 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 23:34:42 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 23:47:16 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 23:47:24 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 23:47:25 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 23:47:26 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 23:47:26 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 23:47:27 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 23:47:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 23:47:28 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a720c0b453d29444434cc1b23aab9aadfe64717e634abbdb60d08c44bf21f19c`  
		Last Modified: Wed, 26 Feb 2020 12:31:02 GMT  
		Size: 2.2 MB (2177999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655d6d48ec871b22d20195af872e0f2a0b502067f01c7998036793680ea6f2b8`  
		Last Modified: Wed, 26 Feb 2020 12:31:06 GMT  
		Size: 16.8 MB (16755146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96468ee01cebaac4bbb9c22eb33c4617d11289115e5ce1a67cf00d61612e6b3`  
		Last Modified: Wed, 26 Feb 2020 12:31:02 GMT  
		Size: 2.2 MB (2170988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18cabd1fc64da1e26b24006e70e974292a199415c3daf589b87ff99c33b7bab`  
		Last Modified: Wed, 26 Feb 2020 23:48:47 GMT  
		Size: 3.9 KB (3924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f51c595b57a1c5596a7292eb97e9ecd9594b9ddb77a514575f6e5be309dac9`  
		Last Modified: Wed, 26 Feb 2020 23:48:48 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ed14888cba72d6da4de76321ad11239ab5b07c3881e5eb849ac766dc326980`  
		Last Modified: Wed, 26 Feb 2020 23:49:47 GMT  
		Size: 154.2 MB (154172617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e164c0b7a2e7e199999dbea53376badfe5bd4ab5679dc940cd09cda0269107bd`  
		Last Modified: Wed, 26 Feb 2020 23:48:48 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-python2` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:f38e7d0b4a24c62d87823ae50065eb3d397e302a897a6646a510de40b7dd524d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.5 MB (197456286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f491d504008f3377155b254e0ae3d9f3717c5e26d2f0731d6feec6f426b81f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 06:49:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 06:49:15 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 18:23:32 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 18:23:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 18:23:47 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 18:23:47 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 18:33:07 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 18:33:09 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 18:33:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 18:33:11 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 18:33:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 18:33:38 GMT
CMD ["python2"]
# Thu, 27 Feb 2020 04:26:39 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 04:26:39 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 04:26:41 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 04:26:42 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 04:39:50 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 04:39:57 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 04:39:58 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 04:39:59 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 04:40:00 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 04:40:00 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 04:40:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 04:40:01 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d99d50b39d76f3fd90dc0eaa7228df164554d76604a524b83002fc37567940`  
		Last Modified: Wed, 26 Feb 2020 18:41:04 GMT  
		Size: 2.2 MB (2238910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed173cf84106c21c4e733ad301f2dcf4b13fe58a2c45b67dc97f6bc53352ab2`  
		Last Modified: Wed, 26 Feb 2020 18:41:11 GMT  
		Size: 17.6 MB (17646664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828f5104cc6203db57f480c339442b7a7c4b9dc976fd4bb48c5964216e74e41e`  
		Last Modified: Wed, 26 Feb 2020 18:41:04 GMT  
		Size: 2.2 MB (2170904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a11f007ca466a7e2d873064418db96552c5239c9a562893d0d03a2cfaad2957`  
		Last Modified: Thu, 27 Feb 2020 04:41:27 GMT  
		Size: 3.9 KB (3941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9647f7696f2c1197e7e659e9bf35b7915d9d0109ba56ec295cf169c4a0031d1a`  
		Last Modified: Thu, 27 Feb 2020 04:41:27 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ebd14353d0b9fcd8141c4c2cc72e896bea1e9a1bc8cf7dbfff8b59011a1394`  
		Last Modified: Thu, 27 Feb 2020 04:42:17 GMT  
		Size: 155.0 MB (155022225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3bdfefd82cb56684e16783f17e4d3c5d0f57ee8cb1b7a50e7f43ec08e1cc34`  
		Last Modified: Thu, 27 Feb 2020 04:41:27 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-python2` - linux; 386

```console
$ docker pull plone@sha256:0cb8be1a109ca0c979b2a0542938d19f7b118f1a2395ff9821cd613f5a89c516
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203807104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:560c1eac7751356d6ace1226b7ea3eaaf53a5710445527e332d90027108ac65d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:35:41 GMT
ADD file:7d77438aab7eb35501c0d27bd4350a3a9b4fd1988ce7e7fc0670a570b3112590 in / 
# Wed, 26 Feb 2020 00:35:42 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:25:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 11:25:58 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 15:38:52 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 15:39:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 15:39:01 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 15:39:01 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 15:46:25 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 15:46:25 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 15:46:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 15:46:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 15:46:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 15:46:41 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 20:21:16 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 20:21:17 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 20:21:19 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 20:21:19 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 20:25:56 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 20:25:58 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 20:25:58 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 20:25:58 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 20:25:59 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 20:25:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 20:25:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 20:25:59 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:5cf237473070a9ef7639307699a23bb6c32cd8321bf84c0cf61b6f9c32b44341`  
		Last Modified: Wed, 26 Feb 2020 00:42:02 GMT  
		Size: 23.1 MB (23141399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2faea37536bb10c13dd52913b524ee145e30cc577f79e94229067fb7381a3366`  
		Last Modified: Wed, 26 Feb 2020 15:52:23 GMT  
		Size: 2.5 MB (2532882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65facf1ea86c567f91573ca42282f8f8104ce0654a00d0c146a6e57a494f04a5`  
		Last Modified: Wed, 26 Feb 2020 15:52:27 GMT  
		Size: 17.2 MB (17244731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82181b01888156e580308b59e5fdd7575df2a0b81e9302aba0e7111029e5637`  
		Last Modified: Wed, 26 Feb 2020 15:52:23 GMT  
		Size: 2.2 MB (2170928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ea53354456a39fd74c387b4c7c8b94a5d97c3324d9673f83df6770778ed76a`  
		Last Modified: Wed, 26 Feb 2020 20:27:24 GMT  
		Size: 3.9 KB (3875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc5b85da19d843ab0e464cb8b42aac8c847173f5cf4c10f89c090c3de32d466`  
		Last Modified: Wed, 26 Feb 2020 20:27:24 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee362b752174680d6e79255910f5b85d8f679597edb1babdd22bbf023ed0c9cb`  
		Last Modified: Wed, 26 Feb 2020 20:28:10 GMT  
		Size: 158.7 MB (158709624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19d233ccc6fd095b8c14398d4b2e18bc38faa4978ac1344092d017ff8340bd4`  
		Last Modified: Wed, 26 Feb 2020 20:27:24 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-python2` - linux; ppc64le

```console
$ docker pull plone@sha256:fabcbbd4ab3358248256c7fe286f1768d2bd7c3652cd90835ee0f94402d0caa3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.9 MB (201869896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e353f7045c5c12c6542c7bdfe883c6b89ef7fc01f67ab70b5a1760d2e8405ca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:37:18 GMT
ADD file:661513607cf6a4c5038d6048ea16a04dedb05c03ce6c0e33e409f51510562e11 in / 
# Wed, 26 Feb 2020 01:37:25 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:01:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 04:02:01 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 05:46:29 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 05:47:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 05:47:09 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 05:47:14 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 06:00:08 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 06:00:11 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 06:00:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 06:00:17 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 06:01:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 06:01:28 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 21:07:57 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 21:08:00 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 21:08:08 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 21:08:09 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 21:29:02 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 21:29:11 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 21:29:15 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 21:29:18 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 21:29:22 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 21:29:26 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 21:29:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 21:29:36 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:21d148b1dce5a6179231486bac7845a111bbaba4fcaf4232bbc39842bf6c5366`  
		Last Modified: Wed, 26 Feb 2020 02:04:13 GMT  
		Size: 22.8 MB (22785269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bc85883bb3736ef2e561ed5e633404a8dff44dd1d9bdf65d8899e44b3a6c6d`  
		Last Modified: Wed, 26 Feb 2020 06:07:34 GMT  
		Size: 2.2 MB (2192776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89deb8a33ea35dcfce45dc587a961eea14d457bbc18a95ffd09d4a5c52e90bab`  
		Last Modified: Wed, 26 Feb 2020 06:07:37 GMT  
		Size: 18.3 MB (18258209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7526c7803ffe676727247704b185a74b9487da6724dc2b3c13a8c37adc9cf7`  
		Last Modified: Wed, 26 Feb 2020 06:07:35 GMT  
		Size: 2.2 MB (2172157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7a26feed99ea23e7e263f6463d1fdb60afd5ba448faa4901a266a5f4965b3a`  
		Last Modified: Wed, 26 Feb 2020 21:34:37 GMT  
		Size: 3.9 KB (3939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1bbbdac1cfc4287d64f299478b23812c7b5d9d10cd2b9c61b5584317957bf5`  
		Last Modified: Wed, 26 Feb 2020 21:34:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f02f21529fbfc45364814399a298f42cf95ef952b5860ef8e1cdc63d2e702d`  
		Last Modified: Wed, 26 Feb 2020 21:38:36 GMT  
		Size: 156.5 MB (156453881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ce4caad5fefe888d2954f28c821862e7d900876801254337f439516deb7e3`  
		Last Modified: Wed, 26 Feb 2020 21:34:37 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2-alpine`

```console
$ docker pull plone@sha256:c8dc0c313bb90c1ea86d31758645c0b352053d9f1c316334580ee8faeb798e79
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
$ docker pull plone@sha256:0c096be1cf04c60572e92f6e048d48bc06b7aaf10ffc7603bc074339a2cd1202
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167524259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d110dfe8b84924bb805ca859c08c3e31a8423095de96fdc510da999ba8f3cd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:42:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 02:37:13 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 02:37:14 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 02:43:48 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:54:17 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:03:22 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:03:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:03:29 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:03:29 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:36:31 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:36:31 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:36:32 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:36:32 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:46:32 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:46:33 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:46:33 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 01:46:33 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:46:34 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:46:34 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:46:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:46:34 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5ad85d9abaadf23d5ae53c3f32e7ccb2df1956869980bfd2491ff396d348a`  
		Last Modified: Sat, 18 Jan 2020 03:11:07 GMT  
		Size: 301.3 KB (301261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29edaae8dc30d7fc1e5c9c5a016e604e4b7cb4f6c5ecb9a3db52ebfc239db28e`  
		Last Modified: Wed, 11 Mar 2020 01:16:37 GMT  
		Size: 28.7 MB (28662304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b1dc8253c8ff1738172bc5fdd061c70e30c965e11fd50436c2de192b80aaf`  
		Last Modified: Wed, 11 Mar 2020 01:16:31 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf370601a519cbf3f23c20bd5324374f3298a016e528911400bbaf2fc9d9fc`  
		Last Modified: Wed, 11 Mar 2020 01:16:32 GMT  
		Size: 1.9 MB (1890930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a4b668572d274ff9367bfbef67a9bc3019ea12fc2a58ea82a0eea5b285eff6`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129d92a5515d89654fe39e14ae01a7ca45c43f3c384eda886f7cd4890a39aba4`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fedfc2f69a3a7fdcd3304d490f66dafb8a602d0237cc37115a420f3d0d1b39`  
		Last Modified: Wed, 11 Mar 2020 01:48:05 GMT  
		Size: 133.9 MB (133861603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2432ae9ed707294c44ebb22b4ae0a84dc1cea08f048c5bc14c6624d4b2491501`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:733ded7baf5291bcb8705d08b37c71dcd350b1908fafcc31b17da63810642269
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.8 MB (164753015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9ee5528cb767a9658228f1568269c7e9e1bd2c5988eed7626a141609dc784f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:38:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:38:59 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:39:06 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 04:50:08 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 10 Mar 2020 23:55:19 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:11:34 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:11:37 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:11:37 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:11:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:11:39 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:11:51 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:11:52 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 00:46:10 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 00:46:11 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 00:46:13 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 00:46:13 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:05:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:05:54 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:05:55 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 01:05:56 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:05:58 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:05:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:05:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:06:00 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a761fb3a5329492c5833bf26b25380ceb0c5243bea653014c9e329fd6901d4a`  
		Last Modified: Sat, 18 Jan 2020 05:43:45 GMT  
		Size: 301.6 KB (301623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ff232bcbce1b952dce3fb1514e26139d4b21a75ef45ab03adf8b3cf16267d9`  
		Last Modified: Wed, 11 Mar 2020 00:28:17 GMT  
		Size: 26.6 MB (26631625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f767fb3cf30af8ed99f6d09de819fa937560cbb3a6d9d9f529b14e4fd273861`  
		Last Modified: Wed, 11 Mar 2020 00:28:07 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e981cab0ab9d602e6cda10e0ebe660effacb6568e23deaaf3762f291e3f091`  
		Last Modified: Wed, 11 Mar 2020 00:28:08 GMT  
		Size: 1.9 MB (1891153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8b4e82b96c780400c428a78f8d81a94fc3ec626dd615eec7ce597bedae4662`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a17fa2cd2cece0abc3cda884ab354878c14621bf6b8723908915cf6f1145771`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aaaf98029b25c2b64b2489034ee2b4f43ddcafb223027120dcaacd032c47194`  
		Last Modified: Wed, 11 Mar 2020 01:07:13 GMT  
		Size: 133.3 MB (133305793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89ab1b02c65c97f665ba6c4ad2119f8425716d6fdc30f4eb946120536580252`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 2.6 KB (2623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:f3f037db79cf64c39db3d599890cbe45a8f8a7167b1634ea17f0a42d4c1b4105
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.7 MB (166671522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a31999e3cdd98ef95738ba5a22ba6e22d5c94e959a3ed4eeb5907168d686e71`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:23:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:23:12 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 03:23:14 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 03:31:26 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:32:45 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:46:21 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:46:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:46:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:46:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:46:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:46:35 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:46:36 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:33:49 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:33:50 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:33:52 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:33:52 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:52:02 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:52:10 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:52:11 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:52:12 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:52:13 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:52:14 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:52:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:52:15 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323ef8020b66a82bff905b3b8da692d6daf69a17f2740337bd5dde99dfe6da5`  
		Last Modified: Sat, 18 Jan 2020 04:18:27 GMT  
		Size: 301.8 KB (301758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ae6db3fff2d501fd9a1588acc79b2d1979a2a85c0dcd74a319491a1a58b7c6`  
		Last Modified: Wed, 11 Mar 2020 02:04:08 GMT  
		Size: 28.2 MB (28152901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45080882b2e9e075b004193066447a213219648430fa7e4c55b2ab9c6b9a3826`  
		Last Modified: Wed, 11 Mar 2020 02:03:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2e226b432b6eddbc490b8471084c95d5a59dae345fa3c2885fdb08d6a65433`  
		Last Modified: Wed, 11 Mar 2020 02:03:59 GMT  
		Size: 1.9 MB (1891200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e625dccbc4bcb58d7656906703e8e5f06d79429f7b81d2b96ff04cae9837732f`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c2281e9cd39ddddc9657eb2933dfe185eb25f55e43684895bd36e8a88c8583`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac109756fff8eaf85044f6b348e8b45a5eb69b8682427cdf4cca8964a289bb2a`  
		Last Modified: Wed, 11 Mar 2020 02:54:23 GMT  
		Size: 133.6 MB (133597324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffc241cb3a360c66b800938870f75ca9a93ea857c9167f64be480e2dfc8b356`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; 386

```console
$ docker pull plone@sha256:96eee82b92d5510c4995f0407bfdbfd0cfe125081a0627717fc2ae1b18f38aa9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.4 MB (165403033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6692c859cb160cb2c7f275d367a860b482904d3b2513e66796ac164b57ec94`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:56:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 01:56:40 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 01:56:42 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 02:07:04 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:26:52 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:36:43 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:36:44 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:36:44 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:36:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:36:45 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:36:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:36:53 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:10:06 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:10:06 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:10:07 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:10:07 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:20:18 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:20:19 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:20:20 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:20:20 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:20:20 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:20:20 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:20:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:20:21 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bb66073d5c36a76368a9927f9e38d96d7f925b38af3fb4396b94e6e7a3a309`  
		Last Modified: Sat, 18 Jan 2020 05:37:35 GMT  
		Size: 301.9 KB (301915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91978cf8e552dc424fe9c7a0e279d06d85b0d8cd8ecb407fcbf1d4e6a5dc743`  
		Last Modified: Wed, 11 Mar 2020 01:50:12 GMT  
		Size: 27.1 MB (27101747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07420e8869fa8e2b11ba9b9ab6a81c54856f9ed3b85f885ec3b9ecc919509da2`  
		Last Modified: Wed, 11 Mar 2020 01:50:06 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95c379d154581bc5f5429c792cb92f3a67c45bd027bf4130cb67a4e81ca90e7`  
		Last Modified: Wed, 11 Mar 2020 01:50:06 GMT  
		Size: 1.9 MB (1890900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc3dc2bbf9b0e01f46c33752dbbf0861abd02214f0fa4c0f527d43d3185957d`  
		Last Modified: Wed, 11 Mar 2020 02:21:22 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9ae7fdbd0b57d5d5fc3571571121f23c7a72fe7bfa8ea007eea322e83e4792`  
		Last Modified: Wed, 11 Mar 2020 02:21:23 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcca93f91c8cf90ee1468f466b73db05b55b09520a045b2843a4fdfd30710b93`  
		Last Modified: Wed, 11 Mar 2020 02:21:57 GMT  
		Size: 133.3 MB (133296714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47476cde9a33c03b602fee9920dfeeec484c0f4e36d7fe94421ec7bdfe33bec7`  
		Last Modified: Wed, 11 Mar 2020 02:21:22 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:5091df027d694226adf6599fa2b46749049efb65c6d0f421c54ed692a134b881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (168951697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50cb00ee5f8cd912f11c217ae2f432513342ed9c3d563ae94409789a384e5a2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:57:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:57:42 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:57:48 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 05:06:31 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:22:59 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:35:08 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:35:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:35:20 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:35:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:35:24 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:35:39 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:35:43 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:35:36 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:35:39 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:35:46 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:35:47 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:53:22 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:53:31 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:53:34 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:53:37 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:53:41 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:53:44 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:53:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:53:58 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83d4344e21f41e55783663900e987c11ef2a6b1168de19ae63f1e05009e4eae`  
		Last Modified: Sat, 18 Jan 2020 05:45:37 GMT  
		Size: 304.0 KB (303987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997052e9d9d744aba0e068db207eeb61eaa721ae09904ce3c203df4e1088408`  
		Last Modified: Wed, 11 Mar 2020 01:52:37 GMT  
		Size: 29.6 MB (29601503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76109d56f0386d8030cb0e3532a1aba32698bda6498c8b8f0e47b733d34b54`  
		Last Modified: Wed, 11 Mar 2020 01:52:29 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0027cf2e6261a311500aab624108c2403b01d6100404370e3b5cfa3e759597fd`  
		Last Modified: Wed, 11 Mar 2020 01:52:30 GMT  
		Size: 1.9 MB (1891099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5a4297dc1e9435d804b5af7fc2cbac58ddc1af9eeab0b3cb1b94369e440f97`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4951daf23dd61a7c9e21936160861cddcd504308e04a4ca81f9952abcc6814e3`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c9333a69e536301bd60e001f4e5b88c7fb88e7fa6bc624409395bb5a208fe4`  
		Last Modified: Wed, 11 Mar 2020 02:56:33 GMT  
		Size: 134.3 MB (134327723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b7eac9ab10fddc9dba9ec26c3cd340093aff28eac163a2cbe57067ebdbbabe`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; s390x

```console
$ docker pull plone@sha256:3589edb381d0570ac641b4a8d0a8cd0a493e7285eac9275e4e22a46da86ed2c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167893238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc12fdb7579ed701d648ffc9ea4636149346b699cc98589581a2769ffbfcae12`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:52:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 01:52:22 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 01:52:23 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 01:56:48 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 18 Jan 2020 01:56:48 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:02:26 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:02:26 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:52:22 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 00:49:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 00:49:26 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 00:49:30 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 00:49:31 GMT
CMD ["python3"]
# Fri, 06 Mar 2020 23:30:07 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 06 Mar 2020 23:30:07 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 06 Mar 2020 23:30:09 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 06 Mar 2020 23:30:10 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 06 Mar 2020 23:37:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Fri, 06 Mar 2020 23:38:23 GMT
VOLUME [/data]
# Fri, 06 Mar 2020 23:38:23 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Fri, 06 Mar 2020 23:38:24 GMT
EXPOSE 8080
# Fri, 06 Mar 2020 23:38:25 GMT
WORKDIR /plone/instance
# Fri, 06 Mar 2020 23:38:25 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 06 Mar 2020 23:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 06 Mar 2020 23:38:27 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2a03efad4a7a2934aa60870dd9847c7c02f10dcbbd1614ea32e83c78531ba2`  
		Last Modified: Sat, 18 Jan 2020 02:16:42 GMT  
		Size: 301.8 KB (301798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0627e873630aec7205c7b8e4f1025c14b29c11134532107ac214bb0646e89ad`  
		Last Modified: Sat, 18 Jan 2020 02:17:03 GMT  
		Size: 28.9 MB (28940433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1052253c74f387f87f6ac8e43dc4e0dbc66ee4ea50dc26d9b6bb9bce0415d7`  
		Last Modified: Sat, 18 Jan 2020 02:16:58 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406603440045cdce1ff839ea8eb3f9ebf716cd7daa1977ac349b7c8cbfd3098`  
		Last Modified: Thu, 06 Feb 2020 00:55:22 GMT  
		Size: 1.9 MB (1892187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89906eb9051286a6f61393b0fdc29cbe1a319a8e92321e967e25f372742aae6`  
		Last Modified: Fri, 06 Mar 2020 23:58:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071ee2dd5709fd6ed2a54c89001cf1f401de53a1c1dd8b885a37d59faa24a14c`  
		Last Modified: Fri, 06 Mar 2020 23:58:06 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f47382a3d80c83b2459b21f836eff7cbce5b520f1a972fbdf10d1bbf0f89f2`  
		Last Modified: Fri, 06 Mar 2020 23:58:42 GMT  
		Size: 134.2 MB (134171528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279fcc4ee668ab6054f985db3e9340958850e39f68c4384f63e86ce447df4a0b`  
		Last Modified: Fri, 06 Mar 2020 23:58:36 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2-python2`

```console
$ docker pull plone@sha256:aa15d492392c7f979a6fc51e6a45346c2efc99ca569901a77e8b366159752194
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `plone:5.2-python2` - linux; amd64

```console
$ docker pull plone@sha256:540d65605e99cbe77e3b24e19685caade491bbcf2bfa487b4518139926b1224d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.1 MB (204072220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da38b5ff841e0e4c692d310295c9067737225a614f460277a26956e93069524a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:35:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:35:17 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 17:36:54 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 17:37:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 17:37:03 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 17:37:03 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 17:44:49 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 17:44:49 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 17:44:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 17:44:50 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 17:45:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 17:45:11 GMT
CMD ["python2"]
# Thu, 27 Feb 2020 05:51:54 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 05:51:54 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 05:51:55 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 05:51:55 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 05:55:18 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 05:55:19 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 05:55:20 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 05:55:20 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 05:55:20 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 05:55:20 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 05:55:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 05:55:21 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc9812e632c6d6ab24bab1e95a31e23ab58ad0bf16eb02f0bfe83eedfde451`  
		Last Modified: Wed, 26 Feb 2020 17:51:28 GMT  
		Size: 2.5 MB (2531126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf60c41eb44a406e9849ec135ae509def6f28fb268aa804c27318320f5d1ad45`  
		Last Modified: Wed, 26 Feb 2020 17:51:33 GMT  
		Size: 18.3 MB (18299655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0afc907c6427941de6a92e5ed45ee6a85da6d712f797ccf9d82dc212d4871e`  
		Last Modified: Wed, 26 Feb 2020 17:51:29 GMT  
		Size: 2.2 MB (2171134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2714e3e3ecaf0cc6c8baedae8713b12db112272b8c0740ea93baa0d44de301ae`  
		Last Modified: Thu, 27 Feb 2020 05:56:04 GMT  
		Size: 3.9 KB (3881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3c44b94b47ff3a4e16f6ff5927c38957d1acd89db27beea470de0783f171f6`  
		Last Modified: Thu, 27 Feb 2020 05:56:04 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9900cabad2c07f45a974670fb9b1dd74765736780a88d86885ef7d5780654c0`  
		Last Modified: Thu, 27 Feb 2020 05:56:33 GMT  
		Size: 158.5 MB (158549398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f334620302933ae284104cb42c85092ec4a83bcf93491ca14061bc79547b3b76`  
		Last Modified: Thu, 27 Feb 2020 05:56:04 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-python2` - linux; arm variant v5

```console
$ docker pull plone@sha256:a1e8e5c5d0043c7abd4b3bf2f26f8abfca1c9b3c04161dda9486889e1d67a001
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198319056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23ae273d660f75adb8e9152eb0898d7d3b9d82a8f9f37c3aa0a497d9e97ebe44`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:53:47 GMT
ADD file:3fa7d31ad19db7be28acd7abacb98667f814acaf8ef495a9abb855abe19c351d in / 
# Wed, 26 Feb 2020 00:53:52 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:42:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 07:42:51 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 09:38:22 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 09:38:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 09:38:40 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 09:38:40 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 09:49:03 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 09:49:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 09:49:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 09:49:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 09:49:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 09:49:41 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 16:50:19 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 16:50:20 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 16:50:21 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 16:50:22 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 17:04:44 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 17:04:52 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 17:04:53 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 17:04:54 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 17:04:54 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 17:04:55 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 17:04:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 17:04:56 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8b6b97522cf0c1b41e02f7a9de64e8eb22bf8ff5c5ae70bbb46c20761af19aff`  
		Last Modified: Wed, 26 Feb 2020 01:03:39 GMT  
		Size: 21.2 MB (21190915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b73943cef5202f8e4dd87696f8e23ffcc73285ff563bd9d93225e77386cc22`  
		Last Modified: Wed, 26 Feb 2020 09:55:25 GMT  
		Size: 2.3 MB (2256550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4665b8b9f4fe07f77f52c530fb25596c8630a917915135e5bf49d8062c4642`  
		Last Modified: Wed, 26 Feb 2020 09:55:31 GMT  
		Size: 17.2 MB (17210295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50406ea4007f79f7a05b48720d7c9b304b6dbb8d098976d8d51da749c89fff9`  
		Last Modified: Wed, 26 Feb 2020 09:55:26 GMT  
		Size: 2.2 MB (2171005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058eac253fa9aad07df17afa5ac99a80770c0c81cc43d9b520a0da588d17d656`  
		Last Modified: Wed, 26 Feb 2020 17:06:17 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846a165f4392d0ea14c9b42704daee0fe3933c34c49606b314faf2deeb4fb57d`  
		Last Modified: Wed, 26 Feb 2020 17:06:17 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0ae4d84ddf208f6c23c317ed4dcde434a59ec79015798458584e1f6b2f0fc8`  
		Last Modified: Wed, 26 Feb 2020 17:07:18 GMT  
		Size: 155.5 MB (155482703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ad5352975d66571cbbdd6121f8af9ca22882ebbdca9b753e6aaa7bd9ace25b`  
		Last Modified: Wed, 26 Feb 2020 17:06:17 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-python2` - linux; arm variant v7

```console
$ docker pull plone@sha256:9e9a3ad31d4d07f21f25816373f818dc88f9edb02054f1a2f7e5f9a78bed80f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194582684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6bc4b60a8df1efaf7e4338984b96e952af03bd6f85d953de399e684460fd085`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 10:10:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 10:10:05 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 12:12:58 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 12:13:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 12:13:31 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 12:13:33 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 12:23:10 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 12:23:12 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 12:23:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 12:23:13 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 12:23:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 12:23:39 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 23:34:39 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 23:34:40 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 23:34:42 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 23:34:42 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 23:47:16 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 23:47:24 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 23:47:25 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 23:47:26 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 23:47:26 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 23:47:27 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 23:47:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 23:47:28 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a720c0b453d29444434cc1b23aab9aadfe64717e634abbdb60d08c44bf21f19c`  
		Last Modified: Wed, 26 Feb 2020 12:31:02 GMT  
		Size: 2.2 MB (2177999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655d6d48ec871b22d20195af872e0f2a0b502067f01c7998036793680ea6f2b8`  
		Last Modified: Wed, 26 Feb 2020 12:31:06 GMT  
		Size: 16.8 MB (16755146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96468ee01cebaac4bbb9c22eb33c4617d11289115e5ce1a67cf00d61612e6b3`  
		Last Modified: Wed, 26 Feb 2020 12:31:02 GMT  
		Size: 2.2 MB (2170988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18cabd1fc64da1e26b24006e70e974292a199415c3daf589b87ff99c33b7bab`  
		Last Modified: Wed, 26 Feb 2020 23:48:47 GMT  
		Size: 3.9 KB (3924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f51c595b57a1c5596a7292eb97e9ecd9594b9ddb77a514575f6e5be309dac9`  
		Last Modified: Wed, 26 Feb 2020 23:48:48 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ed14888cba72d6da4de76321ad11239ab5b07c3881e5eb849ac766dc326980`  
		Last Modified: Wed, 26 Feb 2020 23:49:47 GMT  
		Size: 154.2 MB (154172617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e164c0b7a2e7e199999dbea53376badfe5bd4ab5679dc940cd09cda0269107bd`  
		Last Modified: Wed, 26 Feb 2020 23:48:48 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-python2` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:f38e7d0b4a24c62d87823ae50065eb3d397e302a897a6646a510de40b7dd524d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.5 MB (197456286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f491d504008f3377155b254e0ae3d9f3717c5e26d2f0731d6feec6f426b81f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 06:49:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 06:49:15 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 18:23:32 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 18:23:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 18:23:47 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 18:23:47 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 18:33:07 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 18:33:09 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 18:33:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 18:33:11 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 18:33:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 18:33:38 GMT
CMD ["python2"]
# Thu, 27 Feb 2020 04:26:39 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 04:26:39 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 04:26:41 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 04:26:42 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 04:39:50 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 04:39:57 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 04:39:58 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 04:39:59 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 04:40:00 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 04:40:00 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 04:40:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 04:40:01 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d99d50b39d76f3fd90dc0eaa7228df164554d76604a524b83002fc37567940`  
		Last Modified: Wed, 26 Feb 2020 18:41:04 GMT  
		Size: 2.2 MB (2238910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed173cf84106c21c4e733ad301f2dcf4b13fe58a2c45b67dc97f6bc53352ab2`  
		Last Modified: Wed, 26 Feb 2020 18:41:11 GMT  
		Size: 17.6 MB (17646664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828f5104cc6203db57f480c339442b7a7c4b9dc976fd4bb48c5964216e74e41e`  
		Last Modified: Wed, 26 Feb 2020 18:41:04 GMT  
		Size: 2.2 MB (2170904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a11f007ca466a7e2d873064418db96552c5239c9a562893d0d03a2cfaad2957`  
		Last Modified: Thu, 27 Feb 2020 04:41:27 GMT  
		Size: 3.9 KB (3941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9647f7696f2c1197e7e659e9bf35b7915d9d0109ba56ec295cf169c4a0031d1a`  
		Last Modified: Thu, 27 Feb 2020 04:41:27 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ebd14353d0b9fcd8141c4c2cc72e896bea1e9a1bc8cf7dbfff8b59011a1394`  
		Last Modified: Thu, 27 Feb 2020 04:42:17 GMT  
		Size: 155.0 MB (155022225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3bdfefd82cb56684e16783f17e4d3c5d0f57ee8cb1b7a50e7f43ec08e1cc34`  
		Last Modified: Thu, 27 Feb 2020 04:41:27 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-python2` - linux; 386

```console
$ docker pull plone@sha256:0cb8be1a109ca0c979b2a0542938d19f7b118f1a2395ff9821cd613f5a89c516
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203807104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:560c1eac7751356d6ace1226b7ea3eaaf53a5710445527e332d90027108ac65d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:35:41 GMT
ADD file:7d77438aab7eb35501c0d27bd4350a3a9b4fd1988ce7e7fc0670a570b3112590 in / 
# Wed, 26 Feb 2020 00:35:42 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:25:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 11:25:58 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 15:38:52 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 15:39:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 15:39:01 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 15:39:01 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 15:46:25 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 15:46:25 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 15:46:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 15:46:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 15:46:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 15:46:41 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 20:21:16 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 20:21:17 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 20:21:19 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 20:21:19 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 20:25:56 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 20:25:58 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 20:25:58 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 20:25:58 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 20:25:59 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 20:25:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 20:25:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 20:25:59 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:5cf237473070a9ef7639307699a23bb6c32cd8321bf84c0cf61b6f9c32b44341`  
		Last Modified: Wed, 26 Feb 2020 00:42:02 GMT  
		Size: 23.1 MB (23141399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2faea37536bb10c13dd52913b524ee145e30cc577f79e94229067fb7381a3366`  
		Last Modified: Wed, 26 Feb 2020 15:52:23 GMT  
		Size: 2.5 MB (2532882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65facf1ea86c567f91573ca42282f8f8104ce0654a00d0c146a6e57a494f04a5`  
		Last Modified: Wed, 26 Feb 2020 15:52:27 GMT  
		Size: 17.2 MB (17244731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82181b01888156e580308b59e5fdd7575df2a0b81e9302aba0e7111029e5637`  
		Last Modified: Wed, 26 Feb 2020 15:52:23 GMT  
		Size: 2.2 MB (2170928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ea53354456a39fd74c387b4c7c8b94a5d97c3324d9673f83df6770778ed76a`  
		Last Modified: Wed, 26 Feb 2020 20:27:24 GMT  
		Size: 3.9 KB (3875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc5b85da19d843ab0e464cb8b42aac8c847173f5cf4c10f89c090c3de32d466`  
		Last Modified: Wed, 26 Feb 2020 20:27:24 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee362b752174680d6e79255910f5b85d8f679597edb1babdd22bbf023ed0c9cb`  
		Last Modified: Wed, 26 Feb 2020 20:28:10 GMT  
		Size: 158.7 MB (158709624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19d233ccc6fd095b8c14398d4b2e18bc38faa4978ac1344092d017ff8340bd4`  
		Last Modified: Wed, 26 Feb 2020 20:27:24 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-python2` - linux; ppc64le

```console
$ docker pull plone@sha256:fabcbbd4ab3358248256c7fe286f1768d2bd7c3652cd90835ee0f94402d0caa3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.9 MB (201869896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e353f7045c5c12c6542c7bdfe883c6b89ef7fc01f67ab70b5a1760d2e8405ca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:37:18 GMT
ADD file:661513607cf6a4c5038d6048ea16a04dedb05c03ce6c0e33e409f51510562e11 in / 
# Wed, 26 Feb 2020 01:37:25 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:01:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 04:02:01 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 05:46:29 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 05:47:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 05:47:09 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 05:47:14 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 06:00:08 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 06:00:11 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 06:00:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 06:00:17 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 06:01:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 06:01:28 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 21:07:57 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 21:08:00 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 21:08:08 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 21:08:09 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 21:29:02 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 21:29:11 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 21:29:15 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 21:29:18 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 21:29:22 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 21:29:26 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 21:29:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 21:29:36 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:21d148b1dce5a6179231486bac7845a111bbaba4fcaf4232bbc39842bf6c5366`  
		Last Modified: Wed, 26 Feb 2020 02:04:13 GMT  
		Size: 22.8 MB (22785269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bc85883bb3736ef2e561ed5e633404a8dff44dd1d9bdf65d8899e44b3a6c6d`  
		Last Modified: Wed, 26 Feb 2020 06:07:34 GMT  
		Size: 2.2 MB (2192776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89deb8a33ea35dcfce45dc587a961eea14d457bbc18a95ffd09d4a5c52e90bab`  
		Last Modified: Wed, 26 Feb 2020 06:07:37 GMT  
		Size: 18.3 MB (18258209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7526c7803ffe676727247704b185a74b9487da6724dc2b3c13a8c37adc9cf7`  
		Last Modified: Wed, 26 Feb 2020 06:07:35 GMT  
		Size: 2.2 MB (2172157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7a26feed99ea23e7e263f6463d1fdb60afd5ba448faa4901a266a5f4965b3a`  
		Last Modified: Wed, 26 Feb 2020 21:34:37 GMT  
		Size: 3.9 KB (3939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1bbbdac1cfc4287d64f299478b23812c7b5d9d10cd2b9c61b5584317957bf5`  
		Last Modified: Wed, 26 Feb 2020 21:34:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f02f21529fbfc45364814399a298f42cf95ef952b5860ef8e1cdc63d2e702d`  
		Last Modified: Wed, 26 Feb 2020 21:38:36 GMT  
		Size: 156.5 MB (156453881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ce4caad5fefe888d2954f28c821862e7d900876801254337f439516deb7e3`  
		Last Modified: Wed, 26 Feb 2020 21:34:37 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5-alpine`

```console
$ docker pull plone@sha256:c8dc0c313bb90c1ea86d31758645c0b352053d9f1c316334580ee8faeb798e79
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
$ docker pull plone@sha256:0c096be1cf04c60572e92f6e048d48bc06b7aaf10ffc7603bc074339a2cd1202
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167524259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d110dfe8b84924bb805ca859c08c3e31a8423095de96fdc510da999ba8f3cd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:42:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 02:37:13 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 02:37:14 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 02:43:48 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:54:17 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:03:22 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:03:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:03:29 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:03:29 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:36:31 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:36:31 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:36:32 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:36:32 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:46:32 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:46:33 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:46:33 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 01:46:33 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:46:34 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:46:34 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:46:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:46:34 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5ad85d9abaadf23d5ae53c3f32e7ccb2df1956869980bfd2491ff396d348a`  
		Last Modified: Sat, 18 Jan 2020 03:11:07 GMT  
		Size: 301.3 KB (301261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29edaae8dc30d7fc1e5c9c5a016e604e4b7cb4f6c5ecb9a3db52ebfc239db28e`  
		Last Modified: Wed, 11 Mar 2020 01:16:37 GMT  
		Size: 28.7 MB (28662304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b1dc8253c8ff1738172bc5fdd061c70e30c965e11fd50436c2de192b80aaf`  
		Last Modified: Wed, 11 Mar 2020 01:16:31 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf370601a519cbf3f23c20bd5324374f3298a016e528911400bbaf2fc9d9fc`  
		Last Modified: Wed, 11 Mar 2020 01:16:32 GMT  
		Size: 1.9 MB (1890930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a4b668572d274ff9367bfbef67a9bc3019ea12fc2a58ea82a0eea5b285eff6`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129d92a5515d89654fe39e14ae01a7ca45c43f3c384eda886f7cd4890a39aba4`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fedfc2f69a3a7fdcd3304d490f66dafb8a602d0237cc37115a420f3d0d1b39`  
		Last Modified: Wed, 11 Mar 2020 01:48:05 GMT  
		Size: 133.9 MB (133861603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2432ae9ed707294c44ebb22b4ae0a84dc1cea08f048c5bc14c6624d4b2491501`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:733ded7baf5291bcb8705d08b37c71dcd350b1908fafcc31b17da63810642269
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.8 MB (164753015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9ee5528cb767a9658228f1568269c7e9e1bd2c5988eed7626a141609dc784f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:38:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:38:59 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:39:06 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 04:50:08 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 10 Mar 2020 23:55:19 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:11:34 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:11:37 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:11:37 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:11:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:11:39 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:11:51 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:11:52 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 00:46:10 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 00:46:11 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 00:46:13 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 00:46:13 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:05:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:05:54 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:05:55 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 01:05:56 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:05:58 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:05:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:05:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:06:00 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a761fb3a5329492c5833bf26b25380ceb0c5243bea653014c9e329fd6901d4a`  
		Last Modified: Sat, 18 Jan 2020 05:43:45 GMT  
		Size: 301.6 KB (301623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ff232bcbce1b952dce3fb1514e26139d4b21a75ef45ab03adf8b3cf16267d9`  
		Last Modified: Wed, 11 Mar 2020 00:28:17 GMT  
		Size: 26.6 MB (26631625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f767fb3cf30af8ed99f6d09de819fa937560cbb3a6d9d9f529b14e4fd273861`  
		Last Modified: Wed, 11 Mar 2020 00:28:07 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e981cab0ab9d602e6cda10e0ebe660effacb6568e23deaaf3762f291e3f091`  
		Last Modified: Wed, 11 Mar 2020 00:28:08 GMT  
		Size: 1.9 MB (1891153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8b4e82b96c780400c428a78f8d81a94fc3ec626dd615eec7ce597bedae4662`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a17fa2cd2cece0abc3cda884ab354878c14621bf6b8723908915cf6f1145771`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aaaf98029b25c2b64b2489034ee2b4f43ddcafb223027120dcaacd032c47194`  
		Last Modified: Wed, 11 Mar 2020 01:07:13 GMT  
		Size: 133.3 MB (133305793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89ab1b02c65c97f665ba6c4ad2119f8425716d6fdc30f4eb946120536580252`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 2.6 KB (2623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:f3f037db79cf64c39db3d599890cbe45a8f8a7167b1634ea17f0a42d4c1b4105
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.7 MB (166671522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a31999e3cdd98ef95738ba5a22ba6e22d5c94e959a3ed4eeb5907168d686e71`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:23:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:23:12 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 03:23:14 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 03:31:26 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:32:45 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:46:21 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:46:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:46:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:46:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:46:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:46:35 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:46:36 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:33:49 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:33:50 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:33:52 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:33:52 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:52:02 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:52:10 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:52:11 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:52:12 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:52:13 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:52:14 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:52:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:52:15 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323ef8020b66a82bff905b3b8da692d6daf69a17f2740337bd5dde99dfe6da5`  
		Last Modified: Sat, 18 Jan 2020 04:18:27 GMT  
		Size: 301.8 KB (301758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ae6db3fff2d501fd9a1588acc79b2d1979a2a85c0dcd74a319491a1a58b7c6`  
		Last Modified: Wed, 11 Mar 2020 02:04:08 GMT  
		Size: 28.2 MB (28152901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45080882b2e9e075b004193066447a213219648430fa7e4c55b2ab9c6b9a3826`  
		Last Modified: Wed, 11 Mar 2020 02:03:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2e226b432b6eddbc490b8471084c95d5a59dae345fa3c2885fdb08d6a65433`  
		Last Modified: Wed, 11 Mar 2020 02:03:59 GMT  
		Size: 1.9 MB (1891200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e625dccbc4bcb58d7656906703e8e5f06d79429f7b81d2b96ff04cae9837732f`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c2281e9cd39ddddc9657eb2933dfe185eb25f55e43684895bd36e8a88c8583`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac109756fff8eaf85044f6b348e8b45a5eb69b8682427cdf4cca8964a289bb2a`  
		Last Modified: Wed, 11 Mar 2020 02:54:23 GMT  
		Size: 133.6 MB (133597324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffc241cb3a360c66b800938870f75ca9a93ea857c9167f64be480e2dfc8b356`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; 386

```console
$ docker pull plone@sha256:96eee82b92d5510c4995f0407bfdbfd0cfe125081a0627717fc2ae1b18f38aa9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.4 MB (165403033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6692c859cb160cb2c7f275d367a860b482904d3b2513e66796ac164b57ec94`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:56:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 01:56:40 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 01:56:42 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 02:07:04 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:26:52 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:36:43 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:36:44 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:36:44 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:36:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:36:45 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:36:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:36:53 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:10:06 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:10:06 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:10:07 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:10:07 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:20:18 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:20:19 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:20:20 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:20:20 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:20:20 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:20:20 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:20:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:20:21 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bb66073d5c36a76368a9927f9e38d96d7f925b38af3fb4396b94e6e7a3a309`  
		Last Modified: Sat, 18 Jan 2020 05:37:35 GMT  
		Size: 301.9 KB (301915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91978cf8e552dc424fe9c7a0e279d06d85b0d8cd8ecb407fcbf1d4e6a5dc743`  
		Last Modified: Wed, 11 Mar 2020 01:50:12 GMT  
		Size: 27.1 MB (27101747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07420e8869fa8e2b11ba9b9ab6a81c54856f9ed3b85f885ec3b9ecc919509da2`  
		Last Modified: Wed, 11 Mar 2020 01:50:06 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95c379d154581bc5f5429c792cb92f3a67c45bd027bf4130cb67a4e81ca90e7`  
		Last Modified: Wed, 11 Mar 2020 01:50:06 GMT  
		Size: 1.9 MB (1890900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc3dc2bbf9b0e01f46c33752dbbf0861abd02214f0fa4c0f527d43d3185957d`  
		Last Modified: Wed, 11 Mar 2020 02:21:22 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9ae7fdbd0b57d5d5fc3571571121f23c7a72fe7bfa8ea007eea322e83e4792`  
		Last Modified: Wed, 11 Mar 2020 02:21:23 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcca93f91c8cf90ee1468f466b73db05b55b09520a045b2843a4fdfd30710b93`  
		Last Modified: Wed, 11 Mar 2020 02:21:57 GMT  
		Size: 133.3 MB (133296714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47476cde9a33c03b602fee9920dfeeec484c0f4e36d7fe94421ec7bdfe33bec7`  
		Last Modified: Wed, 11 Mar 2020 02:21:22 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:5091df027d694226adf6599fa2b46749049efb65c6d0f421c54ed692a134b881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (168951697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50cb00ee5f8cd912f11c217ae2f432513342ed9c3d563ae94409789a384e5a2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:57:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:57:42 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:57:48 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 05:06:31 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:22:59 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:35:08 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:35:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:35:20 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:35:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:35:24 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:35:39 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:35:43 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:35:36 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:35:39 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:35:46 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:35:47 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:53:22 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:53:31 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:53:34 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:53:37 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:53:41 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:53:44 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:53:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:53:58 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83d4344e21f41e55783663900e987c11ef2a6b1168de19ae63f1e05009e4eae`  
		Last Modified: Sat, 18 Jan 2020 05:45:37 GMT  
		Size: 304.0 KB (303987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997052e9d9d744aba0e068db207eeb61eaa721ae09904ce3c203df4e1088408`  
		Last Modified: Wed, 11 Mar 2020 01:52:37 GMT  
		Size: 29.6 MB (29601503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76109d56f0386d8030cb0e3532a1aba32698bda6498c8b8f0e47b733d34b54`  
		Last Modified: Wed, 11 Mar 2020 01:52:29 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0027cf2e6261a311500aab624108c2403b01d6100404370e3b5cfa3e759597fd`  
		Last Modified: Wed, 11 Mar 2020 01:52:30 GMT  
		Size: 1.9 MB (1891099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5a4297dc1e9435d804b5af7fc2cbac58ddc1af9eeab0b3cb1b94369e440f97`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4951daf23dd61a7c9e21936160861cddcd504308e04a4ca81f9952abcc6814e3`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c9333a69e536301bd60e001f4e5b88c7fb88e7fa6bc624409395bb5a208fe4`  
		Last Modified: Wed, 11 Mar 2020 02:56:33 GMT  
		Size: 134.3 MB (134327723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b7eac9ab10fddc9dba9ec26c3cd340093aff28eac163a2cbe57067ebdbbabe`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; s390x

```console
$ docker pull plone@sha256:3589edb381d0570ac641b4a8d0a8cd0a493e7285eac9275e4e22a46da86ed2c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167893238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc12fdb7579ed701d648ffc9ea4636149346b699cc98589581a2769ffbfcae12`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:52:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 01:52:22 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 01:52:23 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 01:56:48 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 18 Jan 2020 01:56:48 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:02:26 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:02:26 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:52:22 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 00:49:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 00:49:26 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 00:49:30 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 00:49:31 GMT
CMD ["python3"]
# Fri, 06 Mar 2020 23:30:07 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 06 Mar 2020 23:30:07 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 06 Mar 2020 23:30:09 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 06 Mar 2020 23:30:10 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 06 Mar 2020 23:37:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Fri, 06 Mar 2020 23:38:23 GMT
VOLUME [/data]
# Fri, 06 Mar 2020 23:38:23 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Fri, 06 Mar 2020 23:38:24 GMT
EXPOSE 8080
# Fri, 06 Mar 2020 23:38:25 GMT
WORKDIR /plone/instance
# Fri, 06 Mar 2020 23:38:25 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 06 Mar 2020 23:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 06 Mar 2020 23:38:27 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2a03efad4a7a2934aa60870dd9847c7c02f10dcbbd1614ea32e83c78531ba2`  
		Last Modified: Sat, 18 Jan 2020 02:16:42 GMT  
		Size: 301.8 KB (301798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0627e873630aec7205c7b8e4f1025c14b29c11134532107ac214bb0646e89ad`  
		Last Modified: Sat, 18 Jan 2020 02:17:03 GMT  
		Size: 28.9 MB (28940433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1052253c74f387f87f6ac8e43dc4e0dbc66ee4ea50dc26d9b6bb9bce0415d7`  
		Last Modified: Sat, 18 Jan 2020 02:16:58 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406603440045cdce1ff839ea8eb3f9ebf716cd7daa1977ac349b7c8cbfd3098`  
		Last Modified: Thu, 06 Feb 2020 00:55:22 GMT  
		Size: 1.9 MB (1892187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89906eb9051286a6f61393b0fdc29cbe1a319a8e92321e967e25f372742aae6`  
		Last Modified: Fri, 06 Mar 2020 23:58:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071ee2dd5709fd6ed2a54c89001cf1f401de53a1c1dd8b885a37d59faa24a14c`  
		Last Modified: Fri, 06 Mar 2020 23:58:06 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f47382a3d80c83b2459b21f836eff7cbce5b520f1a972fbdf10d1bbf0f89f2`  
		Last Modified: Fri, 06 Mar 2020 23:58:42 GMT  
		Size: 134.2 MB (134171528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279fcc4ee668ab6054f985db3e9340958850e39f68c4384f63e86ce447df4a0b`  
		Last Modified: Fri, 06 Mar 2020 23:58:36 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5-python2`

```console
$ docker pull plone@sha256:aa15d492392c7f979a6fc51e6a45346c2efc99ca569901a77e8b366159752194
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `plone:5-python2` - linux; amd64

```console
$ docker pull plone@sha256:540d65605e99cbe77e3b24e19685caade491bbcf2bfa487b4518139926b1224d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.1 MB (204072220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da38b5ff841e0e4c692d310295c9067737225a614f460277a26956e93069524a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:35:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:35:17 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 17:36:54 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 17:37:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 17:37:03 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 17:37:03 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 17:44:49 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 17:44:49 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 17:44:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 17:44:50 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 17:45:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 17:45:11 GMT
CMD ["python2"]
# Thu, 27 Feb 2020 05:51:54 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 05:51:54 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 05:51:55 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 05:51:55 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 05:55:18 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 05:55:19 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 05:55:20 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 05:55:20 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 05:55:20 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 05:55:20 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 05:55:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 05:55:21 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc9812e632c6d6ab24bab1e95a31e23ab58ad0bf16eb02f0bfe83eedfde451`  
		Last Modified: Wed, 26 Feb 2020 17:51:28 GMT  
		Size: 2.5 MB (2531126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf60c41eb44a406e9849ec135ae509def6f28fb268aa804c27318320f5d1ad45`  
		Last Modified: Wed, 26 Feb 2020 17:51:33 GMT  
		Size: 18.3 MB (18299655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0afc907c6427941de6a92e5ed45ee6a85da6d712f797ccf9d82dc212d4871e`  
		Last Modified: Wed, 26 Feb 2020 17:51:29 GMT  
		Size: 2.2 MB (2171134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2714e3e3ecaf0cc6c8baedae8713b12db112272b8c0740ea93baa0d44de301ae`  
		Last Modified: Thu, 27 Feb 2020 05:56:04 GMT  
		Size: 3.9 KB (3881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3c44b94b47ff3a4e16f6ff5927c38957d1acd89db27beea470de0783f171f6`  
		Last Modified: Thu, 27 Feb 2020 05:56:04 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9900cabad2c07f45a974670fb9b1dd74765736780a88d86885ef7d5780654c0`  
		Last Modified: Thu, 27 Feb 2020 05:56:33 GMT  
		Size: 158.5 MB (158549398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f334620302933ae284104cb42c85092ec4a83bcf93491ca14061bc79547b3b76`  
		Last Modified: Thu, 27 Feb 2020 05:56:04 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-python2` - linux; arm variant v5

```console
$ docker pull plone@sha256:a1e8e5c5d0043c7abd4b3bf2f26f8abfca1c9b3c04161dda9486889e1d67a001
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198319056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23ae273d660f75adb8e9152eb0898d7d3b9d82a8f9f37c3aa0a497d9e97ebe44`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:53:47 GMT
ADD file:3fa7d31ad19db7be28acd7abacb98667f814acaf8ef495a9abb855abe19c351d in / 
# Wed, 26 Feb 2020 00:53:52 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:42:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 07:42:51 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 09:38:22 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 09:38:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 09:38:40 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 09:38:40 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 09:49:03 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 09:49:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 09:49:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 09:49:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 09:49:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 09:49:41 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 16:50:19 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 16:50:20 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 16:50:21 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 16:50:22 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 17:04:44 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 17:04:52 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 17:04:53 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 17:04:54 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 17:04:54 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 17:04:55 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 17:04:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 17:04:56 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8b6b97522cf0c1b41e02f7a9de64e8eb22bf8ff5c5ae70bbb46c20761af19aff`  
		Last Modified: Wed, 26 Feb 2020 01:03:39 GMT  
		Size: 21.2 MB (21190915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b73943cef5202f8e4dd87696f8e23ffcc73285ff563bd9d93225e77386cc22`  
		Last Modified: Wed, 26 Feb 2020 09:55:25 GMT  
		Size: 2.3 MB (2256550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4665b8b9f4fe07f77f52c530fb25596c8630a917915135e5bf49d8062c4642`  
		Last Modified: Wed, 26 Feb 2020 09:55:31 GMT  
		Size: 17.2 MB (17210295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50406ea4007f79f7a05b48720d7c9b304b6dbb8d098976d8d51da749c89fff9`  
		Last Modified: Wed, 26 Feb 2020 09:55:26 GMT  
		Size: 2.2 MB (2171005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058eac253fa9aad07df17afa5ac99a80770c0c81cc43d9b520a0da588d17d656`  
		Last Modified: Wed, 26 Feb 2020 17:06:17 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846a165f4392d0ea14c9b42704daee0fe3933c34c49606b314faf2deeb4fb57d`  
		Last Modified: Wed, 26 Feb 2020 17:06:17 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0ae4d84ddf208f6c23c317ed4dcde434a59ec79015798458584e1f6b2f0fc8`  
		Last Modified: Wed, 26 Feb 2020 17:07:18 GMT  
		Size: 155.5 MB (155482703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ad5352975d66571cbbdd6121f8af9ca22882ebbdca9b753e6aaa7bd9ace25b`  
		Last Modified: Wed, 26 Feb 2020 17:06:17 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-python2` - linux; arm variant v7

```console
$ docker pull plone@sha256:9e9a3ad31d4d07f21f25816373f818dc88f9edb02054f1a2f7e5f9a78bed80f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194582684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6bc4b60a8df1efaf7e4338984b96e952af03bd6f85d953de399e684460fd085`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 10:10:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 10:10:05 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 12:12:58 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 12:13:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 12:13:31 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 12:13:33 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 12:23:10 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 12:23:12 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 12:23:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 12:23:13 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 12:23:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 12:23:39 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 23:34:39 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 23:34:40 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 23:34:42 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 23:34:42 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 23:47:16 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 23:47:24 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 23:47:25 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 23:47:26 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 23:47:26 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 23:47:27 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 23:47:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 23:47:28 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a720c0b453d29444434cc1b23aab9aadfe64717e634abbdb60d08c44bf21f19c`  
		Last Modified: Wed, 26 Feb 2020 12:31:02 GMT  
		Size: 2.2 MB (2177999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655d6d48ec871b22d20195af872e0f2a0b502067f01c7998036793680ea6f2b8`  
		Last Modified: Wed, 26 Feb 2020 12:31:06 GMT  
		Size: 16.8 MB (16755146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96468ee01cebaac4bbb9c22eb33c4617d11289115e5ce1a67cf00d61612e6b3`  
		Last Modified: Wed, 26 Feb 2020 12:31:02 GMT  
		Size: 2.2 MB (2170988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18cabd1fc64da1e26b24006e70e974292a199415c3daf589b87ff99c33b7bab`  
		Last Modified: Wed, 26 Feb 2020 23:48:47 GMT  
		Size: 3.9 KB (3924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f51c595b57a1c5596a7292eb97e9ecd9594b9ddb77a514575f6e5be309dac9`  
		Last Modified: Wed, 26 Feb 2020 23:48:48 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ed14888cba72d6da4de76321ad11239ab5b07c3881e5eb849ac766dc326980`  
		Last Modified: Wed, 26 Feb 2020 23:49:47 GMT  
		Size: 154.2 MB (154172617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e164c0b7a2e7e199999dbea53376badfe5bd4ab5679dc940cd09cda0269107bd`  
		Last Modified: Wed, 26 Feb 2020 23:48:48 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-python2` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:f38e7d0b4a24c62d87823ae50065eb3d397e302a897a6646a510de40b7dd524d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.5 MB (197456286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f491d504008f3377155b254e0ae3d9f3717c5e26d2f0731d6feec6f426b81f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 06:49:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 06:49:15 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 18:23:32 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 18:23:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 18:23:47 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 18:23:47 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 18:33:07 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 18:33:09 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 18:33:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 18:33:11 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 18:33:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 18:33:38 GMT
CMD ["python2"]
# Thu, 27 Feb 2020 04:26:39 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 04:26:39 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 04:26:41 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 04:26:42 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 04:39:50 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 04:39:57 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 04:39:58 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 04:39:59 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 04:40:00 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 04:40:00 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 04:40:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 04:40:01 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d99d50b39d76f3fd90dc0eaa7228df164554d76604a524b83002fc37567940`  
		Last Modified: Wed, 26 Feb 2020 18:41:04 GMT  
		Size: 2.2 MB (2238910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed173cf84106c21c4e733ad301f2dcf4b13fe58a2c45b67dc97f6bc53352ab2`  
		Last Modified: Wed, 26 Feb 2020 18:41:11 GMT  
		Size: 17.6 MB (17646664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828f5104cc6203db57f480c339442b7a7c4b9dc976fd4bb48c5964216e74e41e`  
		Last Modified: Wed, 26 Feb 2020 18:41:04 GMT  
		Size: 2.2 MB (2170904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a11f007ca466a7e2d873064418db96552c5239c9a562893d0d03a2cfaad2957`  
		Last Modified: Thu, 27 Feb 2020 04:41:27 GMT  
		Size: 3.9 KB (3941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9647f7696f2c1197e7e659e9bf35b7915d9d0109ba56ec295cf169c4a0031d1a`  
		Last Modified: Thu, 27 Feb 2020 04:41:27 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ebd14353d0b9fcd8141c4c2cc72e896bea1e9a1bc8cf7dbfff8b59011a1394`  
		Last Modified: Thu, 27 Feb 2020 04:42:17 GMT  
		Size: 155.0 MB (155022225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3bdfefd82cb56684e16783f17e4d3c5d0f57ee8cb1b7a50e7f43ec08e1cc34`  
		Last Modified: Thu, 27 Feb 2020 04:41:27 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-python2` - linux; 386

```console
$ docker pull plone@sha256:0cb8be1a109ca0c979b2a0542938d19f7b118f1a2395ff9821cd613f5a89c516
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203807104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:560c1eac7751356d6ace1226b7ea3eaaf53a5710445527e332d90027108ac65d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:35:41 GMT
ADD file:7d77438aab7eb35501c0d27bd4350a3a9b4fd1988ce7e7fc0670a570b3112590 in / 
# Wed, 26 Feb 2020 00:35:42 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:25:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 11:25:58 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 15:38:52 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 15:39:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 15:39:01 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 15:39:01 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 15:46:25 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 15:46:25 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 15:46:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 15:46:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 15:46:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 15:46:41 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 20:21:16 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 20:21:17 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 20:21:19 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 20:21:19 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 20:25:56 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 20:25:58 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 20:25:58 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 20:25:58 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 20:25:59 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 20:25:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 20:25:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 20:25:59 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:5cf237473070a9ef7639307699a23bb6c32cd8321bf84c0cf61b6f9c32b44341`  
		Last Modified: Wed, 26 Feb 2020 00:42:02 GMT  
		Size: 23.1 MB (23141399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2faea37536bb10c13dd52913b524ee145e30cc577f79e94229067fb7381a3366`  
		Last Modified: Wed, 26 Feb 2020 15:52:23 GMT  
		Size: 2.5 MB (2532882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65facf1ea86c567f91573ca42282f8f8104ce0654a00d0c146a6e57a494f04a5`  
		Last Modified: Wed, 26 Feb 2020 15:52:27 GMT  
		Size: 17.2 MB (17244731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82181b01888156e580308b59e5fdd7575df2a0b81e9302aba0e7111029e5637`  
		Last Modified: Wed, 26 Feb 2020 15:52:23 GMT  
		Size: 2.2 MB (2170928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ea53354456a39fd74c387b4c7c8b94a5d97c3324d9673f83df6770778ed76a`  
		Last Modified: Wed, 26 Feb 2020 20:27:24 GMT  
		Size: 3.9 KB (3875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc5b85da19d843ab0e464cb8b42aac8c847173f5cf4c10f89c090c3de32d466`  
		Last Modified: Wed, 26 Feb 2020 20:27:24 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee362b752174680d6e79255910f5b85d8f679597edb1babdd22bbf023ed0c9cb`  
		Last Modified: Wed, 26 Feb 2020 20:28:10 GMT  
		Size: 158.7 MB (158709624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19d233ccc6fd095b8c14398d4b2e18bc38faa4978ac1344092d017ff8340bd4`  
		Last Modified: Wed, 26 Feb 2020 20:27:24 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-python2` - linux; ppc64le

```console
$ docker pull plone@sha256:fabcbbd4ab3358248256c7fe286f1768d2bd7c3652cd90835ee0f94402d0caa3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.9 MB (201869896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e353f7045c5c12c6542c7bdfe883c6b89ef7fc01f67ab70b5a1760d2e8405ca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:37:18 GMT
ADD file:661513607cf6a4c5038d6048ea16a04dedb05c03ce6c0e33e409f51510562e11 in / 
# Wed, 26 Feb 2020 01:37:25 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:01:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 04:02:01 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 05:46:29 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 05:47:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 05:47:09 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 05:47:14 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 06:00:08 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 06:00:11 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 06:00:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 06:00:17 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 06:01:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 06:01:28 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 21:07:57 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 21:08:00 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 21:08:08 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 21:08:09 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 21:29:02 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 21:29:11 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 21:29:15 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 21:29:18 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 21:29:22 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 21:29:26 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 21:29:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 21:29:36 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:21d148b1dce5a6179231486bac7845a111bbaba4fcaf4232bbc39842bf6c5366`  
		Last Modified: Wed, 26 Feb 2020 02:04:13 GMT  
		Size: 22.8 MB (22785269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bc85883bb3736ef2e561ed5e633404a8dff44dd1d9bdf65d8899e44b3a6c6d`  
		Last Modified: Wed, 26 Feb 2020 06:07:34 GMT  
		Size: 2.2 MB (2192776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89deb8a33ea35dcfce45dc587a961eea14d457bbc18a95ffd09d4a5c52e90bab`  
		Last Modified: Wed, 26 Feb 2020 06:07:37 GMT  
		Size: 18.3 MB (18258209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7526c7803ffe676727247704b185a74b9487da6724dc2b3c13a8c37adc9cf7`  
		Last Modified: Wed, 26 Feb 2020 06:07:35 GMT  
		Size: 2.2 MB (2172157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7a26feed99ea23e7e263f6463d1fdb60afd5ba448faa4901a266a5f4965b3a`  
		Last Modified: Wed, 26 Feb 2020 21:34:37 GMT  
		Size: 3.9 KB (3939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1bbbdac1cfc4287d64f299478b23812c7b5d9d10cd2b9c61b5584317957bf5`  
		Last Modified: Wed, 26 Feb 2020 21:34:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f02f21529fbfc45364814399a298f42cf95ef952b5860ef8e1cdc63d2e702d`  
		Last Modified: Wed, 26 Feb 2020 21:38:36 GMT  
		Size: 156.5 MB (156453881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ce4caad5fefe888d2954f28c821862e7d900876801254337f439516deb7e3`  
		Last Modified: Wed, 26 Feb 2020 21:34:37 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:alpine`

```console
$ docker pull plone@sha256:c8dc0c313bb90c1ea86d31758645c0b352053d9f1c316334580ee8faeb798e79
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
$ docker pull plone@sha256:0c096be1cf04c60572e92f6e048d48bc06b7aaf10ffc7603bc074339a2cd1202
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167524259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d110dfe8b84924bb805ca859c08c3e31a8423095de96fdc510da999ba8f3cd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:42:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 02:37:13 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 02:37:14 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 02:43:48 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:54:17 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:03:22 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:03:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:03:23 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:03:29 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:03:29 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:36:31 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:36:31 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:36:32 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:36:32 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:46:32 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:46:33 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:46:33 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 01:46:33 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:46:34 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:46:34 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:46:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:46:34 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5ad85d9abaadf23d5ae53c3f32e7ccb2df1956869980bfd2491ff396d348a`  
		Last Modified: Sat, 18 Jan 2020 03:11:07 GMT  
		Size: 301.3 KB (301261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29edaae8dc30d7fc1e5c9c5a016e604e4b7cb4f6c5ecb9a3db52ebfc239db28e`  
		Last Modified: Wed, 11 Mar 2020 01:16:37 GMT  
		Size: 28.7 MB (28662304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b1dc8253c8ff1738172bc5fdd061c70e30c965e11fd50436c2de192b80aaf`  
		Last Modified: Wed, 11 Mar 2020 01:16:31 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf370601a519cbf3f23c20bd5324374f3298a016e528911400bbaf2fc9d9fc`  
		Last Modified: Wed, 11 Mar 2020 01:16:32 GMT  
		Size: 1.9 MB (1890930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a4b668572d274ff9367bfbef67a9bc3019ea12fc2a58ea82a0eea5b285eff6`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129d92a5515d89654fe39e14ae01a7ca45c43f3c384eda886f7cd4890a39aba4`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fedfc2f69a3a7fdcd3304d490f66dafb8a602d0237cc37115a420f3d0d1b39`  
		Last Modified: Wed, 11 Mar 2020 01:48:05 GMT  
		Size: 133.9 MB (133861603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2432ae9ed707294c44ebb22b4ae0a84dc1cea08f048c5bc14c6624d4b2491501`  
		Last Modified: Wed, 11 Mar 2020 01:47:39 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:733ded7baf5291bcb8705d08b37c71dcd350b1908fafcc31b17da63810642269
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.8 MB (164753015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9ee5528cb767a9658228f1568269c7e9e1bd2c5988eed7626a141609dc784f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:38:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:38:59 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:39:06 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 04:50:08 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 10 Mar 2020 23:55:19 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:11:34 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:11:37 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:11:37 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:11:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:11:39 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:11:51 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:11:52 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 00:46:10 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 00:46:11 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 00:46:13 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 00:46:13 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:05:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:05:54 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:05:55 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 01:05:56 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:05:58 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:05:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:05:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:06:00 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a761fb3a5329492c5833bf26b25380ceb0c5243bea653014c9e329fd6901d4a`  
		Last Modified: Sat, 18 Jan 2020 05:43:45 GMT  
		Size: 301.6 KB (301623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ff232bcbce1b952dce3fb1514e26139d4b21a75ef45ab03adf8b3cf16267d9`  
		Last Modified: Wed, 11 Mar 2020 00:28:17 GMT  
		Size: 26.6 MB (26631625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f767fb3cf30af8ed99f6d09de819fa937560cbb3a6d9d9f529b14e4fd273861`  
		Last Modified: Wed, 11 Mar 2020 00:28:07 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e981cab0ab9d602e6cda10e0ebe660effacb6568e23deaaf3762f291e3f091`  
		Last Modified: Wed, 11 Mar 2020 00:28:08 GMT  
		Size: 1.9 MB (1891153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8b4e82b96c780400c428a78f8d81a94fc3ec626dd615eec7ce597bedae4662`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a17fa2cd2cece0abc3cda884ab354878c14621bf6b8723908915cf6f1145771`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aaaf98029b25c2b64b2489034ee2b4f43ddcafb223027120dcaacd032c47194`  
		Last Modified: Wed, 11 Mar 2020 01:07:13 GMT  
		Size: 133.3 MB (133305793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89ab1b02c65c97f665ba6c4ad2119f8425716d6fdc30f4eb946120536580252`  
		Last Modified: Wed, 11 Mar 2020 01:06:17 GMT  
		Size: 2.6 KB (2623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:f3f037db79cf64c39db3d599890cbe45a8f8a7167b1634ea17f0a42d4c1b4105
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.7 MB (166671522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a31999e3cdd98ef95738ba5a22ba6e22d5c94e959a3ed4eeb5907168d686e71`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:23:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:23:12 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 03:23:14 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 03:31:26 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:32:45 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:46:21 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:46:23 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:46:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:46:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:46:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:46:35 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:46:36 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:33:49 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:33:50 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:33:52 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:33:52 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:52:02 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:52:10 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:52:11 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:52:12 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:52:13 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:52:14 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:52:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:52:15 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323ef8020b66a82bff905b3b8da692d6daf69a17f2740337bd5dde99dfe6da5`  
		Last Modified: Sat, 18 Jan 2020 04:18:27 GMT  
		Size: 301.8 KB (301758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ae6db3fff2d501fd9a1588acc79b2d1979a2a85c0dcd74a319491a1a58b7c6`  
		Last Modified: Wed, 11 Mar 2020 02:04:08 GMT  
		Size: 28.2 MB (28152901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45080882b2e9e075b004193066447a213219648430fa7e4c55b2ab9c6b9a3826`  
		Last Modified: Wed, 11 Mar 2020 02:03:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2e226b432b6eddbc490b8471084c95d5a59dae345fa3c2885fdb08d6a65433`  
		Last Modified: Wed, 11 Mar 2020 02:03:59 GMT  
		Size: 1.9 MB (1891200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e625dccbc4bcb58d7656906703e8e5f06d79429f7b81d2b96ff04cae9837732f`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c2281e9cd39ddddc9657eb2933dfe185eb25f55e43684895bd36e8a88c8583`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac109756fff8eaf85044f6b348e8b45a5eb69b8682427cdf4cca8964a289bb2a`  
		Last Modified: Wed, 11 Mar 2020 02:54:23 GMT  
		Size: 133.6 MB (133597324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffc241cb3a360c66b800938870f75ca9a93ea857c9167f64be480e2dfc8b356`  
		Last Modified: Wed, 11 Mar 2020 02:53:37 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; 386

```console
$ docker pull plone@sha256:96eee82b92d5510c4995f0407bfdbfd0cfe125081a0627717fc2ae1b18f38aa9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.4 MB (165403033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6692c859cb160cb2c7f275d367a860b482904d3b2513e66796ac164b57ec94`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:56:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 01:56:40 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 01:56:42 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 02:07:04 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:26:52 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:36:43 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:36:44 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:36:44 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:36:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:36:45 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:36:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:36:53 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:10:06 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:10:06 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:10:07 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:10:07 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:20:18 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:20:19 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:20:20 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:20:20 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:20:20 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:20:20 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:20:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:20:21 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bb66073d5c36a76368a9927f9e38d96d7f925b38af3fb4396b94e6e7a3a309`  
		Last Modified: Sat, 18 Jan 2020 05:37:35 GMT  
		Size: 301.9 KB (301915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91978cf8e552dc424fe9c7a0e279d06d85b0d8cd8ecb407fcbf1d4e6a5dc743`  
		Last Modified: Wed, 11 Mar 2020 01:50:12 GMT  
		Size: 27.1 MB (27101747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07420e8869fa8e2b11ba9b9ab6a81c54856f9ed3b85f885ec3b9ecc919509da2`  
		Last Modified: Wed, 11 Mar 2020 01:50:06 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95c379d154581bc5f5429c792cb92f3a67c45bd027bf4130cb67a4e81ca90e7`  
		Last Modified: Wed, 11 Mar 2020 01:50:06 GMT  
		Size: 1.9 MB (1890900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc3dc2bbf9b0e01f46c33752dbbf0861abd02214f0fa4c0f527d43d3185957d`  
		Last Modified: Wed, 11 Mar 2020 02:21:22 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9ae7fdbd0b57d5d5fc3571571121f23c7a72fe7bfa8ea007eea322e83e4792`  
		Last Modified: Wed, 11 Mar 2020 02:21:23 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcca93f91c8cf90ee1468f466b73db05b55b09520a045b2843a4fdfd30710b93`  
		Last Modified: Wed, 11 Mar 2020 02:21:57 GMT  
		Size: 133.3 MB (133296714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47476cde9a33c03b602fee9920dfeeec484c0f4e36d7fe94421ec7bdfe33bec7`  
		Last Modified: Wed, 11 Mar 2020 02:21:22 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:5091df027d694226adf6599fa2b46749049efb65c6d0f421c54ed692a134b881
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (168951697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50cb00ee5f8cd912f11c217ae2f432513342ed9c3d563ae94409789a384e5a2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:57:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:57:42 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:57:48 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 05:06:31 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:22:59 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:35:08 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:35:17 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:35:20 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:35:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:35:24 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:35:39 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:35:43 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:35:36 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:35:39 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:35:46 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:35:47 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:53:22 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:53:31 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:53:34 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Wed, 11 Mar 2020 02:53:37 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:53:41 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:53:44 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:53:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:53:58 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83d4344e21f41e55783663900e987c11ef2a6b1168de19ae63f1e05009e4eae`  
		Last Modified: Sat, 18 Jan 2020 05:45:37 GMT  
		Size: 304.0 KB (303987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997052e9d9d744aba0e068db207eeb61eaa721ae09904ce3c203df4e1088408`  
		Last Modified: Wed, 11 Mar 2020 01:52:37 GMT  
		Size: 29.6 MB (29601503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76109d56f0386d8030cb0e3532a1aba32698bda6498c8b8f0e47b733d34b54`  
		Last Modified: Wed, 11 Mar 2020 01:52:29 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0027cf2e6261a311500aab624108c2403b01d6100404370e3b5cfa3e759597fd`  
		Last Modified: Wed, 11 Mar 2020 01:52:30 GMT  
		Size: 1.9 MB (1891099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5a4297dc1e9435d804b5af7fc2cbac58ddc1af9eeab0b3cb1b94369e440f97`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4951daf23dd61a7c9e21936160861cddcd504308e04a4ca81f9952abcc6814e3`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c9333a69e536301bd60e001f4e5b88c7fb88e7fa6bc624409395bb5a208fe4`  
		Last Modified: Wed, 11 Mar 2020 02:56:33 GMT  
		Size: 134.3 MB (134327723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b7eac9ab10fddc9dba9ec26c3cd340093aff28eac163a2cbe57067ebdbbabe`  
		Last Modified: Wed, 11 Mar 2020 02:56:00 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; s390x

```console
$ docker pull plone@sha256:3589edb381d0570ac641b4a8d0a8cd0a493e7285eac9275e4e22a46da86ed2c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167893238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc12fdb7579ed701d648ffc9ea4636149346b699cc98589581a2769ffbfcae12`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:52:22 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 01:52:22 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 01:52:23 GMT
RUN apk add --no-cache ca-certificates
# Sat, 18 Jan 2020 01:56:48 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Sat, 18 Jan 2020 01:56:48 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:02:26 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:02:26 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:52:22 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 00:49:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 00:49:26 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 00:49:30 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 00:49:31 GMT
CMD ["python3"]
# Fri, 06 Mar 2020 23:30:07 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Fri, 06 Mar 2020 23:30:07 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 06 Mar 2020 23:30:09 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 06 Mar 2020 23:30:10 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Fri, 06 Mar 2020 23:37:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Fri, 06 Mar 2020 23:38:23 GMT
VOLUME [/data]
# Fri, 06 Mar 2020 23:38:23 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Fri, 06 Mar 2020 23:38:24 GMT
EXPOSE 8080
# Fri, 06 Mar 2020 23:38:25 GMT
WORKDIR /plone/instance
# Fri, 06 Mar 2020 23:38:25 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 06 Mar 2020 23:38:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 06 Mar 2020 23:38:27 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2a03efad4a7a2934aa60870dd9847c7c02f10dcbbd1614ea32e83c78531ba2`  
		Last Modified: Sat, 18 Jan 2020 02:16:42 GMT  
		Size: 301.8 KB (301798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0627e873630aec7205c7b8e4f1025c14b29c11134532107ac214bb0646e89ad`  
		Last Modified: Sat, 18 Jan 2020 02:17:03 GMT  
		Size: 28.9 MB (28940433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1052253c74f387f87f6ac8e43dc4e0dbc66ee4ea50dc26d9b6bb9bce0415d7`  
		Last Modified: Sat, 18 Jan 2020 02:16:58 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406603440045cdce1ff839ea8eb3f9ebf716cd7daa1977ac349b7c8cbfd3098`  
		Last Modified: Thu, 06 Feb 2020 00:55:22 GMT  
		Size: 1.9 MB (1892187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89906eb9051286a6f61393b0fdc29cbe1a319a8e92321e967e25f372742aae6`  
		Last Modified: Fri, 06 Mar 2020 23:58:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071ee2dd5709fd6ed2a54c89001cf1f401de53a1c1dd8b885a37d59faa24a14c`  
		Last Modified: Fri, 06 Mar 2020 23:58:06 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f47382a3d80c83b2459b21f836eff7cbce5b520f1a972fbdf10d1bbf0f89f2`  
		Last Modified: Fri, 06 Mar 2020 23:58:42 GMT  
		Size: 134.2 MB (134171528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279fcc4ee668ab6054f985db3e9340958850e39f68c4384f63e86ce447df4a0b`  
		Last Modified: Fri, 06 Mar 2020 23:58:36 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:latest`

```console
$ docker pull plone@sha256:c583cb291d96e07260995ecdf50728fd44e7ac8a53d6bea2e53aaa7ce1222aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `plone:latest` - linux; amd64

```console
$ docker pull plone@sha256:0cb3178ff05119e305704fb1b3718000ca517e7a531968bcac3a3e519005f195
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211253085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe96873b433705c1595266384781fc091c2122377a84e205e4f0529935cd4b42`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:35:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:35:17 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 15:55:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 15:55:25 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:45:41 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:53:40 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:53:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:53:41 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:53:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:53:41 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:54:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:54:02 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:32:15 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:32:15 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:32:16 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:32:16 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:36:21 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:36:22 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:36:23 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 01:36:23 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:36:23 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:36:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:36:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:36:24 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87645a1e5dc6a7cce4b4059148c822ef0bfac62508e535151f34fd7ef2ff0be`  
		Last Modified: Wed, 26 Feb 2020 17:48:38 GMT  
		Size: 2.5 MB (2531205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b2a106525c16b953cfac555f4bd97f1158ee7ecd291c534b4d7ea8c62530d`  
		Last Modified: Wed, 11 Mar 2020 01:16:27 GMT  
		Size: 25.8 MB (25814054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2caaa87d8571682506fceb34dc423a115adafac19e7c26ddf48ac5c524afba`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7523def2decc1a9122ef74d34ed1d23a7e3afdd75c918d37afc4662be769ae31`  
		Last Modified: Wed, 11 Mar 2020 01:16:22 GMT  
		Size: 2.2 MB (2174480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c989baa44940ac8f4f3f0ba3a7571aeb38be8d60c5ac1b126e634f8fe0ada5f4`  
		Last Modified: Wed, 11 Mar 2020 01:47:00 GMT  
		Size: 3.9 KB (3882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d018905dbfdfac4b268d87683be09e4c0a8413931c9a1d5f7065c96296dbcea9`  
		Last Modified: Wed, 11 Mar 2020 01:47:00 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6d9ea7bdb2987d14a9675c8d91025dbebf5662169e4895e4d1ab8bb579480c`  
		Last Modified: Wed, 11 Mar 2020 01:47:30 GMT  
		Size: 158.2 MB (158212196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98abd9fa4b73bdf091c75d5aca4a7e6913b94d6754e67e51ca54c6fd5d3ad589`  
		Last Modified: Wed, 11 Mar 2020 01:47:00 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; arm variant v5

```console
$ docker pull plone@sha256:6d098653440cb9c09ee4078a6d6376de8c638d37978df489383ceda59aece7a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.2 MB (204161309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81312fdd64b21072ec52cd402403ae7a20fe5294f04b7275056a8535f39264e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:53:47 GMT
ADD file:3fa7d31ad19db7be28acd7abacb98667f814acaf8ef495a9abb855abe19c351d in / 
# Wed, 26 Feb 2020 00:53:52 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:42:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 07:42:51 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 07:43:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 07:43:10 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:45:47 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:55:56 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:55:59 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:55:59 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:56:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:56:02 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:56:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:56:35 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:14:51 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:14:52 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:14:54 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:14:54 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:29:36 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:29:41 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:29:41 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 01:29:42 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:29:43 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:29:43 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:29:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:29:45 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8b6b97522cf0c1b41e02f7a9de64e8eb22bf8ff5c5ae70bbb46c20761af19aff`  
		Last Modified: Wed, 26 Feb 2020 01:03:39 GMT  
		Size: 21.2 MB (21190915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9992cac12f0e315e738b1de5043f1f997260800f3db4354158b7c6f8167a59d6`  
		Last Modified: Wed, 26 Feb 2020 09:52:31 GMT  
		Size: 2.3 MB (2256558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92c89a1c809c7e2e06de3f9b74e3477e19a8c7e1476c323435e70dd0af7a14`  
		Last Modified: Wed, 11 Mar 2020 00:59:09 GMT  
		Size: 22.8 MB (22774720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208971892dd05fdf86f76efc76041389fa5b1ccc9d61f3a01e3f42e718ddcf17`  
		Last Modified: Wed, 11 Mar 2020 00:59:01 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35230a6c8743392e9e2a71494f96888fe7c3c2adeaf01f994e345fe8a4f87f5a`  
		Last Modified: Wed, 11 Mar 2020 00:59:02 GMT  
		Size: 2.2 MB (2174471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e561d6b0e2609ad719f94ea798b4268e2c134de85a65ee5bfdf94abddf8274aa`  
		Last Modified: Wed, 11 Mar 2020 01:30:14 GMT  
		Size: 3.9 KB (3927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc51c443208a1e2450955b4dd9317f517255a5f7d6b9989b9f08b2642b40dc0`  
		Last Modified: Wed, 11 Mar 2020 01:30:14 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b86bfd9a64793b4c244055f0d2e3df61fae1fe93c63d6d7045aa134736f9d9e`  
		Last Modified: Wed, 11 Mar 2020 01:31:13 GMT  
		Size: 155.8 MB (155756814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5e9a5787f7acfecfe4a0adb5f67f2a9dd93db677352a85ac8347356bda19bd`  
		Last Modified: Wed, 11 Mar 2020 01:30:15 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; arm variant v7

```console
$ docker pull plone@sha256:53abb10dca0476d722cf7340a88ded5fc1de0ecaff947764d7a31b9d2636c5bb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201410579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4b6de4f8793d6fb85b3e886eb49cbb537e8f2ce8daeae8ce46105e4167ea63`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 10:10:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 10:10:05 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 10:10:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 10:10:23 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 00:41:57 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 00:55:00 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 00:55:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 00:55:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 00:55:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 00:55:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 00:55:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 00:55:36 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 01:40:25 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 01:40:25 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 01:40:27 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 01:40:28 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 01:53:34 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 01:53:40 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 01:53:41 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 01:53:41 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 01:53:42 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 01:53:42 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 01:53:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 01:53:44 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a1abc64420e94f85d5deba6b89198f83ed3b269e0396792a904f32d4c1b41a`  
		Last Modified: Wed, 26 Feb 2020 12:27:50 GMT  
		Size: 2.2 MB (2177910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45e41c6e2f8aaef75d598dea9eca9d40f4fcda2a0901582aebe6d306ee50efe`  
		Last Modified: Wed, 11 Mar 2020 01:24:13 GMT  
		Size: 23.3 MB (23309168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607048708c96e44149035b34a2ed5a3e87628ebec4c259dfec7b9db0e26cb3e8`  
		Last Modified: Wed, 11 Mar 2020 01:24:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2640e593c8f87c8624e2b11445083bdec9c44c44b299b19b4204bb86b76524`  
		Last Modified: Wed, 11 Mar 2020 01:24:06 GMT  
		Size: 2.2 MB (2174477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951a3359b1f20d805716e61fdb3006312addf55d34a6a694e85ab91f417d0a4f`  
		Last Modified: Wed, 11 Mar 2020 01:54:02 GMT  
		Size: 3.9 KB (3923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8787cfaf46151cc05c3cb8bfac270908dfd3de1c64b943126e70b51dc2798273`  
		Last Modified: Wed, 11 Mar 2020 01:54:03 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa725bb12cf10f82e4d4cf5669b08c5da3c39c07b3f35fad64fcd8996b7c6b58`  
		Last Modified: Wed, 11 Mar 2020 01:55:02 GMT  
		Size: 154.4 MB (154442850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dd734c260cb9196caf7cfc4d256bb7f8d3c5c7f5b0b56ca1e8772d273e81bb`  
		Last Modified: Wed, 11 Mar 2020 01:54:02 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:00fef410ced7c8124ba6679e6660210ab431894e06d6b508678d1a497c40ee12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.7 MB (204729108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9713e846490b44dc73dd613f727365112ac269982773eddfc85f587164850cde`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 06:49:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 06:49:15 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 16:31:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 16:31:06 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:19:30 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:32:02 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:32:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:32:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:32:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:32:07 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:32:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:32:35 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:20:07 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:20:08 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:20:10 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:20:11 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:33:22 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:33:27 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:33:28 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 02:33:28 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:33:29 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:33:30 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:33:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:33:31 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa16eb173765dedf5be678e2f52fa830e07c02f08b04230546c226c1c8e3713`  
		Last Modified: Wed, 26 Feb 2020 18:37:39 GMT  
		Size: 2.2 MB (2239022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fe0ef4f061e52c5a449e99af521a6b39c95f8ecb9ac72e7c623cb3d9bf295a`  
		Last Modified: Wed, 11 Mar 2020 02:03:52 GMT  
		Size: 24.6 MB (24648861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99758f14acfef3b5933115eb26e06f8affc666dc4896cbe24251ed44133a99f7`  
		Last Modified: Wed, 11 Mar 2020 02:03:43 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c23db0034242e225d54e2cbf7e896b6ffea4de1a525d6c012248d723beac99`  
		Last Modified: Wed, 11 Mar 2020 02:03:44 GMT  
		Size: 2.2 MB (2174412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fcc65b631d5d768adbf8410f52baba0b32b21c35b43d49f97135ad38151972`  
		Last Modified: Wed, 11 Mar 2020 02:52:34 GMT  
		Size: 3.9 KB (3939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa31b0e87a19054d3aa9a02db510d6a3bc2a3ba1cc602082a551694ef2e45b`  
		Last Modified: Wed, 11 Mar 2020 02:52:34 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902b44f6b903a62d9a139788a4816cadba1acdc844468829dc774bfb30a488`  
		Last Modified: Wed, 11 Mar 2020 02:53:24 GMT  
		Size: 155.3 MB (155288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95b07b6eb49fc08a26cbe7babedb15ff2ba1e6bf4de0160e78517e2d6eee82b`  
		Last Modified: Wed, 11 Mar 2020 02:52:34 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; 386

```console
$ docker pull plone@sha256:65146f9148ef1bc03b555311f39768a00aa2bf62b20120586a43c278a289d0e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.5 MB (210459204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5de6f5d69682704a07fa9cfd305dd4fd27b8f014cba0a4c845a680de6d567e8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:35:41 GMT
ADD file:7d77438aab7eb35501c0d27bd4350a3a9b4fd1988ce7e7fc0670a570b3112590 in / 
# Wed, 26 Feb 2020 00:35:42 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:25:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 11:25:58 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 13:32:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 13:32:29 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:17:17 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:26:28 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:26:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:26:29 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:26:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:26:29 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:26:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:26:44 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:05:50 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:05:50 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:05:51 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:05:51 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:09:48 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:09:50 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:09:50 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 02:09:50 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:09:50 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:09:51 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:09:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:09:51 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:5cf237473070a9ef7639307699a23bb6c32cd8321bf84c0cf61b6f9c32b44341`  
		Last Modified: Wed, 26 Feb 2020 00:42:02 GMT  
		Size: 23.1 MB (23141399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4967a9ed267c1255b8f9d33516517d50eb0555c2653a3353f92d04d1dc57d4f`  
		Last Modified: Wed, 26 Feb 2020 15:50:10 GMT  
		Size: 2.5 MB (2532885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac247d2b4799c201a9d2b9df26abe8d3d4963053c341fb070ed0c5273667515`  
		Last Modified: Wed, 11 Mar 2020 01:50:00 GMT  
		Size: 24.2 MB (24181838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703246de72ee13411ff22ede73d86fdb2b75f50d0f75a865ea7dddc686ca30cf`  
		Last Modified: Wed, 11 Mar 2020 01:49:53 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cec631a0546598549f0b296cfed4f22a1f8c0be3be5b37eb827e14a5c26390`  
		Last Modified: Wed, 11 Mar 2020 01:49:54 GMT  
		Size: 2.2 MB (2173881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f91b8fd3c30527357ff6e91a32ea02107902cbd9792e23fe1a4650bf4a884b3`  
		Last Modified: Wed, 11 Mar 2020 02:20:34 GMT  
		Size: 3.9 KB (3875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e435f995303fafcf9a2cda29a1c614bc6099c69c1aba2f567204ee271be18a`  
		Last Modified: Wed, 11 Mar 2020 02:20:34 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4e51d9c776bb1628133878b3190f1cda8cb6b911f92517dfd0f8ca092cd27`  
		Last Modified: Wed, 11 Mar 2020 02:21:15 GMT  
		Size: 158.4 MB (158421426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2077f302ac4bd347f71e254a371a7879ef941d0cae2dcf00876ae88f6028df`  
		Last Modified: Wed, 11 Mar 2020 02:20:34 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; ppc64le

```console
$ docker pull plone@sha256:00d6f420c63806681956a9226fa3ed2228656330898a515abe576d0542201e0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.7 MB (209731614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d633a48efffd457506814ee7f55acacb206adec5798ea69bb4180f7b599db55c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:37:18 GMT
ADD file:661513607cf6a4c5038d6048ea16a04dedb05c03ce6c0e33e409f51510562e11 in / 
# Wed, 26 Feb 2020 01:37:25 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:01:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 04:02:01 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 04:02:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:02:36 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Wed, 11 Mar 2020 01:07:30 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 11 Mar 2020 01:21:49 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 11 Mar 2020 01:21:55 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 11 Mar 2020 01:21:57 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 11 Mar 2020 01:21:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 11 Mar 2020 01:22:01 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 11 Mar 2020 01:22:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Mar 2020 01:22:49 GMT
CMD ["python3"]
# Wed, 11 Mar 2020 02:13:26 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 11 Mar 2020 02:13:29 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 11 Mar 2020 02:13:40 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 11 Mar 2020 02:13:41 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 11 Mar 2020 02:34:53 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 11 Mar 2020 02:35:00 GMT
VOLUME [/data]
# Wed, 11 Mar 2020 02:35:01 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 11 Mar 2020 02:35:03 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 02:35:07 GMT
WORKDIR /plone/instance
# Wed, 11 Mar 2020 02:35:11 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 11 Mar 2020 02:35:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Mar 2020 02:35:18 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:21d148b1dce5a6179231486bac7845a111bbaba4fcaf4232bbc39842bf6c5366`  
		Last Modified: Wed, 26 Feb 2020 02:04:13 GMT  
		Size: 22.8 MB (22785269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04588e26d3c0ec872194ff5ef594823fcf086866a0ec8f2d5a6eeddd987ed841`  
		Last Modified: Wed, 26 Feb 2020 06:05:23 GMT  
		Size: 2.2 MB (2192705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd168104b4b256e82aacc6ed232d1568f33b1e93a094780a12e92564cb7da8`  
		Last Modified: Wed, 11 Mar 2020 01:52:19 GMT  
		Size: 25.9 MB (25853125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f1050b97275cfe94c058bf8f2ea59586046a45a8bc3c5ca46d8994d43ac035`  
		Last Modified: Wed, 11 Mar 2020 01:52:11 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be261a9444d3fba5dc1a3bd9a97b796835615927636aee545115461247a7f02`  
		Last Modified: Wed, 11 Mar 2020 01:52:12 GMT  
		Size: 2.2 MB (2175332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d5b0650bdae6cc629411942f8996e26cd0f0ad4cef676d8144c46a49a527fa`  
		Last Modified: Wed, 11 Mar 2020 02:54:30 GMT  
		Size: 3.9 KB (3935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7573258eb31ff044d820fb7d687da62edd99dff534c759fd3799b0601ea0a89`  
		Last Modified: Wed, 11 Mar 2020 02:54:41 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fb8f493563d5a382df2a8a844e8d407278432a5739ec90c38ab3ee1676a217`  
		Last Modified: Wed, 11 Mar 2020 02:55:41 GMT  
		Size: 156.7 MB (156717344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bc946735b67e3cb0651e21d3ee7391eaaf81b9634cb3fe0914e938a0d0c14d`  
		Last Modified: Wed, 11 Mar 2020 02:54:30 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:python2`

```console
$ docker pull plone@sha256:aa15d492392c7f979a6fc51e6a45346c2efc99ca569901a77e8b366159752194
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `plone:python2` - linux; amd64

```console
$ docker pull plone@sha256:540d65605e99cbe77e3b24e19685caade491bbcf2bfa487b4518139926b1224d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.1 MB (204072220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da38b5ff841e0e4c692d310295c9067737225a614f460277a26956e93069524a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:35:16 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:35:17 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 17:36:54 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 17:37:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 17:37:03 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 17:37:03 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 17:44:49 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 17:44:49 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 17:44:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 17:44:50 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 17:45:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 17:45:11 GMT
CMD ["python2"]
# Thu, 27 Feb 2020 05:51:54 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 05:51:54 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 05:51:55 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 05:51:55 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 05:55:18 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 05:55:19 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 05:55:20 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 05:55:20 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 05:55:20 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 05:55:20 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 05:55:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 05:55:21 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc9812e632c6d6ab24bab1e95a31e23ab58ad0bf16eb02f0bfe83eedfde451`  
		Last Modified: Wed, 26 Feb 2020 17:51:28 GMT  
		Size: 2.5 MB (2531126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf60c41eb44a406e9849ec135ae509def6f28fb268aa804c27318320f5d1ad45`  
		Last Modified: Wed, 26 Feb 2020 17:51:33 GMT  
		Size: 18.3 MB (18299655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0afc907c6427941de6a92e5ed45ee6a85da6d712f797ccf9d82dc212d4871e`  
		Last Modified: Wed, 26 Feb 2020 17:51:29 GMT  
		Size: 2.2 MB (2171134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2714e3e3ecaf0cc6c8baedae8713b12db112272b8c0740ea93baa0d44de301ae`  
		Last Modified: Thu, 27 Feb 2020 05:56:04 GMT  
		Size: 3.9 KB (3881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3c44b94b47ff3a4e16f6ff5927c38957d1acd89db27beea470de0783f171f6`  
		Last Modified: Thu, 27 Feb 2020 05:56:04 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9900cabad2c07f45a974670fb9b1dd74765736780a88d86885ef7d5780654c0`  
		Last Modified: Thu, 27 Feb 2020 05:56:33 GMT  
		Size: 158.5 MB (158549398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f334620302933ae284104cb42c85092ec4a83bcf93491ca14061bc79547b3b76`  
		Last Modified: Thu, 27 Feb 2020 05:56:04 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python2` - linux; arm variant v5

```console
$ docker pull plone@sha256:a1e8e5c5d0043c7abd4b3bf2f26f8abfca1c9b3c04161dda9486889e1d67a001
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198319056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23ae273d660f75adb8e9152eb0898d7d3b9d82a8f9f37c3aa0a497d9e97ebe44`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:53:47 GMT
ADD file:3fa7d31ad19db7be28acd7abacb98667f814acaf8ef495a9abb855abe19c351d in / 
# Wed, 26 Feb 2020 00:53:52 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:42:50 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 07:42:51 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 09:38:22 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 09:38:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 09:38:40 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 09:38:40 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 09:49:03 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 09:49:05 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 09:49:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 09:49:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 09:49:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 09:49:41 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 16:50:19 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 16:50:20 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 16:50:21 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 16:50:22 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 17:04:44 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 17:04:52 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 17:04:53 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 17:04:54 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 17:04:54 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 17:04:55 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 17:04:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 17:04:56 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8b6b97522cf0c1b41e02f7a9de64e8eb22bf8ff5c5ae70bbb46c20761af19aff`  
		Last Modified: Wed, 26 Feb 2020 01:03:39 GMT  
		Size: 21.2 MB (21190915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b73943cef5202f8e4dd87696f8e23ffcc73285ff563bd9d93225e77386cc22`  
		Last Modified: Wed, 26 Feb 2020 09:55:25 GMT  
		Size: 2.3 MB (2256550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4665b8b9f4fe07f77f52c530fb25596c8630a917915135e5bf49d8062c4642`  
		Last Modified: Wed, 26 Feb 2020 09:55:31 GMT  
		Size: 17.2 MB (17210295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50406ea4007f79f7a05b48720d7c9b304b6dbb8d098976d8d51da749c89fff9`  
		Last Modified: Wed, 26 Feb 2020 09:55:26 GMT  
		Size: 2.2 MB (2171005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058eac253fa9aad07df17afa5ac99a80770c0c81cc43d9b520a0da588d17d656`  
		Last Modified: Wed, 26 Feb 2020 17:06:17 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846a165f4392d0ea14c9b42704daee0fe3933c34c49606b314faf2deeb4fb57d`  
		Last Modified: Wed, 26 Feb 2020 17:06:17 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0ae4d84ddf208f6c23c317ed4dcde434a59ec79015798458584e1f6b2f0fc8`  
		Last Modified: Wed, 26 Feb 2020 17:07:18 GMT  
		Size: 155.5 MB (155482703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ad5352975d66571cbbdd6121f8af9ca22882ebbdca9b753e6aaa7bd9ace25b`  
		Last Modified: Wed, 26 Feb 2020 17:06:17 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python2` - linux; arm variant v7

```console
$ docker pull plone@sha256:9e9a3ad31d4d07f21f25816373f818dc88f9edb02054f1a2f7e5f9a78bed80f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194582684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6bc4b60a8df1efaf7e4338984b96e952af03bd6f85d953de399e684460fd085`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 10:10:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 10:10:05 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 12:12:58 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 12:13:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 12:13:31 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 12:13:33 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 12:23:10 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 12:23:12 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 12:23:13 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 12:23:13 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 12:23:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 12:23:39 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 23:34:39 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 23:34:40 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 23:34:42 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 23:34:42 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 23:47:16 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 23:47:24 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 23:47:25 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 23:47:26 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 23:47:26 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 23:47:27 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 23:47:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 23:47:28 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a720c0b453d29444434cc1b23aab9aadfe64717e634abbdb60d08c44bf21f19c`  
		Last Modified: Wed, 26 Feb 2020 12:31:02 GMT  
		Size: 2.2 MB (2177999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655d6d48ec871b22d20195af872e0f2a0b502067f01c7998036793680ea6f2b8`  
		Last Modified: Wed, 26 Feb 2020 12:31:06 GMT  
		Size: 16.8 MB (16755146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96468ee01cebaac4bbb9c22eb33c4617d11289115e5ce1a67cf00d61612e6b3`  
		Last Modified: Wed, 26 Feb 2020 12:31:02 GMT  
		Size: 2.2 MB (2170988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18cabd1fc64da1e26b24006e70e974292a199415c3daf589b87ff99c33b7bab`  
		Last Modified: Wed, 26 Feb 2020 23:48:47 GMT  
		Size: 3.9 KB (3924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f51c595b57a1c5596a7292eb97e9ecd9594b9ddb77a514575f6e5be309dac9`  
		Last Modified: Wed, 26 Feb 2020 23:48:48 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ed14888cba72d6da4de76321ad11239ab5b07c3881e5eb849ac766dc326980`  
		Last Modified: Wed, 26 Feb 2020 23:49:47 GMT  
		Size: 154.2 MB (154172617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e164c0b7a2e7e199999dbea53376badfe5bd4ab5679dc940cd09cda0269107bd`  
		Last Modified: Wed, 26 Feb 2020 23:48:48 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python2` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:f38e7d0b4a24c62d87823ae50065eb3d397e302a897a6646a510de40b7dd524d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.5 MB (197456286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f491d504008f3377155b254e0ae3d9f3717c5e26d2f0731d6feec6f426b81f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 06:49:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 06:49:15 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 18:23:32 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 18:23:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 18:23:47 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 18:23:47 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 18:33:07 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 18:33:09 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 18:33:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 18:33:11 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 18:33:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 18:33:38 GMT
CMD ["python2"]
# Thu, 27 Feb 2020 04:26:39 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 04:26:39 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 04:26:41 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 04:26:42 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 04:39:50 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 04:39:57 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 04:39:58 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 04:39:59 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 04:40:00 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 04:40:00 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 04:40:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 04:40:01 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d99d50b39d76f3fd90dc0eaa7228df164554d76604a524b83002fc37567940`  
		Last Modified: Wed, 26 Feb 2020 18:41:04 GMT  
		Size: 2.2 MB (2238910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed173cf84106c21c4e733ad301f2dcf4b13fe58a2c45b67dc97f6bc53352ab2`  
		Last Modified: Wed, 26 Feb 2020 18:41:11 GMT  
		Size: 17.6 MB (17646664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828f5104cc6203db57f480c339442b7a7c4b9dc976fd4bb48c5964216e74e41e`  
		Last Modified: Wed, 26 Feb 2020 18:41:04 GMT  
		Size: 2.2 MB (2170904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a11f007ca466a7e2d873064418db96552c5239c9a562893d0d03a2cfaad2957`  
		Last Modified: Thu, 27 Feb 2020 04:41:27 GMT  
		Size: 3.9 KB (3941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9647f7696f2c1197e7e659e9bf35b7915d9d0109ba56ec295cf169c4a0031d1a`  
		Last Modified: Thu, 27 Feb 2020 04:41:27 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ebd14353d0b9fcd8141c4c2cc72e896bea1e9a1bc8cf7dbfff8b59011a1394`  
		Last Modified: Thu, 27 Feb 2020 04:42:17 GMT  
		Size: 155.0 MB (155022225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3bdfefd82cb56684e16783f17e4d3c5d0f57ee8cb1b7a50e7f43ec08e1cc34`  
		Last Modified: Thu, 27 Feb 2020 04:41:27 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python2` - linux; 386

```console
$ docker pull plone@sha256:0cb8be1a109ca0c979b2a0542938d19f7b118f1a2395ff9821cd613f5a89c516
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203807104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:560c1eac7751356d6ace1226b7ea3eaaf53a5710445527e332d90027108ac65d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 00:35:41 GMT
ADD file:7d77438aab7eb35501c0d27bd4350a3a9b4fd1988ce7e7fc0670a570b3112590 in / 
# Wed, 26 Feb 2020 00:35:42 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:25:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 11:25:58 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 15:38:52 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 15:39:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 15:39:01 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 15:39:01 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 15:46:25 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 15:46:25 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 15:46:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 15:46:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 15:46:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 15:46:41 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 20:21:16 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 20:21:17 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 20:21:19 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 20:21:19 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 20:25:56 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 20:25:58 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 20:25:58 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 20:25:58 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 20:25:59 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 20:25:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 20:25:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 20:25:59 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:5cf237473070a9ef7639307699a23bb6c32cd8321bf84c0cf61b6f9c32b44341`  
		Last Modified: Wed, 26 Feb 2020 00:42:02 GMT  
		Size: 23.1 MB (23141399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2faea37536bb10c13dd52913b524ee145e30cc577f79e94229067fb7381a3366`  
		Last Modified: Wed, 26 Feb 2020 15:52:23 GMT  
		Size: 2.5 MB (2532882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65facf1ea86c567f91573ca42282f8f8104ce0654a00d0c146a6e57a494f04a5`  
		Last Modified: Wed, 26 Feb 2020 15:52:27 GMT  
		Size: 17.2 MB (17244731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82181b01888156e580308b59e5fdd7575df2a0b81e9302aba0e7111029e5637`  
		Last Modified: Wed, 26 Feb 2020 15:52:23 GMT  
		Size: 2.2 MB (2170928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ea53354456a39fd74c387b4c7c8b94a5d97c3324d9673f83df6770778ed76a`  
		Last Modified: Wed, 26 Feb 2020 20:27:24 GMT  
		Size: 3.9 KB (3875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc5b85da19d843ab0e464cb8b42aac8c847173f5cf4c10f89c090c3de32d466`  
		Last Modified: Wed, 26 Feb 2020 20:27:24 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee362b752174680d6e79255910f5b85d8f679597edb1babdd22bbf023ed0c9cb`  
		Last Modified: Wed, 26 Feb 2020 20:28:10 GMT  
		Size: 158.7 MB (158709624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19d233ccc6fd095b8c14398d4b2e18bc38faa4978ac1344092d017ff8340bd4`  
		Last Modified: Wed, 26 Feb 2020 20:27:24 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:python2` - linux; ppc64le

```console
$ docker pull plone@sha256:fabcbbd4ab3358248256c7fe286f1768d2bd7c3652cd90835ee0f94402d0caa3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.9 MB (201869896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e353f7045c5c12c6542c7bdfe883c6b89ef7fc01f67ab70b5a1760d2e8405ca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Wed, 26 Feb 2020 01:37:18 GMT
ADD file:661513607cf6a4c5038d6048ea16a04dedb05c03ce6c0e33e409f51510562e11 in / 
# Wed, 26 Feb 2020 01:37:25 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:01:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 04:02:01 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 05:46:29 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 26 Feb 2020 05:47:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		netbase 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 05:47:09 GMT
ENV GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF
# Wed, 26 Feb 2020 05:47:14 GMT
ENV PYTHON_VERSION=2.7.17
# Wed, 26 Feb 2020 06:00:08 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbz2-dev 		libc6-dev 		libdb-dev 		libgdbm-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--enable-unicode=ucs4 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python2 --version
# Wed, 26 Feb 2020 06:00:11 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 06:00:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 06:00:17 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 06:01:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 06:01:28 GMT
CMD ["python2"]
# Wed, 26 Feb 2020 21:07:57 GMT
ENV PIP=19.0.3 ZC_BUILDOUT=2.13.2 SETUPTOOLS=41.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 21:08:00 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 21:08:08 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 21:08:09 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 21:29:02 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 21:29:11 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 21:29:15 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 21:29:18 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 21:29:22 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 21:29:26 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 21:29:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 21:29:36 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:21d148b1dce5a6179231486bac7845a111bbaba4fcaf4232bbc39842bf6c5366`  
		Last Modified: Wed, 26 Feb 2020 02:04:13 GMT  
		Size: 22.8 MB (22785269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bc85883bb3736ef2e561ed5e633404a8dff44dd1d9bdf65d8899e44b3a6c6d`  
		Last Modified: Wed, 26 Feb 2020 06:07:34 GMT  
		Size: 2.2 MB (2192776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89deb8a33ea35dcfce45dc587a961eea14d457bbc18a95ffd09d4a5c52e90bab`  
		Last Modified: Wed, 26 Feb 2020 06:07:37 GMT  
		Size: 18.3 MB (18258209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7526c7803ffe676727247704b185a74b9487da6724dc2b3c13a8c37adc9cf7`  
		Last Modified: Wed, 26 Feb 2020 06:07:35 GMT  
		Size: 2.2 MB (2172157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7a26feed99ea23e7e263f6463d1fdb60afd5ba448faa4901a266a5f4965b3a`  
		Last Modified: Wed, 26 Feb 2020 21:34:37 GMT  
		Size: 3.9 KB (3939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1bbbdac1cfc4287d64f299478b23812c7b5d9d10cd2b9c61b5584317957bf5`  
		Last Modified: Wed, 26 Feb 2020 21:34:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f02f21529fbfc45364814399a298f42cf95ef952b5860ef8e1cdc63d2e702d`  
		Last Modified: Wed, 26 Feb 2020 21:38:36 GMT  
		Size: 156.5 MB (156453881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ce4caad5fefe888d2954f28c821862e7d900876801254337f439516deb7e3`  
		Last Modified: Wed, 26 Feb 2020 21:34:37 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
