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
$ docker pull plone@sha256:3598db582fd18e0e79067a869f63c8bc063cee5fd9c01c40ee01f625944a3a0c
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
$ docker pull plone@sha256:ceb59901e866ec67d66005ef2f747b98cf6c13962b89bd96a24d8acb2dbb4a56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211290985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0dc524b96661924ba6b46ef04c6fe07f5e7da04ee95116822a7ec8d128f114b`
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
# Wed, 26 Feb 2020 15:55:25 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 16:05:21 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 16:05:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 16:05:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 16:05:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 16:05:24 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 16:05:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 16:05:44 GMT
CMD ["python3"]
# Thu, 27 Feb 2020 05:48:05 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 05:48:05 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 05:48:06 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 05:48:06 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 05:51:37 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 05:51:38 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 05:51:38 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 05:51:39 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 05:51:39 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 05:51:39 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 05:51:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 05:51:39 GMT
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
	-	`sha256:6a33999da14c835e8d3ddcef893fa350153761194bdad1c4a5ee5aa0be90f99c`  
		Last Modified: Wed, 26 Feb 2020 17:48:44 GMT  
		Size: 25.8 MB (25798778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66020c9836480d0db8f94f2acc77f32bf2dd3063a10f4d1d20de5b149009ef4`  
		Last Modified: Wed, 26 Feb 2020 17:48:38 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4703522495058fef344d4879a78cca1e9e153944cee3f036a8ab1ecae6dd839`  
		Last Modified: Wed, 26 Feb 2020 17:48:38 GMT  
		Size: 2.2 MB (2176130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e763c27664adfe48dfa0c2e91cfbb1f2526dd6282a1f2c05d9f93805b66e6b`  
		Last Modified: Thu, 27 Feb 2020 05:55:31 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d47d7fdaea68eeb5b75b87786b64e2b50ef6147dd07c686e7b21488a14f260`  
		Last Modified: Thu, 27 Feb 2020 05:55:31 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68114f24f65e8d32aecc6b595c0ab1d22dec7865ea29a09a06793330c2b6787f`  
		Last Modified: Thu, 27 Feb 2020 05:55:58 GMT  
		Size: 158.3 MB (158263721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bd512f7102a2793a61a194251288014c655138b3f7bc8f9b7f6ce98a037e0d`  
		Last Modified: Thu, 27 Feb 2020 05:55:30 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; arm variant v5

```console
$ docker pull plone@sha256:f1ee2e2cf24e672ab9d950a816efd14c229edcadd2f1f4e7ff1d494969eb47ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.2 MB (204187751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701fabf98700b541e80f72ac32cfd6579de85841d6f46ee50b198971aad428b3`
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
# Wed, 26 Feb 2020 07:43:10 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 07:53:26 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 07:53:29 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 07:53:30 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 07:53:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 07:53:31 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 07:54:04 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 07:54:05 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 16:34:34 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 16:34:35 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 16:34:38 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 16:34:39 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 16:49:53 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 16:50:02 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 16:50:03 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 16:50:04 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 16:50:04 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 16:50:05 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 16:50:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 16:50:06 GMT
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
	-	`sha256:d656f5a68dce32db0da25657fa8145509090dd717db0863e3db4a1311d35cad7`  
		Last Modified: Wed, 26 Feb 2020 09:52:39 GMT  
		Size: 22.8 MB (22770271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe441b54bc0ba71262311bc0d52e1668eeac33128e8f36c6af8fa3e6f331b17`  
		Last Modified: Wed, 26 Feb 2020 09:52:31 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595aaeb76d185f5074015b02211536772493bf063be415920a206b07df589942`  
		Last Modified: Wed, 26 Feb 2020 09:52:32 GMT  
		Size: 2.2 MB (2175913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c00d302ea0af84737c436e4cb35da3708abe19235483300dcd58d85b2e9b1b`  
		Last Modified: Wed, 26 Feb 2020 17:05:07 GMT  
		Size: 3.9 KB (3925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abee76f1efce0ea1da36f0f2989c826993ed3ea2e50b6d09bc9b1835b05e1b0`  
		Last Modified: Wed, 26 Feb 2020 17:05:07 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862e034aab772fc7287991f2c52184c8a9ff9aa92f6c16b043211519c0194e49`  
		Last Modified: Wed, 26 Feb 2020 17:06:08 GMT  
		Size: 155.8 MB (155786269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de48e91c45e20dca818e2dcaf7e5caba591beeab6628b545b31b8e0b068d9ada`  
		Last Modified: Wed, 26 Feb 2020 17:05:07 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; arm variant v7

```console
$ docker pull plone@sha256:214303debdcd61422d269ee7b40b0b4da11af7c3295724f5561d92081892d525
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.5 MB (201472309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16474bc9c1a41eb8c1eebd8f52c7f821e1c21ae48d47289152b4c30c6837e247`
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
# Wed, 26 Feb 2020 10:10:24 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 10:23:19 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 10:23:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 10:23:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 10:23:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 10:23:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 10:23:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 10:23:52 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 23:21:11 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 23:21:12 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 23:21:16 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 23:21:17 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 23:34:21 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 23:34:28 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 23:34:29 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 23:34:29 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 23:34:30 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 23:34:31 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 23:34:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 23:34:32 GMT
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
	-	`sha256:6b2b245c7a0af359854db6ff69d5961cf78220a90f0c35e133f8b1c193b64b2c`  
		Last Modified: Wed, 26 Feb 2020 12:27:59 GMT  
		Size: 23.3 MB (23341944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa24266bc1f7d33a53425b488668c6f12d9119b321df759e07b7511c5a0cf057`  
		Last Modified: Wed, 26 Feb 2020 12:27:49 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb838bd6d171e306f9a7bae4693aa12f8b3661bb1513744488d25cbefbecc34`  
		Last Modified: Wed, 26 Feb 2020 12:27:50 GMT  
		Size: 2.2 MB (2175955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b22b8976660ae5dd1d3a6e3b9fd151b01613f6851f628848d2319d2cd3d687e`  
		Last Modified: Wed, 26 Feb 2020 23:47:42 GMT  
		Size: 3.9 KB (3927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ece09e7454f28201a9b11ea15b4c65bff449a93cdc594127208114975c26b7`  
		Last Modified: Wed, 26 Feb 2020 23:47:42 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82da71967ea508b1c336249654a489de13b1c340e27a3277f2b2c3b76bc5afd6`  
		Last Modified: Wed, 26 Feb 2020 23:48:38 GMT  
		Size: 154.5 MB (154470319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0fd9bb5d13ee64e18385cbb3953e7e18cddc8db731d536a0f1e73041ccac18`  
		Last Modified: Wed, 26 Feb 2020 23:47:41 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:1f7389070d10279c0672d02cea678b9e2a62f5a07c430516f108f0bc63ccdcaa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.8 MB (204756651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9bc590e017ec955cbddb1164ce1f21a67e5c9b4d2de4da4d287e46b8df8503`
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
# Wed, 26 Feb 2020 16:31:07 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 16:43:32 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 16:43:34 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 16:43:35 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 16:43:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 16:43:36 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 16:44:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 16:44:01 GMT
CMD ["python3"]
# Thu, 27 Feb 2020 04:12:36 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 04:12:37 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 04:12:39 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 04:12:40 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 04:26:07 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 04:26:13 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 04:26:14 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 04:26:15 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 04:26:16 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 04:26:16 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 04:26:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 04:26:18 GMT
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
	-	`sha256:7a935d604f767a1b217bfe7f9d447c14b71eb5374ffa8278a1a2b2c3ade4b8d4`  
		Last Modified: Wed, 26 Feb 2020 18:37:47 GMT  
		Size: 24.6 MB (24642485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2c221be0fd5417f9d1b382f04d0be0c23decf3862a18be2557a5ada8b38a81`  
		Last Modified: Wed, 26 Feb 2020 18:37:38 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f859a56ff0ad189b82614fc47d2db5777e932e063ad0a077d771c825fbc0a18`  
		Last Modified: Wed, 26 Feb 2020 18:37:39 GMT  
		Size: 2.2 MB (2175818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaeb4713261f88d7096432170cbb67ead5bfd0fdcb56f3e734b3c15854d978`  
		Last Modified: Thu, 27 Feb 2020 04:40:29 GMT  
		Size: 3.9 KB (3938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6501e3434223e00219cc740175867bfe7ffa66bff8732bcfe605e4b583b3b1ed`  
		Last Modified: Thu, 27 Feb 2020 04:40:29 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12efba0f87b7801cf9ecc73d27a8912b48fe5cd541de54acc680f2ebe50870a`  
		Last Modified: Thu, 27 Feb 2020 04:41:15 GMT  
		Size: 155.3 MB (155321506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a7147a31133fdd8d62354a465c24571ddd88266d90240fea63ae932a5f1e82`  
		Last Modified: Thu, 27 Feb 2020 04:40:29 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; 386

```console
$ docker pull plone@sha256:7156ed5eed6a8d9d2e803ea06f9190a7865460c779ecbd513f4b9e0b94ce0d21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.5 MB (210547897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21f43ffd375048752eaaf0c8a0b5e5a9908d68a58b3bc64e76068bb0943c87e7`
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
# Wed, 26 Feb 2020 13:32:29 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 13:46:05 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 13:46:06 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 13:46:06 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 13:46:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 13:46:07 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 13:46:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 13:46:24 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 20:16:25 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 20:16:25 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 20:16:26 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 20:16:26 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 20:20:57 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 20:20:58 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 20:20:58 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 20:20:58 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 20:20:58 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 20:20:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 20:20:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 20:20:59 GMT
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
	-	`sha256:348e763dadfd1b50ff2edb8db5bfc850d30d36ecc064bb59619b6c6d6907e0ee`  
		Last Modified: Wed, 26 Feb 2020 15:50:16 GMT  
		Size: 24.2 MB (24220228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddab4eecfc9a7a10fccdd0e8bab77fd7b8ee7fb0071010573940c23c7628670`  
		Last Modified: Wed, 26 Feb 2020 15:50:09 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e48df556a7b9278e2d994e723c841a90b489f0402a453ba8431053380219fbc`  
		Last Modified: Wed, 26 Feb 2020 15:50:10 GMT  
		Size: 2.2 MB (2175788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e4005781a4394f5c90bc432850f94859e490bb5f21717f2e6b932ff6a191d2`  
		Last Modified: Wed, 26 Feb 2020 20:26:21 GMT  
		Size: 3.9 KB (3873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0ec73ea37c1efe7f599ed0256171c4652822b56fe58b4481980beae0bd309a`  
		Last Modified: Wed, 26 Feb 2020 20:26:21 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc6846fa93309fbbafd84b2465c4259e8b48e8e3f0f7ae193a7170be3fd43de`  
		Last Modified: Wed, 26 Feb 2020 20:27:18 GMT  
		Size: 158.5 MB (158469826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d833dfe4555374e8ab4eceabe08d85851e659e6a0eba6711ee0a0f924dc8dcd0`  
		Last Modified: Wed, 26 Feb 2020 20:26:21 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5` - linux; ppc64le

```console
$ docker pull plone@sha256:17c4307890f9a856016b666c7061b3e0b5a1eea5fb8a8cde982151717aefb96d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.8 MB (209783941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d2fe8cfe5a13c4b275bc426038eec3858c7357395e5ee4effe9119a5540e8ea`
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
# Wed, 26 Feb 2020 04:02:38 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 04:18:08 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 04:18:16 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 04:18:18 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 04:18:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 04:18:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 04:19:18 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 04:19:21 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 20:47:42 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 20:47:45 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 20:47:56 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 20:47:57 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 21:06:50 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 21:06:57 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 21:06:59 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 21:07:01 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 21:07:04 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 21:07:07 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 21:07:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 21:07:13 GMT
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
	-	`sha256:af1513bf2ee03f2207d52345cb8aab950ec5068ec549b6cc088883cbca15f589`  
		Last Modified: Wed, 26 Feb 2020 06:05:30 GMT  
		Size: 25.9 MB (25876486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b3c1956c8f7efa590d60fe60b38ae14e16d52e0cf761a027fa508bdcc6e9c3`  
		Last Modified: Wed, 26 Feb 2020 06:05:22 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d06518c1d2db54727f6703bbbb53ca3d6c455f37698b29ac36e7f56aa8072b`  
		Last Modified: Wed, 26 Feb 2020 06:05:29 GMT  
		Size: 2.2 MB (2177157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0979f1e8cf6dcc2466de7ff88c1da8b24f21d1981cf323a1357100177df72`  
		Last Modified: Wed, 26 Feb 2020 21:29:59 GMT  
		Size: 3.9 KB (3938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d7021169b65fe3a0fe29d0b106245899e94afccee671744aa0b78f29a77479`  
		Last Modified: Wed, 26 Feb 2020 21:29:59 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb31f56f89b4d9ddf929bc79a25c705f4ea472b254a66931f16eb372ddb207f`  
		Last Modified: Wed, 26 Feb 2020 21:34:15 GMT  
		Size: 156.7 MB (156744482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d994590772d0ed4543da406d847fbd2362b5c00f00a8e39a6858fe972dc7a70d`  
		Last Modified: Wed, 26 Feb 2020 21:29:59 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2`

```console
$ docker pull plone@sha256:3598db582fd18e0e79067a869f63c8bc063cee5fd9c01c40ee01f625944a3a0c
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
$ docker pull plone@sha256:ceb59901e866ec67d66005ef2f747b98cf6c13962b89bd96a24d8acb2dbb4a56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211290985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0dc524b96661924ba6b46ef04c6fe07f5e7da04ee95116822a7ec8d128f114b`
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
# Wed, 26 Feb 2020 15:55:25 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 16:05:21 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 16:05:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 16:05:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 16:05:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 16:05:24 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 16:05:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 16:05:44 GMT
CMD ["python3"]
# Thu, 27 Feb 2020 05:48:05 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 05:48:05 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 05:48:06 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 05:48:06 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 05:51:37 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 05:51:38 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 05:51:38 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 05:51:39 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 05:51:39 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 05:51:39 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 05:51:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 05:51:39 GMT
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
	-	`sha256:6a33999da14c835e8d3ddcef893fa350153761194bdad1c4a5ee5aa0be90f99c`  
		Last Modified: Wed, 26 Feb 2020 17:48:44 GMT  
		Size: 25.8 MB (25798778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66020c9836480d0db8f94f2acc77f32bf2dd3063a10f4d1d20de5b149009ef4`  
		Last Modified: Wed, 26 Feb 2020 17:48:38 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4703522495058fef344d4879a78cca1e9e153944cee3f036a8ab1ecae6dd839`  
		Last Modified: Wed, 26 Feb 2020 17:48:38 GMT  
		Size: 2.2 MB (2176130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e763c27664adfe48dfa0c2e91cfbb1f2526dd6282a1f2c05d9f93805b66e6b`  
		Last Modified: Thu, 27 Feb 2020 05:55:31 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d47d7fdaea68eeb5b75b87786b64e2b50ef6147dd07c686e7b21488a14f260`  
		Last Modified: Thu, 27 Feb 2020 05:55:31 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68114f24f65e8d32aecc6b595c0ab1d22dec7865ea29a09a06793330c2b6787f`  
		Last Modified: Thu, 27 Feb 2020 05:55:58 GMT  
		Size: 158.3 MB (158263721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bd512f7102a2793a61a194251288014c655138b3f7bc8f9b7f6ce98a037e0d`  
		Last Modified: Thu, 27 Feb 2020 05:55:30 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; arm variant v5

```console
$ docker pull plone@sha256:f1ee2e2cf24e672ab9d950a816efd14c229edcadd2f1f4e7ff1d494969eb47ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.2 MB (204187751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701fabf98700b541e80f72ac32cfd6579de85841d6f46ee50b198971aad428b3`
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
# Wed, 26 Feb 2020 07:43:10 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 07:53:26 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 07:53:29 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 07:53:30 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 07:53:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 07:53:31 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 07:54:04 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 07:54:05 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 16:34:34 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 16:34:35 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 16:34:38 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 16:34:39 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 16:49:53 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 16:50:02 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 16:50:03 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 16:50:04 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 16:50:04 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 16:50:05 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 16:50:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 16:50:06 GMT
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
	-	`sha256:d656f5a68dce32db0da25657fa8145509090dd717db0863e3db4a1311d35cad7`  
		Last Modified: Wed, 26 Feb 2020 09:52:39 GMT  
		Size: 22.8 MB (22770271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe441b54bc0ba71262311bc0d52e1668eeac33128e8f36c6af8fa3e6f331b17`  
		Last Modified: Wed, 26 Feb 2020 09:52:31 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595aaeb76d185f5074015b02211536772493bf063be415920a206b07df589942`  
		Last Modified: Wed, 26 Feb 2020 09:52:32 GMT  
		Size: 2.2 MB (2175913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c00d302ea0af84737c436e4cb35da3708abe19235483300dcd58d85b2e9b1b`  
		Last Modified: Wed, 26 Feb 2020 17:05:07 GMT  
		Size: 3.9 KB (3925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abee76f1efce0ea1da36f0f2989c826993ed3ea2e50b6d09bc9b1835b05e1b0`  
		Last Modified: Wed, 26 Feb 2020 17:05:07 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862e034aab772fc7287991f2c52184c8a9ff9aa92f6c16b043211519c0194e49`  
		Last Modified: Wed, 26 Feb 2020 17:06:08 GMT  
		Size: 155.8 MB (155786269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de48e91c45e20dca818e2dcaf7e5caba591beeab6628b545b31b8e0b068d9ada`  
		Last Modified: Wed, 26 Feb 2020 17:05:07 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; arm variant v7

```console
$ docker pull plone@sha256:214303debdcd61422d269ee7b40b0b4da11af7c3295724f5561d92081892d525
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.5 MB (201472309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16474bc9c1a41eb8c1eebd8f52c7f821e1c21ae48d47289152b4c30c6837e247`
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
# Wed, 26 Feb 2020 10:10:24 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 10:23:19 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 10:23:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 10:23:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 10:23:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 10:23:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 10:23:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 10:23:52 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 23:21:11 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 23:21:12 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 23:21:16 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 23:21:17 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 23:34:21 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 23:34:28 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 23:34:29 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 23:34:29 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 23:34:30 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 23:34:31 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 23:34:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 23:34:32 GMT
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
	-	`sha256:6b2b245c7a0af359854db6ff69d5961cf78220a90f0c35e133f8b1c193b64b2c`  
		Last Modified: Wed, 26 Feb 2020 12:27:59 GMT  
		Size: 23.3 MB (23341944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa24266bc1f7d33a53425b488668c6f12d9119b321df759e07b7511c5a0cf057`  
		Last Modified: Wed, 26 Feb 2020 12:27:49 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb838bd6d171e306f9a7bae4693aa12f8b3661bb1513744488d25cbefbecc34`  
		Last Modified: Wed, 26 Feb 2020 12:27:50 GMT  
		Size: 2.2 MB (2175955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b22b8976660ae5dd1d3a6e3b9fd151b01613f6851f628848d2319d2cd3d687e`  
		Last Modified: Wed, 26 Feb 2020 23:47:42 GMT  
		Size: 3.9 KB (3927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ece09e7454f28201a9b11ea15b4c65bff449a93cdc594127208114975c26b7`  
		Last Modified: Wed, 26 Feb 2020 23:47:42 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82da71967ea508b1c336249654a489de13b1c340e27a3277f2b2c3b76bc5afd6`  
		Last Modified: Wed, 26 Feb 2020 23:48:38 GMT  
		Size: 154.5 MB (154470319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0fd9bb5d13ee64e18385cbb3953e7e18cddc8db731d536a0f1e73041ccac18`  
		Last Modified: Wed, 26 Feb 2020 23:47:41 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:1f7389070d10279c0672d02cea678b9e2a62f5a07c430516f108f0bc63ccdcaa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.8 MB (204756651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9bc590e017ec955cbddb1164ce1f21a67e5c9b4d2de4da4d287e46b8df8503`
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
# Wed, 26 Feb 2020 16:31:07 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 16:43:32 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 16:43:34 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 16:43:35 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 16:43:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 16:43:36 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 16:44:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 16:44:01 GMT
CMD ["python3"]
# Thu, 27 Feb 2020 04:12:36 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 04:12:37 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 04:12:39 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 04:12:40 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 04:26:07 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 04:26:13 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 04:26:14 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 04:26:15 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 04:26:16 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 04:26:16 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 04:26:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 04:26:18 GMT
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
	-	`sha256:7a935d604f767a1b217bfe7f9d447c14b71eb5374ffa8278a1a2b2c3ade4b8d4`  
		Last Modified: Wed, 26 Feb 2020 18:37:47 GMT  
		Size: 24.6 MB (24642485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2c221be0fd5417f9d1b382f04d0be0c23decf3862a18be2557a5ada8b38a81`  
		Last Modified: Wed, 26 Feb 2020 18:37:38 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f859a56ff0ad189b82614fc47d2db5777e932e063ad0a077d771c825fbc0a18`  
		Last Modified: Wed, 26 Feb 2020 18:37:39 GMT  
		Size: 2.2 MB (2175818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaeb4713261f88d7096432170cbb67ead5bfd0fdcb56f3e734b3c15854d978`  
		Last Modified: Thu, 27 Feb 2020 04:40:29 GMT  
		Size: 3.9 KB (3938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6501e3434223e00219cc740175867bfe7ffa66bff8732bcfe605e4b583b3b1ed`  
		Last Modified: Thu, 27 Feb 2020 04:40:29 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12efba0f87b7801cf9ecc73d27a8912b48fe5cd541de54acc680f2ebe50870a`  
		Last Modified: Thu, 27 Feb 2020 04:41:15 GMT  
		Size: 155.3 MB (155321506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a7147a31133fdd8d62354a465c24571ddd88266d90240fea63ae932a5f1e82`  
		Last Modified: Thu, 27 Feb 2020 04:40:29 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; 386

```console
$ docker pull plone@sha256:7156ed5eed6a8d9d2e803ea06f9190a7865460c779ecbd513f4b9e0b94ce0d21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.5 MB (210547897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21f43ffd375048752eaaf0c8a0b5e5a9908d68a58b3bc64e76068bb0943c87e7`
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
# Wed, 26 Feb 2020 13:32:29 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 13:46:05 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 13:46:06 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 13:46:06 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 13:46:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 13:46:07 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 13:46:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 13:46:24 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 20:16:25 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 20:16:25 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 20:16:26 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 20:16:26 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 20:20:57 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 20:20:58 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 20:20:58 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 20:20:58 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 20:20:58 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 20:20:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 20:20:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 20:20:59 GMT
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
	-	`sha256:348e763dadfd1b50ff2edb8db5bfc850d30d36ecc064bb59619b6c6d6907e0ee`  
		Last Modified: Wed, 26 Feb 2020 15:50:16 GMT  
		Size: 24.2 MB (24220228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddab4eecfc9a7a10fccdd0e8bab77fd7b8ee7fb0071010573940c23c7628670`  
		Last Modified: Wed, 26 Feb 2020 15:50:09 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e48df556a7b9278e2d994e723c841a90b489f0402a453ba8431053380219fbc`  
		Last Modified: Wed, 26 Feb 2020 15:50:10 GMT  
		Size: 2.2 MB (2175788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e4005781a4394f5c90bc432850f94859e490bb5f21717f2e6b932ff6a191d2`  
		Last Modified: Wed, 26 Feb 2020 20:26:21 GMT  
		Size: 3.9 KB (3873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0ec73ea37c1efe7f599ed0256171c4652822b56fe58b4481980beae0bd309a`  
		Last Modified: Wed, 26 Feb 2020 20:26:21 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc6846fa93309fbbafd84b2465c4259e8b48e8e3f0f7ae193a7170be3fd43de`  
		Last Modified: Wed, 26 Feb 2020 20:27:18 GMT  
		Size: 158.5 MB (158469826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d833dfe4555374e8ab4eceabe08d85851e659e6a0eba6711ee0a0f924dc8dcd0`  
		Last Modified: Wed, 26 Feb 2020 20:26:21 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2` - linux; ppc64le

```console
$ docker pull plone@sha256:17c4307890f9a856016b666c7061b3e0b5a1eea5fb8a8cde982151717aefb96d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.8 MB (209783941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d2fe8cfe5a13c4b275bc426038eec3858c7357395e5ee4effe9119a5540e8ea`
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
# Wed, 26 Feb 2020 04:02:38 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 04:18:08 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 04:18:16 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 04:18:18 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 04:18:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 04:18:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 04:19:18 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 04:19:21 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 20:47:42 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 20:47:45 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 20:47:56 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 20:47:57 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 21:06:50 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 21:06:57 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 21:06:59 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 21:07:01 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 21:07:04 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 21:07:07 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 21:07:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 21:07:13 GMT
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
	-	`sha256:af1513bf2ee03f2207d52345cb8aab950ec5068ec549b6cc088883cbca15f589`  
		Last Modified: Wed, 26 Feb 2020 06:05:30 GMT  
		Size: 25.9 MB (25876486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b3c1956c8f7efa590d60fe60b38ae14e16d52e0cf761a027fa508bdcc6e9c3`  
		Last Modified: Wed, 26 Feb 2020 06:05:22 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d06518c1d2db54727f6703bbbb53ca3d6c455f37698b29ac36e7f56aa8072b`  
		Last Modified: Wed, 26 Feb 2020 06:05:29 GMT  
		Size: 2.2 MB (2177157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0979f1e8cf6dcc2466de7ff88c1da8b24f21d1981cf323a1357100177df72`  
		Last Modified: Wed, 26 Feb 2020 21:29:59 GMT  
		Size: 3.9 KB (3938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d7021169b65fe3a0fe29d0b106245899e94afccee671744aa0b78f29a77479`  
		Last Modified: Wed, 26 Feb 2020 21:29:59 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb31f56f89b4d9ddf929bc79a25c705f4ea472b254a66931f16eb372ddb207f`  
		Last Modified: Wed, 26 Feb 2020 21:34:15 GMT  
		Size: 156.7 MB (156744482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d994590772d0ed4543da406d847fbd2362b5c00f00a8e39a6858fe972dc7a70d`  
		Last Modified: Wed, 26 Feb 2020 21:29:59 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2.1`

```console
$ docker pull plone@sha256:3598db582fd18e0e79067a869f63c8bc063cee5fd9c01c40ee01f625944a3a0c
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
$ docker pull plone@sha256:ceb59901e866ec67d66005ef2f747b98cf6c13962b89bd96a24d8acb2dbb4a56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211290985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0dc524b96661924ba6b46ef04c6fe07f5e7da04ee95116822a7ec8d128f114b`
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
# Wed, 26 Feb 2020 15:55:25 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 16:05:21 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 16:05:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 16:05:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 16:05:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 16:05:24 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 16:05:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 16:05:44 GMT
CMD ["python3"]
# Thu, 27 Feb 2020 05:48:05 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 05:48:05 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 05:48:06 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 05:48:06 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 05:51:37 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 05:51:38 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 05:51:38 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 05:51:39 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 05:51:39 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 05:51:39 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 05:51:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 05:51:39 GMT
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
	-	`sha256:6a33999da14c835e8d3ddcef893fa350153761194bdad1c4a5ee5aa0be90f99c`  
		Last Modified: Wed, 26 Feb 2020 17:48:44 GMT  
		Size: 25.8 MB (25798778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66020c9836480d0db8f94f2acc77f32bf2dd3063a10f4d1d20de5b149009ef4`  
		Last Modified: Wed, 26 Feb 2020 17:48:38 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4703522495058fef344d4879a78cca1e9e153944cee3f036a8ab1ecae6dd839`  
		Last Modified: Wed, 26 Feb 2020 17:48:38 GMT  
		Size: 2.2 MB (2176130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e763c27664adfe48dfa0c2e91cfbb1f2526dd6282a1f2c05d9f93805b66e6b`  
		Last Modified: Thu, 27 Feb 2020 05:55:31 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d47d7fdaea68eeb5b75b87786b64e2b50ef6147dd07c686e7b21488a14f260`  
		Last Modified: Thu, 27 Feb 2020 05:55:31 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68114f24f65e8d32aecc6b595c0ab1d22dec7865ea29a09a06793330c2b6787f`  
		Last Modified: Thu, 27 Feb 2020 05:55:58 GMT  
		Size: 158.3 MB (158263721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bd512f7102a2793a61a194251288014c655138b3f7bc8f9b7f6ce98a037e0d`  
		Last Modified: Thu, 27 Feb 2020 05:55:30 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1` - linux; arm variant v5

```console
$ docker pull plone@sha256:f1ee2e2cf24e672ab9d950a816efd14c229edcadd2f1f4e7ff1d494969eb47ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.2 MB (204187751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701fabf98700b541e80f72ac32cfd6579de85841d6f46ee50b198971aad428b3`
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
# Wed, 26 Feb 2020 07:43:10 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 07:53:26 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 07:53:29 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 07:53:30 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 07:53:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 07:53:31 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 07:54:04 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 07:54:05 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 16:34:34 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 16:34:35 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 16:34:38 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 16:34:39 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 16:49:53 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 16:50:02 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 16:50:03 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 16:50:04 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 16:50:04 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 16:50:05 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 16:50:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 16:50:06 GMT
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
	-	`sha256:d656f5a68dce32db0da25657fa8145509090dd717db0863e3db4a1311d35cad7`  
		Last Modified: Wed, 26 Feb 2020 09:52:39 GMT  
		Size: 22.8 MB (22770271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe441b54bc0ba71262311bc0d52e1668eeac33128e8f36c6af8fa3e6f331b17`  
		Last Modified: Wed, 26 Feb 2020 09:52:31 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595aaeb76d185f5074015b02211536772493bf063be415920a206b07df589942`  
		Last Modified: Wed, 26 Feb 2020 09:52:32 GMT  
		Size: 2.2 MB (2175913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c00d302ea0af84737c436e4cb35da3708abe19235483300dcd58d85b2e9b1b`  
		Last Modified: Wed, 26 Feb 2020 17:05:07 GMT  
		Size: 3.9 KB (3925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abee76f1efce0ea1da36f0f2989c826993ed3ea2e50b6d09bc9b1835b05e1b0`  
		Last Modified: Wed, 26 Feb 2020 17:05:07 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862e034aab772fc7287991f2c52184c8a9ff9aa92f6c16b043211519c0194e49`  
		Last Modified: Wed, 26 Feb 2020 17:06:08 GMT  
		Size: 155.8 MB (155786269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de48e91c45e20dca818e2dcaf7e5caba591beeab6628b545b31b8e0b068d9ada`  
		Last Modified: Wed, 26 Feb 2020 17:05:07 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1` - linux; arm variant v7

```console
$ docker pull plone@sha256:214303debdcd61422d269ee7b40b0b4da11af7c3295724f5561d92081892d525
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.5 MB (201472309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16474bc9c1a41eb8c1eebd8f52c7f821e1c21ae48d47289152b4c30c6837e247`
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
# Wed, 26 Feb 2020 10:10:24 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 10:23:19 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 10:23:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 10:23:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 10:23:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 10:23:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 10:23:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 10:23:52 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 23:21:11 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 23:21:12 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 23:21:16 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 23:21:17 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 23:34:21 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 23:34:28 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 23:34:29 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 23:34:29 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 23:34:30 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 23:34:31 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 23:34:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 23:34:32 GMT
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
	-	`sha256:6b2b245c7a0af359854db6ff69d5961cf78220a90f0c35e133f8b1c193b64b2c`  
		Last Modified: Wed, 26 Feb 2020 12:27:59 GMT  
		Size: 23.3 MB (23341944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa24266bc1f7d33a53425b488668c6f12d9119b321df759e07b7511c5a0cf057`  
		Last Modified: Wed, 26 Feb 2020 12:27:49 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb838bd6d171e306f9a7bae4693aa12f8b3661bb1513744488d25cbefbecc34`  
		Last Modified: Wed, 26 Feb 2020 12:27:50 GMT  
		Size: 2.2 MB (2175955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b22b8976660ae5dd1d3a6e3b9fd151b01613f6851f628848d2319d2cd3d687e`  
		Last Modified: Wed, 26 Feb 2020 23:47:42 GMT  
		Size: 3.9 KB (3927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ece09e7454f28201a9b11ea15b4c65bff449a93cdc594127208114975c26b7`  
		Last Modified: Wed, 26 Feb 2020 23:47:42 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82da71967ea508b1c336249654a489de13b1c340e27a3277f2b2c3b76bc5afd6`  
		Last Modified: Wed, 26 Feb 2020 23:48:38 GMT  
		Size: 154.5 MB (154470319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0fd9bb5d13ee64e18385cbb3953e7e18cddc8db731d536a0f1e73041ccac18`  
		Last Modified: Wed, 26 Feb 2020 23:47:41 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:1f7389070d10279c0672d02cea678b9e2a62f5a07c430516f108f0bc63ccdcaa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.8 MB (204756651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9bc590e017ec955cbddb1164ce1f21a67e5c9b4d2de4da4d287e46b8df8503`
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
# Wed, 26 Feb 2020 16:31:07 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 16:43:32 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 16:43:34 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 16:43:35 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 16:43:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 16:43:36 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 16:44:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 16:44:01 GMT
CMD ["python3"]
# Thu, 27 Feb 2020 04:12:36 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 04:12:37 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 04:12:39 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 04:12:40 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 04:26:07 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 04:26:13 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 04:26:14 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 04:26:15 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 04:26:16 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 04:26:16 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 04:26:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 04:26:18 GMT
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
	-	`sha256:7a935d604f767a1b217bfe7f9d447c14b71eb5374ffa8278a1a2b2c3ade4b8d4`  
		Last Modified: Wed, 26 Feb 2020 18:37:47 GMT  
		Size: 24.6 MB (24642485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2c221be0fd5417f9d1b382f04d0be0c23decf3862a18be2557a5ada8b38a81`  
		Last Modified: Wed, 26 Feb 2020 18:37:38 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f859a56ff0ad189b82614fc47d2db5777e932e063ad0a077d771c825fbc0a18`  
		Last Modified: Wed, 26 Feb 2020 18:37:39 GMT  
		Size: 2.2 MB (2175818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaeb4713261f88d7096432170cbb67ead5bfd0fdcb56f3e734b3c15854d978`  
		Last Modified: Thu, 27 Feb 2020 04:40:29 GMT  
		Size: 3.9 KB (3938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6501e3434223e00219cc740175867bfe7ffa66bff8732bcfe605e4b583b3b1ed`  
		Last Modified: Thu, 27 Feb 2020 04:40:29 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12efba0f87b7801cf9ecc73d27a8912b48fe5cd541de54acc680f2ebe50870a`  
		Last Modified: Thu, 27 Feb 2020 04:41:15 GMT  
		Size: 155.3 MB (155321506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a7147a31133fdd8d62354a465c24571ddd88266d90240fea63ae932a5f1e82`  
		Last Modified: Thu, 27 Feb 2020 04:40:29 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1` - linux; 386

```console
$ docker pull plone@sha256:7156ed5eed6a8d9d2e803ea06f9190a7865460c779ecbd513f4b9e0b94ce0d21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.5 MB (210547897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21f43ffd375048752eaaf0c8a0b5e5a9908d68a58b3bc64e76068bb0943c87e7`
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
# Wed, 26 Feb 2020 13:32:29 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 13:46:05 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 13:46:06 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 13:46:06 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 13:46:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 13:46:07 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 13:46:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 13:46:24 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 20:16:25 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 20:16:25 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 20:16:26 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 20:16:26 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 20:20:57 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 20:20:58 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 20:20:58 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 20:20:58 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 20:20:58 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 20:20:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 20:20:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 20:20:59 GMT
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
	-	`sha256:348e763dadfd1b50ff2edb8db5bfc850d30d36ecc064bb59619b6c6d6907e0ee`  
		Last Modified: Wed, 26 Feb 2020 15:50:16 GMT  
		Size: 24.2 MB (24220228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddab4eecfc9a7a10fccdd0e8bab77fd7b8ee7fb0071010573940c23c7628670`  
		Last Modified: Wed, 26 Feb 2020 15:50:09 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e48df556a7b9278e2d994e723c841a90b489f0402a453ba8431053380219fbc`  
		Last Modified: Wed, 26 Feb 2020 15:50:10 GMT  
		Size: 2.2 MB (2175788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e4005781a4394f5c90bc432850f94859e490bb5f21717f2e6b932ff6a191d2`  
		Last Modified: Wed, 26 Feb 2020 20:26:21 GMT  
		Size: 3.9 KB (3873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0ec73ea37c1efe7f599ed0256171c4652822b56fe58b4481980beae0bd309a`  
		Last Modified: Wed, 26 Feb 2020 20:26:21 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc6846fa93309fbbafd84b2465c4259e8b48e8e3f0f7ae193a7170be3fd43de`  
		Last Modified: Wed, 26 Feb 2020 20:27:18 GMT  
		Size: 158.5 MB (158469826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d833dfe4555374e8ab4eceabe08d85851e659e6a0eba6711ee0a0f924dc8dcd0`  
		Last Modified: Wed, 26 Feb 2020 20:26:21 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1` - linux; ppc64le

```console
$ docker pull plone@sha256:17c4307890f9a856016b666c7061b3e0b5a1eea5fb8a8cde982151717aefb96d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.8 MB (209783941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d2fe8cfe5a13c4b275bc426038eec3858c7357395e5ee4effe9119a5540e8ea`
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
# Wed, 26 Feb 2020 04:02:38 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 04:18:08 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 04:18:16 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 04:18:18 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 04:18:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 04:18:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 04:19:18 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 04:19:21 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 20:47:42 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 20:47:45 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 20:47:56 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 20:47:57 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 21:06:50 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 21:06:57 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 21:06:59 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 21:07:01 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 21:07:04 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 21:07:07 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 21:07:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 21:07:13 GMT
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
	-	`sha256:af1513bf2ee03f2207d52345cb8aab950ec5068ec549b6cc088883cbca15f589`  
		Last Modified: Wed, 26 Feb 2020 06:05:30 GMT  
		Size: 25.9 MB (25876486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b3c1956c8f7efa590d60fe60b38ae14e16d52e0cf761a027fa508bdcc6e9c3`  
		Last Modified: Wed, 26 Feb 2020 06:05:22 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d06518c1d2db54727f6703bbbb53ca3d6c455f37698b29ac36e7f56aa8072b`  
		Last Modified: Wed, 26 Feb 2020 06:05:29 GMT  
		Size: 2.2 MB (2177157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0979f1e8cf6dcc2466de7ff88c1da8b24f21d1981cf323a1357100177df72`  
		Last Modified: Wed, 26 Feb 2020 21:29:59 GMT  
		Size: 3.9 KB (3938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d7021169b65fe3a0fe29d0b106245899e94afccee671744aa0b78f29a77479`  
		Last Modified: Wed, 26 Feb 2020 21:29:59 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb31f56f89b4d9ddf929bc79a25c705f4ea472b254a66931f16eb372ddb207f`  
		Last Modified: Wed, 26 Feb 2020 21:34:15 GMT  
		Size: 156.7 MB (156744482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d994590772d0ed4543da406d847fbd2362b5c00f00a8e39a6858fe972dc7a70d`  
		Last Modified: Wed, 26 Feb 2020 21:29:59 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:5.2.1-alpine`

```console
$ docker pull plone@sha256:9d26bf42175e073f2d43a8e306f3d56f09feb51d195f9c34bf783b255463ba69
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
$ docker pull plone@sha256:b73b0018004aa08ba04c658453b57363f046354ea73ccbac27b6d3c10daa031b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.6 MB (167603380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:495fedeb528f4a81a23475277826be9efd9e4a03f22e80b70feeb6d6b7efa4ea`
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
# Sat, 18 Jan 2020 02:43:48 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:51:40 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:51:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 02:51:16 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:38:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:38:21 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:38:28 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:38:28 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 02:23:18 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 02:23:18 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 02:23:19 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 02:23:19 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 02:31:44 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 02:31:45 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 02:31:45 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 02:31:45 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 02:31:45 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 02:31:45 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 02:31:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 02:31:46 GMT
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
	-	`sha256:53a2fca3c2ea7aa6237addb6763b98a5dfdc15c3a0f33222f9b206d5acac0b91`  
		Last Modified: Sat, 18 Jan 2020 03:11:30 GMT  
		Size: 28.7 MB (28689845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fce49de8b1e8a52f778591ddbf56241326e2d3f3aea9afa3f2d28939ed1fbd`  
		Last Modified: Sat, 18 Jan 2020 03:11:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca406aaf66e09244c9cabb69523721a85751dac98c452dea02390395c5a212df`  
		Last Modified: Thu, 06 Feb 2020 01:44:29 GMT  
		Size: 1.9 MB (1892190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050bda448ba7c14f4ae8fa6f05e2e5001de0b7664375bc0f3277b185b8dd3afe`  
		Last Modified: Thu, 06 Feb 2020 02:36:18 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b823874a3e0e70868ec3182d708c4a41d63310e987680e66f8cd12c3ce34d2`  
		Last Modified: Thu, 06 Feb 2020 02:36:18 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abbf8d18f9e5482e835ffce6a58ade3390522430db489738a84eedf716fee32`  
		Last Modified: Thu, 06 Feb 2020 02:37:13 GMT  
		Size: 133.9 MB (133911926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ccc5c7b3b031094f84969221fbde349bdd3c0e05dc998cb3a99c680c4aa13f`  
		Last Modified: Thu, 06 Feb 2020 02:36:18 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:c4ad99dd2a9e61dbf46a8f22007a3d798560415180ceca57e479826947a8b386
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.9 MB (164907993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4206e1b5bb03314c228aaee3c2dc74548d9512dcf5110a500e9ab1148092b7c6`
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
# Sat, 18 Jan 2020 04:50:12 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 05:06:53 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 05:07:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:53:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:39:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:39:19 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:39:33 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:39:34 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 02:09:44 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 02:09:44 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 02:09:46 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 02:09:47 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 02:30:07 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 02:30:12 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 02:30:13 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 02:30:14 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 02:30:16 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 02:30:17 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 02:30:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 02:30:21 GMT
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
	-	`sha256:aebbc07e72ffbabc6d0ea65ef24ded7dedd55b70faed4aa7235f61e0c6dc0478`  
		Last Modified: Sat, 18 Jan 2020 05:44:23 GMT  
		Size: 26.7 MB (26726326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ccfccce4f40de4c690f1c4c953215c68bf6d9edbeaa444c40d9a220fe7c694`  
		Last Modified: Sat, 18 Jan 2020 05:44:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081556640fdf47a0865f131ba1ff89e9774a48d2552816afd56ded95c240be36`  
		Last Modified: Thu, 06 Feb 2020 01:44:33 GMT  
		Size: 1.9 MB (1892487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132f9f541686c1d5f5db650675cbd1a42e4757e43dd6e7b3a3a07dff4b9fc9cd`  
		Last Modified: Thu, 06 Feb 2020 02:30:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6162e73e5521785fca9fe0c2e87bed2bb19cee2fa6e157f8c57873a36fb32e`  
		Last Modified: Thu, 06 Feb 2020 02:30:38 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2451f229c978d1820e81f1e1ae2c6987ec284088e537a1b965465f0d178cb4`  
		Last Modified: Thu, 06 Feb 2020 02:32:24 GMT  
		Size: 133.4 MB (133364728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfbf2b49771c341da99951ab3af1e1083ced861e14baa6c8660bb6d039654d5`  
		Last Modified: Thu, 06 Feb 2020 02:30:38 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:b8de73d598630e403e648ab2ee0766db6dbe103cae87f49d522a2a6953b95cb4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.8 MB (166775914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6eb3797f2fd9195d4689504752402b054150c3994d6d2767100d056867e818`
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
# Sat, 18 Jan 2020 03:31:27 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 03:45:43 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 03:45:55 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 02:15:46 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:54:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:54:37 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:54:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:54:53 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 03:36:21 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 03:36:22 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 03:36:23 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 03:36:24 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 03:54:30 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 03:54:34 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 03:54:35 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 03:54:36 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 03:54:36 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 03:54:37 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 03:54:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 03:54:38 GMT
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
	-	`sha256:b4d853162255da370dbadaff288bb9f1d3903c095741010d25e14aa51fb0df2e`  
		Last Modified: Sat, 18 Jan 2020 04:19:04 GMT  
		Size: 28.2 MB (28192647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a396952f54f422d45ba879b0f6a69920e7fa88f932f020242c7e3d59058c48d6`  
		Last Modified: Sat, 18 Jan 2020 04:18:54 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4e8ba8a523242d7ae1f4aff8e7099f660f86b5782fef744336a667f1a4087d`  
		Last Modified: Thu, 06 Feb 2020 02:11:19 GMT  
		Size: 1.9 MB (1892503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdacff862803686cab92a2a12e6d56e3e061aa2022ee12d2d62b4498ea173db`  
		Last Modified: Thu, 06 Feb 2020 04:09:46 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4e1afc585605f90af813e5a830a154c8bd15f5eb8b3a1e164585f707649e64`  
		Last Modified: Thu, 06 Feb 2020 04:09:45 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f47c6820783296d753715ea94dab8728a6ceb909e8e9e6cc5fd8be509138e3`  
		Last Modified: Thu, 06 Feb 2020 04:10:56 GMT  
		Size: 133.7 MB (133660666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3ccf36f0a15835cb8ce12b772e2f99aca7e5f6099b239483b93b9e2e788810`  
		Last Modified: Thu, 06 Feb 2020 04:09:46 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-alpine` - linux; 386

```console
$ docker pull plone@sha256:bf31fdbf1f4d199115a23c5c3be3889ce8c81b40cb317a9a5ac0164d5b40fc0d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165565521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56a77edbdae9b52c7f7e2c51ed41a2813afde9ca90c2c1e6ae89a9ca6aa6ef8`
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
# Sat, 18 Jan 2020 02:07:04 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:19:45 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:19:46 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:58:55 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 00:49:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 00:49:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 00:49:13 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 00:49:13 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 01:37:55 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 01:37:55 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 01:37:56 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 01:37:56 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 01:48:53 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 01:48:55 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 01:48:55 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 01:48:56 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 01:48:56 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 01:48:57 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 01:48:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 01:48:57 GMT
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
	-	`sha256:ae5ce9d316aa4df2055853b0491ee281a07f3f59665bb923a35e4538259fafe4`  
		Last Modified: Sat, 18 Jan 2020 05:38:02 GMT  
		Size: 27.2 MB (27204546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042a4df44aa41c2b54d88fe0f00920dae6f7eafd7e087027bab618b4912ecfc`  
		Last Modified: Sat, 18 Jan 2020 05:37:54 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a08247c30e77b055b7b8ddf2cfb3a02c68333956507dd96f12abfa49f1f7c0f`  
		Last Modified: Thu, 06 Feb 2020 00:56:36 GMT  
		Size: 1.9 MB (1892251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a323f5d6868cf70fbc1491873064f97448096f5c259b6d3a938787bb6b9996d`  
		Last Modified: Thu, 06 Feb 2020 01:57:03 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552813d6ae47a688a0cad95b973bbfcd0115af8ac7f9df47653876f9bba4bfa5`  
		Last Modified: Thu, 06 Feb 2020 01:57:03 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1f9aba7b6eae397db855925cf7f8eab7f4b09230a79f62991ef2c1a80aa031`  
		Last Modified: Thu, 06 Feb 2020 01:57:50 GMT  
		Size: 133.4 MB (133355054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a788b90738187646f8348d43ab52f688259e467e9a10f01129704615c2ead4d`  
		Last Modified: Thu, 06 Feb 2020 01:57:03 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:d8fd8495c45b8b9f78bfc6f44ef9e4fb79fc7e0eff56f1c0a59fabf421d1b752
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169056884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba8a6f58b3af1bb5e6c697e52e4a21f0cbd456843d96f84d67e89d4f54ff62fa`
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
# Sat, 18 Jan 2020 05:06:33 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 05:18:22 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 05:18:29 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 02:38:30 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:31:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:31:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:31:47 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:31:51 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 02:51:44 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 02:51:46 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 02:51:56 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 02:51:57 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 03:07:40 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 03:07:48 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 03:07:50 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 03:07:53 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 03:07:56 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 03:07:58 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 03:08:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 03:08:04 GMT
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
	-	`sha256:9f5d173893fbe54a062519b8ef5d68403a697a00c4c8741ea641e742dd41862a`  
		Last Modified: Sat, 18 Jan 2020 05:46:19 GMT  
		Size: 29.6 MB (29612538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030ea3db62c6d8771ba19ecee7109a97439e647e0e25356096f6f7aad6dd2e04`  
		Last Modified: Sat, 18 Jan 2020 05:46:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bde1575b2c7098a717fde701a00a7d2ff87b57de35c5a05cfe0ef1b8eddf51`  
		Last Modified: Thu, 06 Feb 2020 01:52:32 GMT  
		Size: 1.9 MB (1892522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089c1e6255322429c9764c5aaf56595ea92e8aea94595d2ae8db33e47f4ac98a`  
		Last Modified: Thu, 06 Feb 2020 03:28:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06be0137416a9df9b42aae289f6e95730348856ee1c5e64ecf73c2c231aec25`  
		Last Modified: Thu, 06 Feb 2020 03:28:10 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cb69c6d827fc2558f8943eab2da793b84beeb7ad2531268964477ecde9342f`  
		Last Modified: Thu, 06 Feb 2020 03:29:37 GMT  
		Size: 134.4 MB (134420448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416a144bb270c6ea27ef44de61e6faf957d91b37bdef99fc728e35f1170b2197`  
		Last Modified: Thu, 06 Feb 2020 03:28:10 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2.1-alpine` - linux; s390x

```console
$ docker pull plone@sha256:9ccd0aff5954e7b8041056369e02d6fa2df67b558a4f1a49d73503367c355a18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167856958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9016c845f528be148a21d9ad7960888a0eb978970eb2e8bba2a82f1677d2ede1`
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
# Sat, 25 Jan 2020 01:52:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/42ad3426cb1ef05863521d7988d5f7fec0c99560/get-pip.py
# Sat, 25 Jan 2020 01:52:23 GMT
ENV PYTHON_GET_PIP_SHA256=da288fc002d0bb2b90f6fbabc91048c1fa18d567ad067ee713c6e331d3a32b45
# Sat, 25 Jan 2020 01:52:27 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 25 Jan 2020 01:52:27 GMT
CMD ["python3"]
# Thu, 30 Jan 2020 23:09:56 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 30 Jan 2020 23:09:56 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 30 Jan 2020 23:09:57 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 30 Jan 2020 23:09:57 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 30 Jan 2020 23:16:19 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 30 Jan 2020 23:16:28 GMT
VOLUME [/data]
# Thu, 30 Jan 2020 23:16:28 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 30 Jan 2020 23:16:28 GMT
EXPOSE 8080
# Thu, 30 Jan 2020 23:16:29 GMT
WORKDIR /plone/instance
# Thu, 30 Jan 2020 23:16:29 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 30 Jan 2020 23:16:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:16:29 GMT
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
	-	`sha256:1997174415ba324b2612ca12762fb1dec19c25b34ee9cc34897cb678bafcbe19`  
		Last Modified: Sat, 25 Jan 2020 01:57:54 GMT  
		Size: 1.9 MB (1887363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e137422f32895097ef542b97feed35cdfd5666da0d2b7287f5eaa60d12a9ab`  
		Last Modified: Thu, 30 Jan 2020 23:31:05 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73988218a40a1217b0569567ddb67c61444a1485c5bb26c6dcdb118cdbfca76`  
		Last Modified: Thu, 30 Jan 2020 23:31:11 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973926f54c6dd626dbc9f6923d102074d3ed09a79a4bfafd0b7f80c96321e9a`  
		Last Modified: Thu, 30 Jan 2020 23:31:24 GMT  
		Size: 134.1 MB (134140072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1086dbcd802262647497b67e66504660a7e23e7ad0050e3a794f9009cf71cdd3`  
		Last Modified: Thu, 30 Jan 2020 23:31:05 GMT  
		Size: 2.6 KB (2625 bytes)  
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
$ docker pull plone@sha256:9d26bf42175e073f2d43a8e306f3d56f09feb51d195f9c34bf783b255463ba69
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
$ docker pull plone@sha256:b73b0018004aa08ba04c658453b57363f046354ea73ccbac27b6d3c10daa031b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.6 MB (167603380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:495fedeb528f4a81a23475277826be9efd9e4a03f22e80b70feeb6d6b7efa4ea`
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
# Sat, 18 Jan 2020 02:43:48 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:51:40 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:51:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 02:51:16 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:38:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:38:21 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:38:28 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:38:28 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 02:23:18 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 02:23:18 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 02:23:19 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 02:23:19 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 02:31:44 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 02:31:45 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 02:31:45 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 02:31:45 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 02:31:45 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 02:31:45 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 02:31:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 02:31:46 GMT
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
	-	`sha256:53a2fca3c2ea7aa6237addb6763b98a5dfdc15c3a0f33222f9b206d5acac0b91`  
		Last Modified: Sat, 18 Jan 2020 03:11:30 GMT  
		Size: 28.7 MB (28689845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fce49de8b1e8a52f778591ddbf56241326e2d3f3aea9afa3f2d28939ed1fbd`  
		Last Modified: Sat, 18 Jan 2020 03:11:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca406aaf66e09244c9cabb69523721a85751dac98c452dea02390395c5a212df`  
		Last Modified: Thu, 06 Feb 2020 01:44:29 GMT  
		Size: 1.9 MB (1892190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050bda448ba7c14f4ae8fa6f05e2e5001de0b7664375bc0f3277b185b8dd3afe`  
		Last Modified: Thu, 06 Feb 2020 02:36:18 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b823874a3e0e70868ec3182d708c4a41d63310e987680e66f8cd12c3ce34d2`  
		Last Modified: Thu, 06 Feb 2020 02:36:18 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abbf8d18f9e5482e835ffce6a58ade3390522430db489738a84eedf716fee32`  
		Last Modified: Thu, 06 Feb 2020 02:37:13 GMT  
		Size: 133.9 MB (133911926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ccc5c7b3b031094f84969221fbde349bdd3c0e05dc998cb3a99c680c4aa13f`  
		Last Modified: Thu, 06 Feb 2020 02:36:18 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:c4ad99dd2a9e61dbf46a8f22007a3d798560415180ceca57e479826947a8b386
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.9 MB (164907993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4206e1b5bb03314c228aaee3c2dc74548d9512dcf5110a500e9ab1148092b7c6`
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
# Sat, 18 Jan 2020 04:50:12 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 05:06:53 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 05:07:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:53:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:39:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:39:19 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:39:33 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:39:34 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 02:09:44 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 02:09:44 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 02:09:46 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 02:09:47 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 02:30:07 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 02:30:12 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 02:30:13 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 02:30:14 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 02:30:16 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 02:30:17 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 02:30:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 02:30:21 GMT
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
	-	`sha256:aebbc07e72ffbabc6d0ea65ef24ded7dedd55b70faed4aa7235f61e0c6dc0478`  
		Last Modified: Sat, 18 Jan 2020 05:44:23 GMT  
		Size: 26.7 MB (26726326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ccfccce4f40de4c690f1c4c953215c68bf6d9edbeaa444c40d9a220fe7c694`  
		Last Modified: Sat, 18 Jan 2020 05:44:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081556640fdf47a0865f131ba1ff89e9774a48d2552816afd56ded95c240be36`  
		Last Modified: Thu, 06 Feb 2020 01:44:33 GMT  
		Size: 1.9 MB (1892487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132f9f541686c1d5f5db650675cbd1a42e4757e43dd6e7b3a3a07dff4b9fc9cd`  
		Last Modified: Thu, 06 Feb 2020 02:30:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6162e73e5521785fca9fe0c2e87bed2bb19cee2fa6e157f8c57873a36fb32e`  
		Last Modified: Thu, 06 Feb 2020 02:30:38 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2451f229c978d1820e81f1e1ae2c6987ec284088e537a1b965465f0d178cb4`  
		Last Modified: Thu, 06 Feb 2020 02:32:24 GMT  
		Size: 133.4 MB (133364728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfbf2b49771c341da99951ab3af1e1083ced861e14baa6c8660bb6d039654d5`  
		Last Modified: Thu, 06 Feb 2020 02:30:38 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:b8de73d598630e403e648ab2ee0766db6dbe103cae87f49d522a2a6953b95cb4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.8 MB (166775914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6eb3797f2fd9195d4689504752402b054150c3994d6d2767100d056867e818`
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
# Sat, 18 Jan 2020 03:31:27 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 03:45:43 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 03:45:55 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 02:15:46 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:54:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:54:37 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:54:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:54:53 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 03:36:21 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 03:36:22 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 03:36:23 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 03:36:24 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 03:54:30 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 03:54:34 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 03:54:35 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 03:54:36 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 03:54:36 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 03:54:37 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 03:54:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 03:54:38 GMT
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
	-	`sha256:b4d853162255da370dbadaff288bb9f1d3903c095741010d25e14aa51fb0df2e`  
		Last Modified: Sat, 18 Jan 2020 04:19:04 GMT  
		Size: 28.2 MB (28192647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a396952f54f422d45ba879b0f6a69920e7fa88f932f020242c7e3d59058c48d6`  
		Last Modified: Sat, 18 Jan 2020 04:18:54 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4e8ba8a523242d7ae1f4aff8e7099f660f86b5782fef744336a667f1a4087d`  
		Last Modified: Thu, 06 Feb 2020 02:11:19 GMT  
		Size: 1.9 MB (1892503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdacff862803686cab92a2a12e6d56e3e061aa2022ee12d2d62b4498ea173db`  
		Last Modified: Thu, 06 Feb 2020 04:09:46 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4e1afc585605f90af813e5a830a154c8bd15f5eb8b3a1e164585f707649e64`  
		Last Modified: Thu, 06 Feb 2020 04:09:45 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f47c6820783296d753715ea94dab8728a6ceb909e8e9e6cc5fd8be509138e3`  
		Last Modified: Thu, 06 Feb 2020 04:10:56 GMT  
		Size: 133.7 MB (133660666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3ccf36f0a15835cb8ce12b772e2f99aca7e5f6099b239483b93b9e2e788810`  
		Last Modified: Thu, 06 Feb 2020 04:09:46 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; 386

```console
$ docker pull plone@sha256:bf31fdbf1f4d199115a23c5c3be3889ce8c81b40cb317a9a5ac0164d5b40fc0d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165565521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56a77edbdae9b52c7f7e2c51ed41a2813afde9ca90c2c1e6ae89a9ca6aa6ef8`
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
# Sat, 18 Jan 2020 02:07:04 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:19:45 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:19:46 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:58:55 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 00:49:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 00:49:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 00:49:13 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 00:49:13 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 01:37:55 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 01:37:55 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 01:37:56 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 01:37:56 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 01:48:53 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 01:48:55 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 01:48:55 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 01:48:56 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 01:48:56 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 01:48:57 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 01:48:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 01:48:57 GMT
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
	-	`sha256:ae5ce9d316aa4df2055853b0491ee281a07f3f59665bb923a35e4538259fafe4`  
		Last Modified: Sat, 18 Jan 2020 05:38:02 GMT  
		Size: 27.2 MB (27204546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042a4df44aa41c2b54d88fe0f00920dae6f7eafd7e087027bab618b4912ecfc`  
		Last Modified: Sat, 18 Jan 2020 05:37:54 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a08247c30e77b055b7b8ddf2cfb3a02c68333956507dd96f12abfa49f1f7c0f`  
		Last Modified: Thu, 06 Feb 2020 00:56:36 GMT  
		Size: 1.9 MB (1892251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a323f5d6868cf70fbc1491873064f97448096f5c259b6d3a938787bb6b9996d`  
		Last Modified: Thu, 06 Feb 2020 01:57:03 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552813d6ae47a688a0cad95b973bbfcd0115af8ac7f9df47653876f9bba4bfa5`  
		Last Modified: Thu, 06 Feb 2020 01:57:03 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1f9aba7b6eae397db855925cf7f8eab7f4b09230a79f62991ef2c1a80aa031`  
		Last Modified: Thu, 06 Feb 2020 01:57:50 GMT  
		Size: 133.4 MB (133355054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a788b90738187646f8348d43ab52f688259e467e9a10f01129704615c2ead4d`  
		Last Modified: Thu, 06 Feb 2020 01:57:03 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:d8fd8495c45b8b9f78bfc6f44ef9e4fb79fc7e0eff56f1c0a59fabf421d1b752
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169056884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba8a6f58b3af1bb5e6c697e52e4a21f0cbd456843d96f84d67e89d4f54ff62fa`
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
# Sat, 18 Jan 2020 05:06:33 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 05:18:22 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 05:18:29 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 02:38:30 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:31:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:31:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:31:47 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:31:51 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 02:51:44 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 02:51:46 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 02:51:56 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 02:51:57 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 03:07:40 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 03:07:48 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 03:07:50 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 03:07:53 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 03:07:56 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 03:07:58 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 03:08:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 03:08:04 GMT
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
	-	`sha256:9f5d173893fbe54a062519b8ef5d68403a697a00c4c8741ea641e742dd41862a`  
		Last Modified: Sat, 18 Jan 2020 05:46:19 GMT  
		Size: 29.6 MB (29612538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030ea3db62c6d8771ba19ecee7109a97439e647e0e25356096f6f7aad6dd2e04`  
		Last Modified: Sat, 18 Jan 2020 05:46:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bde1575b2c7098a717fde701a00a7d2ff87b57de35c5a05cfe0ef1b8eddf51`  
		Last Modified: Thu, 06 Feb 2020 01:52:32 GMT  
		Size: 1.9 MB (1892522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089c1e6255322429c9764c5aaf56595ea92e8aea94595d2ae8db33e47f4ac98a`  
		Last Modified: Thu, 06 Feb 2020 03:28:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06be0137416a9df9b42aae289f6e95730348856ee1c5e64ecf73c2c231aec25`  
		Last Modified: Thu, 06 Feb 2020 03:28:10 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cb69c6d827fc2558f8943eab2da793b84beeb7ad2531268964477ecde9342f`  
		Last Modified: Thu, 06 Feb 2020 03:29:37 GMT  
		Size: 134.4 MB (134420448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416a144bb270c6ea27ef44de61e6faf957d91b37bdef99fc728e35f1170b2197`  
		Last Modified: Thu, 06 Feb 2020 03:28:10 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5.2-alpine` - linux; s390x

```console
$ docker pull plone@sha256:9ccd0aff5954e7b8041056369e02d6fa2df67b558a4f1a49d73503367c355a18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167856958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9016c845f528be148a21d9ad7960888a0eb978970eb2e8bba2a82f1677d2ede1`
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
# Sat, 25 Jan 2020 01:52:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/42ad3426cb1ef05863521d7988d5f7fec0c99560/get-pip.py
# Sat, 25 Jan 2020 01:52:23 GMT
ENV PYTHON_GET_PIP_SHA256=da288fc002d0bb2b90f6fbabc91048c1fa18d567ad067ee713c6e331d3a32b45
# Sat, 25 Jan 2020 01:52:27 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 25 Jan 2020 01:52:27 GMT
CMD ["python3"]
# Thu, 30 Jan 2020 23:09:56 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 30 Jan 2020 23:09:56 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 30 Jan 2020 23:09:57 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 30 Jan 2020 23:09:57 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 30 Jan 2020 23:16:19 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 30 Jan 2020 23:16:28 GMT
VOLUME [/data]
# Thu, 30 Jan 2020 23:16:28 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 30 Jan 2020 23:16:28 GMT
EXPOSE 8080
# Thu, 30 Jan 2020 23:16:29 GMT
WORKDIR /plone/instance
# Thu, 30 Jan 2020 23:16:29 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 30 Jan 2020 23:16:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:16:29 GMT
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
	-	`sha256:1997174415ba324b2612ca12762fb1dec19c25b34ee9cc34897cb678bafcbe19`  
		Last Modified: Sat, 25 Jan 2020 01:57:54 GMT  
		Size: 1.9 MB (1887363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e137422f32895097ef542b97feed35cdfd5666da0d2b7287f5eaa60d12a9ab`  
		Last Modified: Thu, 30 Jan 2020 23:31:05 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73988218a40a1217b0569567ddb67c61444a1485c5bb26c6dcdb118cdbfca76`  
		Last Modified: Thu, 30 Jan 2020 23:31:11 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973926f54c6dd626dbc9f6923d102074d3ed09a79a4bfafd0b7f80c96321e9a`  
		Last Modified: Thu, 30 Jan 2020 23:31:24 GMT  
		Size: 134.1 MB (134140072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1086dbcd802262647497b67e66504660a7e23e7ad0050e3a794f9009cf71cdd3`  
		Last Modified: Thu, 30 Jan 2020 23:31:05 GMT  
		Size: 2.6 KB (2625 bytes)  
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
$ docker pull plone@sha256:9d26bf42175e073f2d43a8e306f3d56f09feb51d195f9c34bf783b255463ba69
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
$ docker pull plone@sha256:b73b0018004aa08ba04c658453b57363f046354ea73ccbac27b6d3c10daa031b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.6 MB (167603380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:495fedeb528f4a81a23475277826be9efd9e4a03f22e80b70feeb6d6b7efa4ea`
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
# Sat, 18 Jan 2020 02:43:48 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:51:40 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:51:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 02:51:16 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:38:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:38:21 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:38:28 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:38:28 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 02:23:18 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 02:23:18 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 02:23:19 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 02:23:19 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 02:31:44 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 02:31:45 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 02:31:45 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 02:31:45 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 02:31:45 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 02:31:45 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 02:31:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 02:31:46 GMT
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
	-	`sha256:53a2fca3c2ea7aa6237addb6763b98a5dfdc15c3a0f33222f9b206d5acac0b91`  
		Last Modified: Sat, 18 Jan 2020 03:11:30 GMT  
		Size: 28.7 MB (28689845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fce49de8b1e8a52f778591ddbf56241326e2d3f3aea9afa3f2d28939ed1fbd`  
		Last Modified: Sat, 18 Jan 2020 03:11:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca406aaf66e09244c9cabb69523721a85751dac98c452dea02390395c5a212df`  
		Last Modified: Thu, 06 Feb 2020 01:44:29 GMT  
		Size: 1.9 MB (1892190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050bda448ba7c14f4ae8fa6f05e2e5001de0b7664375bc0f3277b185b8dd3afe`  
		Last Modified: Thu, 06 Feb 2020 02:36:18 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b823874a3e0e70868ec3182d708c4a41d63310e987680e66f8cd12c3ce34d2`  
		Last Modified: Thu, 06 Feb 2020 02:36:18 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abbf8d18f9e5482e835ffce6a58ade3390522430db489738a84eedf716fee32`  
		Last Modified: Thu, 06 Feb 2020 02:37:13 GMT  
		Size: 133.9 MB (133911926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ccc5c7b3b031094f84969221fbde349bdd3c0e05dc998cb3a99c680c4aa13f`  
		Last Modified: Thu, 06 Feb 2020 02:36:18 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:c4ad99dd2a9e61dbf46a8f22007a3d798560415180ceca57e479826947a8b386
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.9 MB (164907993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4206e1b5bb03314c228aaee3c2dc74548d9512dcf5110a500e9ab1148092b7c6`
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
# Sat, 18 Jan 2020 04:50:12 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 05:06:53 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 05:07:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:53:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:39:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:39:19 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:39:33 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:39:34 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 02:09:44 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 02:09:44 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 02:09:46 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 02:09:47 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 02:30:07 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 02:30:12 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 02:30:13 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 02:30:14 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 02:30:16 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 02:30:17 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 02:30:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 02:30:21 GMT
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
	-	`sha256:aebbc07e72ffbabc6d0ea65ef24ded7dedd55b70faed4aa7235f61e0c6dc0478`  
		Last Modified: Sat, 18 Jan 2020 05:44:23 GMT  
		Size: 26.7 MB (26726326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ccfccce4f40de4c690f1c4c953215c68bf6d9edbeaa444c40d9a220fe7c694`  
		Last Modified: Sat, 18 Jan 2020 05:44:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081556640fdf47a0865f131ba1ff89e9774a48d2552816afd56ded95c240be36`  
		Last Modified: Thu, 06 Feb 2020 01:44:33 GMT  
		Size: 1.9 MB (1892487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132f9f541686c1d5f5db650675cbd1a42e4757e43dd6e7b3a3a07dff4b9fc9cd`  
		Last Modified: Thu, 06 Feb 2020 02:30:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6162e73e5521785fca9fe0c2e87bed2bb19cee2fa6e157f8c57873a36fb32e`  
		Last Modified: Thu, 06 Feb 2020 02:30:38 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2451f229c978d1820e81f1e1ae2c6987ec284088e537a1b965465f0d178cb4`  
		Last Modified: Thu, 06 Feb 2020 02:32:24 GMT  
		Size: 133.4 MB (133364728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfbf2b49771c341da99951ab3af1e1083ced861e14baa6c8660bb6d039654d5`  
		Last Modified: Thu, 06 Feb 2020 02:30:38 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:b8de73d598630e403e648ab2ee0766db6dbe103cae87f49d522a2a6953b95cb4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.8 MB (166775914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6eb3797f2fd9195d4689504752402b054150c3994d6d2767100d056867e818`
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
# Sat, 18 Jan 2020 03:31:27 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 03:45:43 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 03:45:55 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 02:15:46 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:54:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:54:37 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:54:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:54:53 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 03:36:21 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 03:36:22 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 03:36:23 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 03:36:24 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 03:54:30 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 03:54:34 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 03:54:35 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 03:54:36 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 03:54:36 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 03:54:37 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 03:54:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 03:54:38 GMT
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
	-	`sha256:b4d853162255da370dbadaff288bb9f1d3903c095741010d25e14aa51fb0df2e`  
		Last Modified: Sat, 18 Jan 2020 04:19:04 GMT  
		Size: 28.2 MB (28192647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a396952f54f422d45ba879b0f6a69920e7fa88f932f020242c7e3d59058c48d6`  
		Last Modified: Sat, 18 Jan 2020 04:18:54 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4e8ba8a523242d7ae1f4aff8e7099f660f86b5782fef744336a667f1a4087d`  
		Last Modified: Thu, 06 Feb 2020 02:11:19 GMT  
		Size: 1.9 MB (1892503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdacff862803686cab92a2a12e6d56e3e061aa2022ee12d2d62b4498ea173db`  
		Last Modified: Thu, 06 Feb 2020 04:09:46 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4e1afc585605f90af813e5a830a154c8bd15f5eb8b3a1e164585f707649e64`  
		Last Modified: Thu, 06 Feb 2020 04:09:45 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f47c6820783296d753715ea94dab8728a6ceb909e8e9e6cc5fd8be509138e3`  
		Last Modified: Thu, 06 Feb 2020 04:10:56 GMT  
		Size: 133.7 MB (133660666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3ccf36f0a15835cb8ce12b772e2f99aca7e5f6099b239483b93b9e2e788810`  
		Last Modified: Thu, 06 Feb 2020 04:09:46 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; 386

```console
$ docker pull plone@sha256:bf31fdbf1f4d199115a23c5c3be3889ce8c81b40cb317a9a5ac0164d5b40fc0d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165565521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56a77edbdae9b52c7f7e2c51ed41a2813afde9ca90c2c1e6ae89a9ca6aa6ef8`
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
# Sat, 18 Jan 2020 02:07:04 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:19:45 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:19:46 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:58:55 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 00:49:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 00:49:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 00:49:13 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 00:49:13 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 01:37:55 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 01:37:55 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 01:37:56 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 01:37:56 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 01:48:53 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 01:48:55 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 01:48:55 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 01:48:56 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 01:48:56 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 01:48:57 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 01:48:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 01:48:57 GMT
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
	-	`sha256:ae5ce9d316aa4df2055853b0491ee281a07f3f59665bb923a35e4538259fafe4`  
		Last Modified: Sat, 18 Jan 2020 05:38:02 GMT  
		Size: 27.2 MB (27204546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042a4df44aa41c2b54d88fe0f00920dae6f7eafd7e087027bab618b4912ecfc`  
		Last Modified: Sat, 18 Jan 2020 05:37:54 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a08247c30e77b055b7b8ddf2cfb3a02c68333956507dd96f12abfa49f1f7c0f`  
		Last Modified: Thu, 06 Feb 2020 00:56:36 GMT  
		Size: 1.9 MB (1892251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a323f5d6868cf70fbc1491873064f97448096f5c259b6d3a938787bb6b9996d`  
		Last Modified: Thu, 06 Feb 2020 01:57:03 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552813d6ae47a688a0cad95b973bbfcd0115af8ac7f9df47653876f9bba4bfa5`  
		Last Modified: Thu, 06 Feb 2020 01:57:03 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1f9aba7b6eae397db855925cf7f8eab7f4b09230a79f62991ef2c1a80aa031`  
		Last Modified: Thu, 06 Feb 2020 01:57:50 GMT  
		Size: 133.4 MB (133355054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a788b90738187646f8348d43ab52f688259e467e9a10f01129704615c2ead4d`  
		Last Modified: Thu, 06 Feb 2020 01:57:03 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:d8fd8495c45b8b9f78bfc6f44ef9e4fb79fc7e0eff56f1c0a59fabf421d1b752
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169056884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba8a6f58b3af1bb5e6c697e52e4a21f0cbd456843d96f84d67e89d4f54ff62fa`
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
# Sat, 18 Jan 2020 05:06:33 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 05:18:22 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 05:18:29 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 02:38:30 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:31:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:31:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:31:47 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:31:51 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 02:51:44 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 02:51:46 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 02:51:56 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 02:51:57 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 03:07:40 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 03:07:48 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 03:07:50 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 03:07:53 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 03:07:56 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 03:07:58 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 03:08:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 03:08:04 GMT
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
	-	`sha256:9f5d173893fbe54a062519b8ef5d68403a697a00c4c8741ea641e742dd41862a`  
		Last Modified: Sat, 18 Jan 2020 05:46:19 GMT  
		Size: 29.6 MB (29612538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030ea3db62c6d8771ba19ecee7109a97439e647e0e25356096f6f7aad6dd2e04`  
		Last Modified: Sat, 18 Jan 2020 05:46:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bde1575b2c7098a717fde701a00a7d2ff87b57de35c5a05cfe0ef1b8eddf51`  
		Last Modified: Thu, 06 Feb 2020 01:52:32 GMT  
		Size: 1.9 MB (1892522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089c1e6255322429c9764c5aaf56595ea92e8aea94595d2ae8db33e47f4ac98a`  
		Last Modified: Thu, 06 Feb 2020 03:28:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06be0137416a9df9b42aae289f6e95730348856ee1c5e64ecf73c2c231aec25`  
		Last Modified: Thu, 06 Feb 2020 03:28:10 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cb69c6d827fc2558f8943eab2da793b84beeb7ad2531268964477ecde9342f`  
		Last Modified: Thu, 06 Feb 2020 03:29:37 GMT  
		Size: 134.4 MB (134420448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416a144bb270c6ea27ef44de61e6faf957d91b37bdef99fc728e35f1170b2197`  
		Last Modified: Thu, 06 Feb 2020 03:28:10 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; s390x

```console
$ docker pull plone@sha256:9ccd0aff5954e7b8041056369e02d6fa2df67b558a4f1a49d73503367c355a18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167856958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9016c845f528be148a21d9ad7960888a0eb978970eb2e8bba2a82f1677d2ede1`
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
# Sat, 25 Jan 2020 01:52:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/42ad3426cb1ef05863521d7988d5f7fec0c99560/get-pip.py
# Sat, 25 Jan 2020 01:52:23 GMT
ENV PYTHON_GET_PIP_SHA256=da288fc002d0bb2b90f6fbabc91048c1fa18d567ad067ee713c6e331d3a32b45
# Sat, 25 Jan 2020 01:52:27 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 25 Jan 2020 01:52:27 GMT
CMD ["python3"]
# Thu, 30 Jan 2020 23:09:56 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 30 Jan 2020 23:09:56 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 30 Jan 2020 23:09:57 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 30 Jan 2020 23:09:57 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 30 Jan 2020 23:16:19 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 30 Jan 2020 23:16:28 GMT
VOLUME [/data]
# Thu, 30 Jan 2020 23:16:28 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 30 Jan 2020 23:16:28 GMT
EXPOSE 8080
# Thu, 30 Jan 2020 23:16:29 GMT
WORKDIR /plone/instance
# Thu, 30 Jan 2020 23:16:29 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 30 Jan 2020 23:16:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:16:29 GMT
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
	-	`sha256:1997174415ba324b2612ca12762fb1dec19c25b34ee9cc34897cb678bafcbe19`  
		Last Modified: Sat, 25 Jan 2020 01:57:54 GMT  
		Size: 1.9 MB (1887363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e137422f32895097ef542b97feed35cdfd5666da0d2b7287f5eaa60d12a9ab`  
		Last Modified: Thu, 30 Jan 2020 23:31:05 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73988218a40a1217b0569567ddb67c61444a1485c5bb26c6dcdb118cdbfca76`  
		Last Modified: Thu, 30 Jan 2020 23:31:11 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973926f54c6dd626dbc9f6923d102074d3ed09a79a4bfafd0b7f80c96321e9a`  
		Last Modified: Thu, 30 Jan 2020 23:31:24 GMT  
		Size: 134.1 MB (134140072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1086dbcd802262647497b67e66504660a7e23e7ad0050e3a794f9009cf71cdd3`  
		Last Modified: Thu, 30 Jan 2020 23:31:05 GMT  
		Size: 2.6 KB (2625 bytes)  
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
$ docker pull plone@sha256:9d26bf42175e073f2d43a8e306f3d56f09feb51d195f9c34bf783b255463ba69
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
$ docker pull plone@sha256:b73b0018004aa08ba04c658453b57363f046354ea73ccbac27b6d3c10daa031b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.6 MB (167603380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:495fedeb528f4a81a23475277826be9efd9e4a03f22e80b70feeb6d6b7efa4ea`
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
# Sat, 18 Jan 2020 02:43:48 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:51:40 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:51:41 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 02:51:16 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:38:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:38:21 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:38:28 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:38:28 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 02:23:18 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 02:23:18 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 02:23:19 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 02:23:19 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 02:31:44 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 02:31:45 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 02:31:45 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 02:31:45 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 02:31:45 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 02:31:45 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 02:31:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 02:31:46 GMT
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
	-	`sha256:53a2fca3c2ea7aa6237addb6763b98a5dfdc15c3a0f33222f9b206d5acac0b91`  
		Last Modified: Sat, 18 Jan 2020 03:11:30 GMT  
		Size: 28.7 MB (28689845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fce49de8b1e8a52f778591ddbf56241326e2d3f3aea9afa3f2d28939ed1fbd`  
		Last Modified: Sat, 18 Jan 2020 03:11:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca406aaf66e09244c9cabb69523721a85751dac98c452dea02390395c5a212df`  
		Last Modified: Thu, 06 Feb 2020 01:44:29 GMT  
		Size: 1.9 MB (1892190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050bda448ba7c14f4ae8fa6f05e2e5001de0b7664375bc0f3277b185b8dd3afe`  
		Last Modified: Thu, 06 Feb 2020 02:36:18 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b823874a3e0e70868ec3182d708c4a41d63310e987680e66f8cd12c3ce34d2`  
		Last Modified: Thu, 06 Feb 2020 02:36:18 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abbf8d18f9e5482e835ffce6a58ade3390522430db489738a84eedf716fee32`  
		Last Modified: Thu, 06 Feb 2020 02:37:13 GMT  
		Size: 133.9 MB (133911926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ccc5c7b3b031094f84969221fbde349bdd3c0e05dc998cb3a99c680c4aa13f`  
		Last Modified: Thu, 06 Feb 2020 02:36:18 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:c4ad99dd2a9e61dbf46a8f22007a3d798560415180ceca57e479826947a8b386
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.9 MB (164907993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4206e1b5bb03314c228aaee3c2dc74548d9512dcf5110a500e9ab1148092b7c6`
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
# Sat, 18 Jan 2020 04:50:12 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 05:06:53 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 05:07:04 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:53:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:39:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:39:19 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:39:33 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:39:34 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 02:09:44 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 02:09:44 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 02:09:46 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 02:09:47 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 02:30:07 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 02:30:12 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 02:30:13 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 02:30:14 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 02:30:16 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 02:30:17 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 02:30:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 02:30:21 GMT
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
	-	`sha256:aebbc07e72ffbabc6d0ea65ef24ded7dedd55b70faed4aa7235f61e0c6dc0478`  
		Last Modified: Sat, 18 Jan 2020 05:44:23 GMT  
		Size: 26.7 MB (26726326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ccfccce4f40de4c690f1c4c953215c68bf6d9edbeaa444c40d9a220fe7c694`  
		Last Modified: Sat, 18 Jan 2020 05:44:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081556640fdf47a0865f131ba1ff89e9774a48d2552816afd56ded95c240be36`  
		Last Modified: Thu, 06 Feb 2020 01:44:33 GMT  
		Size: 1.9 MB (1892487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132f9f541686c1d5f5db650675cbd1a42e4757e43dd6e7b3a3a07dff4b9fc9cd`  
		Last Modified: Thu, 06 Feb 2020 02:30:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6162e73e5521785fca9fe0c2e87bed2bb19cee2fa6e157f8c57873a36fb32e`  
		Last Modified: Thu, 06 Feb 2020 02:30:38 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2451f229c978d1820e81f1e1ae2c6987ec284088e537a1b965465f0d178cb4`  
		Last Modified: Thu, 06 Feb 2020 02:32:24 GMT  
		Size: 133.4 MB (133364728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfbf2b49771c341da99951ab3af1e1083ced861e14baa6c8660bb6d039654d5`  
		Last Modified: Thu, 06 Feb 2020 02:30:38 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:b8de73d598630e403e648ab2ee0766db6dbe103cae87f49d522a2a6953b95cb4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.8 MB (166775914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6eb3797f2fd9195d4689504752402b054150c3994d6d2767100d056867e818`
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
# Sat, 18 Jan 2020 03:31:27 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 03:45:43 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 03:45:55 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 02:15:46 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:54:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:54:37 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:54:52 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:54:53 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 03:36:21 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 03:36:22 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 03:36:23 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 03:36:24 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 03:54:30 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 03:54:34 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 03:54:35 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 03:54:36 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 03:54:36 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 03:54:37 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 03:54:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 03:54:38 GMT
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
	-	`sha256:b4d853162255da370dbadaff288bb9f1d3903c095741010d25e14aa51fb0df2e`  
		Last Modified: Sat, 18 Jan 2020 04:19:04 GMT  
		Size: 28.2 MB (28192647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a396952f54f422d45ba879b0f6a69920e7fa88f932f020242c7e3d59058c48d6`  
		Last Modified: Sat, 18 Jan 2020 04:18:54 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4e8ba8a523242d7ae1f4aff8e7099f660f86b5782fef744336a667f1a4087d`  
		Last Modified: Thu, 06 Feb 2020 02:11:19 GMT  
		Size: 1.9 MB (1892503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdacff862803686cab92a2a12e6d56e3e061aa2022ee12d2d62b4498ea173db`  
		Last Modified: Thu, 06 Feb 2020 04:09:46 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4e1afc585605f90af813e5a830a154c8bd15f5eb8b3a1e164585f707649e64`  
		Last Modified: Thu, 06 Feb 2020 04:09:45 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f47c6820783296d753715ea94dab8728a6ceb909e8e9e6cc5fd8be509138e3`  
		Last Modified: Thu, 06 Feb 2020 04:10:56 GMT  
		Size: 133.7 MB (133660666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3ccf36f0a15835cb8ce12b772e2f99aca7e5f6099b239483b93b9e2e788810`  
		Last Modified: Thu, 06 Feb 2020 04:09:46 GMT  
		Size: 2.6 KB (2626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; 386

```console
$ docker pull plone@sha256:bf31fdbf1f4d199115a23c5c3be3889ce8c81b40cb317a9a5ac0164d5b40fc0d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165565521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56a77edbdae9b52c7f7e2c51ed41a2813afde9ca90c2c1e6ae89a9ca6aa6ef8`
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
# Sat, 18 Jan 2020 02:07:04 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 02:19:45 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 02:19:46 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 01:58:55 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 00:49:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 00:49:06 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 00:49:13 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 00:49:13 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 01:37:55 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 01:37:55 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 01:37:56 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 01:37:56 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 01:48:53 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 01:48:55 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 01:48:55 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 01:48:56 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 01:48:56 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 01:48:57 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 01:48:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 01:48:57 GMT
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
	-	`sha256:ae5ce9d316aa4df2055853b0491ee281a07f3f59665bb923a35e4538259fafe4`  
		Last Modified: Sat, 18 Jan 2020 05:38:02 GMT  
		Size: 27.2 MB (27204546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5042a4df44aa41c2b54d88fe0f00920dae6f7eafd7e087027bab618b4912ecfc`  
		Last Modified: Sat, 18 Jan 2020 05:37:54 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a08247c30e77b055b7b8ddf2cfb3a02c68333956507dd96f12abfa49f1f7c0f`  
		Last Modified: Thu, 06 Feb 2020 00:56:36 GMT  
		Size: 1.9 MB (1892251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a323f5d6868cf70fbc1491873064f97448096f5c259b6d3a938787bb6b9996d`  
		Last Modified: Thu, 06 Feb 2020 01:57:03 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552813d6ae47a688a0cad95b973bbfcd0115af8ac7f9df47653876f9bba4bfa5`  
		Last Modified: Thu, 06 Feb 2020 01:57:03 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1f9aba7b6eae397db855925cf7f8eab7f4b09230a79f62991ef2c1a80aa031`  
		Last Modified: Thu, 06 Feb 2020 01:57:50 GMT  
		Size: 133.4 MB (133355054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a788b90738187646f8348d43ab52f688259e467e9a10f01129704615c2ead4d`  
		Last Modified: Thu, 06 Feb 2020 01:57:03 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:d8fd8495c45b8b9f78bfc6f44ef9e4fb79fc7e0eff56f1c0a59fabf421d1b752
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169056884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba8a6f58b3af1bb5e6c697e52e4a21f0cbd456843d96f84d67e89d4f54ff62fa`
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
# Sat, 18 Jan 2020 05:06:33 GMT
ENV PYTHON_VERSION=3.7.6
# Sat, 18 Jan 2020 05:18:22 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Sat, 18 Jan 2020 05:18:29 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 25 Jan 2020 02:38:30 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Thu, 06 Feb 2020 01:31:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Thu, 06 Feb 2020 01:31:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Thu, 06 Feb 2020 01:31:47 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 06 Feb 2020 01:31:51 GMT
CMD ["python3"]
# Thu, 06 Feb 2020 02:51:44 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 06 Feb 2020 02:51:46 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 06 Feb 2020 02:51:56 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 06 Feb 2020 02:51:57 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 06 Feb 2020 03:07:40 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 06 Feb 2020 03:07:48 GMT
VOLUME [/data]
# Thu, 06 Feb 2020 03:07:50 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 06 Feb 2020 03:07:53 GMT
EXPOSE 8080
# Thu, 06 Feb 2020 03:07:56 GMT
WORKDIR /plone/instance
# Thu, 06 Feb 2020 03:07:58 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 06 Feb 2020 03:08:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Feb 2020 03:08:04 GMT
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
	-	`sha256:9f5d173893fbe54a062519b8ef5d68403a697a00c4c8741ea641e742dd41862a`  
		Last Modified: Sat, 18 Jan 2020 05:46:19 GMT  
		Size: 29.6 MB (29612538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030ea3db62c6d8771ba19ecee7109a97439e647e0e25356096f6f7aad6dd2e04`  
		Last Modified: Sat, 18 Jan 2020 05:46:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bde1575b2c7098a717fde701a00a7d2ff87b57de35c5a05cfe0ef1b8eddf51`  
		Last Modified: Thu, 06 Feb 2020 01:52:32 GMT  
		Size: 1.9 MB (1892522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089c1e6255322429c9764c5aaf56595ea92e8aea94595d2ae8db33e47f4ac98a`  
		Last Modified: Thu, 06 Feb 2020 03:28:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06be0137416a9df9b42aae289f6e95730348856ee1c5e64ecf73c2c231aec25`  
		Last Modified: Thu, 06 Feb 2020 03:28:10 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cb69c6d827fc2558f8943eab2da793b84beeb7ad2531268964477ecde9342f`  
		Last Modified: Thu, 06 Feb 2020 03:29:37 GMT  
		Size: 134.4 MB (134420448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416a144bb270c6ea27ef44de61e6faf957d91b37bdef99fc728e35f1170b2197`  
		Last Modified: Thu, 06 Feb 2020 03:28:10 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; s390x

```console
$ docker pull plone@sha256:9ccd0aff5954e7b8041056369e02d6fa2df67b558a4f1a49d73503367c355a18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167856958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9016c845f528be148a21d9ad7960888a0eb978970eb2e8bba2a82f1677d2ede1`
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
# Sat, 25 Jan 2020 01:52:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/42ad3426cb1ef05863521d7988d5f7fec0c99560/get-pip.py
# Sat, 25 Jan 2020 01:52:23 GMT
ENV PYTHON_GET_PIP_SHA256=da288fc002d0bb2b90f6fbabc91048c1fa18d567ad067ee713c6e331d3a32b45
# Sat, 25 Jan 2020 01:52:27 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 25 Jan 2020 01:52:27 GMT
CMD ["python3"]
# Thu, 30 Jan 2020 23:09:56 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 30 Jan 2020 23:09:56 GMT
LABEL plone=5.2.1 os=alpine os.version=3.11 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 30 Jan 2020 23:09:57 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 30 Jan 2020 23:09:57 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 30 Jan 2020 23:16:19 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 30 Jan 2020 23:16:28 GMT
VOLUME [/data]
# Thu, 30 Jan 2020 23:16:28 GMT
COPY multi:c1f88121bdba3f4019314daa8a4906c592b99b3ebbde00413dc4680482b6d329 in / 
# Thu, 30 Jan 2020 23:16:28 GMT
EXPOSE 8080
# Thu, 30 Jan 2020 23:16:29 GMT
WORKDIR /plone/instance
# Thu, 30 Jan 2020 23:16:29 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 30 Jan 2020 23:16:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:16:29 GMT
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
	-	`sha256:1997174415ba324b2612ca12762fb1dec19c25b34ee9cc34897cb678bafcbe19`  
		Last Modified: Sat, 25 Jan 2020 01:57:54 GMT  
		Size: 1.9 MB (1887363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e137422f32895097ef542b97feed35cdfd5666da0d2b7287f5eaa60d12a9ab`  
		Last Modified: Thu, 30 Jan 2020 23:31:05 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73988218a40a1217b0569567ddb67c61444a1485c5bb26c6dcdb118cdbfca76`  
		Last Modified: Thu, 30 Jan 2020 23:31:11 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973926f54c6dd626dbc9f6923d102074d3ed09a79a4bfafd0b7f80c96321e9a`  
		Last Modified: Thu, 30 Jan 2020 23:31:24 GMT  
		Size: 134.1 MB (134140072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1086dbcd802262647497b67e66504660a7e23e7ad0050e3a794f9009cf71cdd3`  
		Last Modified: Thu, 30 Jan 2020 23:31:05 GMT  
		Size: 2.6 KB (2625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `plone:latest`

```console
$ docker pull plone@sha256:3598db582fd18e0e79067a869f63c8bc063cee5fd9c01c40ee01f625944a3a0c
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
$ docker pull plone@sha256:ceb59901e866ec67d66005ef2f747b98cf6c13962b89bd96a24d8acb2dbb4a56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211290985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0dc524b96661924ba6b46ef04c6fe07f5e7da04ee95116822a7ec8d128f114b`
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
# Wed, 26 Feb 2020 15:55:25 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 16:05:21 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 16:05:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 16:05:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 16:05:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 16:05:24 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 16:05:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 16:05:44 GMT
CMD ["python3"]
# Thu, 27 Feb 2020 05:48:05 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 05:48:05 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 05:48:06 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 05:48:06 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 05:51:37 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 05:51:38 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 05:51:38 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 05:51:39 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 05:51:39 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 05:51:39 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 05:51:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 05:51:39 GMT
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
	-	`sha256:6a33999da14c835e8d3ddcef893fa350153761194bdad1c4a5ee5aa0be90f99c`  
		Last Modified: Wed, 26 Feb 2020 17:48:44 GMT  
		Size: 25.8 MB (25798778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66020c9836480d0db8f94f2acc77f32bf2dd3063a10f4d1d20de5b149009ef4`  
		Last Modified: Wed, 26 Feb 2020 17:48:38 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4703522495058fef344d4879a78cca1e9e153944cee3f036a8ab1ecae6dd839`  
		Last Modified: Wed, 26 Feb 2020 17:48:38 GMT  
		Size: 2.2 MB (2176130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e763c27664adfe48dfa0c2e91cfbb1f2526dd6282a1f2c05d9f93805b66e6b`  
		Last Modified: Thu, 27 Feb 2020 05:55:31 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d47d7fdaea68eeb5b75b87786b64e2b50ef6147dd07c686e7b21488a14f260`  
		Last Modified: Thu, 27 Feb 2020 05:55:31 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68114f24f65e8d32aecc6b595c0ab1d22dec7865ea29a09a06793330c2b6787f`  
		Last Modified: Thu, 27 Feb 2020 05:55:58 GMT  
		Size: 158.3 MB (158263721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bd512f7102a2793a61a194251288014c655138b3f7bc8f9b7f6ce98a037e0d`  
		Last Modified: Thu, 27 Feb 2020 05:55:30 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; arm variant v5

```console
$ docker pull plone@sha256:f1ee2e2cf24e672ab9d950a816efd14c229edcadd2f1f4e7ff1d494969eb47ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.2 MB (204187751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701fabf98700b541e80f72ac32cfd6579de85841d6f46ee50b198971aad428b3`
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
# Wed, 26 Feb 2020 07:43:10 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 07:53:26 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 07:53:29 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 07:53:30 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 07:53:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 07:53:31 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 07:54:04 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 07:54:05 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 16:34:34 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 16:34:35 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 16:34:38 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 16:34:39 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 16:49:53 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 16:50:02 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 16:50:03 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 16:50:04 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 16:50:04 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 16:50:05 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 16:50:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 16:50:06 GMT
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
	-	`sha256:d656f5a68dce32db0da25657fa8145509090dd717db0863e3db4a1311d35cad7`  
		Last Modified: Wed, 26 Feb 2020 09:52:39 GMT  
		Size: 22.8 MB (22770271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe441b54bc0ba71262311bc0d52e1668eeac33128e8f36c6af8fa3e6f331b17`  
		Last Modified: Wed, 26 Feb 2020 09:52:31 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595aaeb76d185f5074015b02211536772493bf063be415920a206b07df589942`  
		Last Modified: Wed, 26 Feb 2020 09:52:32 GMT  
		Size: 2.2 MB (2175913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c00d302ea0af84737c436e4cb35da3708abe19235483300dcd58d85b2e9b1b`  
		Last Modified: Wed, 26 Feb 2020 17:05:07 GMT  
		Size: 3.9 KB (3925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abee76f1efce0ea1da36f0f2989c826993ed3ea2e50b6d09bc9b1835b05e1b0`  
		Last Modified: Wed, 26 Feb 2020 17:05:07 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862e034aab772fc7287991f2c52184c8a9ff9aa92f6c16b043211519c0194e49`  
		Last Modified: Wed, 26 Feb 2020 17:06:08 GMT  
		Size: 155.8 MB (155786269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de48e91c45e20dca818e2dcaf7e5caba591beeab6628b545b31b8e0b068d9ada`  
		Last Modified: Wed, 26 Feb 2020 17:05:07 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; arm variant v7

```console
$ docker pull plone@sha256:214303debdcd61422d269ee7b40b0b4da11af7c3295724f5561d92081892d525
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.5 MB (201472309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16474bc9c1a41eb8c1eebd8f52c7f821e1c21ae48d47289152b4c30c6837e247`
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
# Wed, 26 Feb 2020 10:10:24 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 10:23:19 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 10:23:22 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 10:23:23 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 10:23:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 10:23:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 10:23:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 10:23:52 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 23:21:11 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 23:21:12 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 23:21:16 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 23:21:17 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 23:34:21 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 23:34:28 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 23:34:29 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 23:34:29 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 23:34:30 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 23:34:31 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 23:34:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 23:34:32 GMT
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
	-	`sha256:6b2b245c7a0af359854db6ff69d5961cf78220a90f0c35e133f8b1c193b64b2c`  
		Last Modified: Wed, 26 Feb 2020 12:27:59 GMT  
		Size: 23.3 MB (23341944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa24266bc1f7d33a53425b488668c6f12d9119b321df759e07b7511c5a0cf057`  
		Last Modified: Wed, 26 Feb 2020 12:27:49 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb838bd6d171e306f9a7bae4693aa12f8b3661bb1513744488d25cbefbecc34`  
		Last Modified: Wed, 26 Feb 2020 12:27:50 GMT  
		Size: 2.2 MB (2175955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b22b8976660ae5dd1d3a6e3b9fd151b01613f6851f628848d2319d2cd3d687e`  
		Last Modified: Wed, 26 Feb 2020 23:47:42 GMT  
		Size: 3.9 KB (3927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ece09e7454f28201a9b11ea15b4c65bff449a93cdc594127208114975c26b7`  
		Last Modified: Wed, 26 Feb 2020 23:47:42 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82da71967ea508b1c336249654a489de13b1c340e27a3277f2b2c3b76bc5afd6`  
		Last Modified: Wed, 26 Feb 2020 23:48:38 GMT  
		Size: 154.5 MB (154470319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0fd9bb5d13ee64e18385cbb3953e7e18cddc8db731d536a0f1e73041ccac18`  
		Last Modified: Wed, 26 Feb 2020 23:47:41 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:1f7389070d10279c0672d02cea678b9e2a62f5a07c430516f108f0bc63ccdcaa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.8 MB (204756651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9bc590e017ec955cbddb1164ce1f21a67e5c9b4d2de4da4d287e46b8df8503`
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
# Wed, 26 Feb 2020 16:31:07 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 16:43:32 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 16:43:34 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 16:43:35 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 16:43:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 16:43:36 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 16:44:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 16:44:01 GMT
CMD ["python3"]
# Thu, 27 Feb 2020 04:12:36 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Thu, 27 Feb 2020 04:12:37 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 27 Feb 2020 04:12:39 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Thu, 27 Feb 2020 04:12:40 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Thu, 27 Feb 2020 04:26:07 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Thu, 27 Feb 2020 04:26:13 GMT
VOLUME [/data]
# Thu, 27 Feb 2020 04:26:14 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Thu, 27 Feb 2020 04:26:15 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 04:26:16 GMT
WORKDIR /plone/instance
# Thu, 27 Feb 2020 04:26:16 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 27 Feb 2020 04:26:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 04:26:18 GMT
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
	-	`sha256:7a935d604f767a1b217bfe7f9d447c14b71eb5374ffa8278a1a2b2c3ade4b8d4`  
		Last Modified: Wed, 26 Feb 2020 18:37:47 GMT  
		Size: 24.6 MB (24642485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2c221be0fd5417f9d1b382f04d0be0c23decf3862a18be2557a5ada8b38a81`  
		Last Modified: Wed, 26 Feb 2020 18:37:38 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f859a56ff0ad189b82614fc47d2db5777e932e063ad0a077d771c825fbc0a18`  
		Last Modified: Wed, 26 Feb 2020 18:37:39 GMT  
		Size: 2.2 MB (2175818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaeb4713261f88d7096432170cbb67ead5bfd0fdcb56f3e734b3c15854d978`  
		Last Modified: Thu, 27 Feb 2020 04:40:29 GMT  
		Size: 3.9 KB (3938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6501e3434223e00219cc740175867bfe7ffa66bff8732bcfe605e4b583b3b1ed`  
		Last Modified: Thu, 27 Feb 2020 04:40:29 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12efba0f87b7801cf9ecc73d27a8912b48fe5cd541de54acc680f2ebe50870a`  
		Last Modified: Thu, 27 Feb 2020 04:41:15 GMT  
		Size: 155.3 MB (155321506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a7147a31133fdd8d62354a465c24571ddd88266d90240fea63ae932a5f1e82`  
		Last Modified: Thu, 27 Feb 2020 04:40:29 GMT  
		Size: 2.6 KB (2621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; 386

```console
$ docker pull plone@sha256:7156ed5eed6a8d9d2e803ea06f9190a7865460c779ecbd513f4b9e0b94ce0d21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.5 MB (210547897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21f43ffd375048752eaaf0c8a0b5e5a9908d68a58b3bc64e76068bb0943c87e7`
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
# Wed, 26 Feb 2020 13:32:29 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 13:46:05 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 13:46:06 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 13:46:06 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 13:46:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 13:46:07 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 13:46:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 13:46:24 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 20:16:25 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 20:16:25 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 20:16:26 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 20:16:26 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 20:20:57 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 20:20:58 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 20:20:58 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 20:20:58 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 20:20:58 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 20:20:59 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 20:20:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 20:20:59 GMT
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
	-	`sha256:348e763dadfd1b50ff2edb8db5bfc850d30d36ecc064bb59619b6c6d6907e0ee`  
		Last Modified: Wed, 26 Feb 2020 15:50:16 GMT  
		Size: 24.2 MB (24220228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddab4eecfc9a7a10fccdd0e8bab77fd7b8ee7fb0071010573940c23c7628670`  
		Last Modified: Wed, 26 Feb 2020 15:50:09 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e48df556a7b9278e2d994e723c841a90b489f0402a453ba8431053380219fbc`  
		Last Modified: Wed, 26 Feb 2020 15:50:10 GMT  
		Size: 2.2 MB (2175788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e4005781a4394f5c90bc432850f94859e490bb5f21717f2e6b932ff6a191d2`  
		Last Modified: Wed, 26 Feb 2020 20:26:21 GMT  
		Size: 3.9 KB (3873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0ec73ea37c1efe7f599ed0256171c4652822b56fe58b4481980beae0bd309a`  
		Last Modified: Wed, 26 Feb 2020 20:26:21 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc6846fa93309fbbafd84b2465c4259e8b48e8e3f0f7ae193a7170be3fd43de`  
		Last Modified: Wed, 26 Feb 2020 20:27:18 GMT  
		Size: 158.5 MB (158469826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d833dfe4555374e8ab4eceabe08d85851e659e6a0eba6711ee0a0f924dc8dcd0`  
		Last Modified: Wed, 26 Feb 2020 20:26:21 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:latest` - linux; ppc64le

```console
$ docker pull plone@sha256:17c4307890f9a856016b666c7061b3e0b5a1eea5fb8a8cde982151717aefb96d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.8 MB (209783941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d2fe8cfe5a13c4b275bc426038eec3858c7357395e5ee4effe9119a5540e8ea`
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
# Wed, 26 Feb 2020 04:02:38 GMT
ENV PYTHON_VERSION=3.7.6
# Wed, 26 Feb 2020 04:18:08 GMT
RUN set -ex 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libbluetooth-dev 		libbz2-dev 		libc6-dev 		libexpat1-dev 		libffi-dev 		libgdbm-dev 		liblzma-dev 		libncursesw5-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		make 		tk-dev 		uuid-dev 		wget 		xz-utils 		zlib1g-dev 		$(command -v gpg > /dev/null || echo 'gnupg dirmngr') 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		PROFILE_TASK='-m test.regrtest --pgo 			test_array 			test_base64 			test_binascii 			test_binhex 			test_binop 			test_bytes 			test_c_locale_coercion 			test_class 			test_cmath 			test_codecs 			test_compile 			test_complex 			test_csv 			test_decimal 			test_dict 			test_float 			test_fstring 			test_hashlib 			test_io 			test_iter 			test_json 			test_long 			test_math 			test_memoryview 			test_pickle 			test_re 			test_set 			test_slice 			test_struct 			test_threading 			test_time 			test_traceback 			test_unicode 		' 	&& make install 	&& ldconfig 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark 	&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 	&& rm -rf /var/lib/apt/lists/* 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' + 	&& rm -rf /usr/src/python 		&& python3 --version
# Wed, 26 Feb 2020 04:18:16 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 26 Feb 2020 04:18:18 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 26 Feb 2020 04:18:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 26 Feb 2020 04:18:25 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 26 Feb 2020 04:19:18 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Feb 2020 04:19:21 GMT
CMD ["python3"]
# Wed, 26 Feb 2020 20:47:42 GMT
ENV PIP=19.3.1 ZC_BUILDOUT=2.13.2 SETUPTOOLS=45.0.0 WHEEL=0.33.6 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.1 PLONE_VERSION_RELEASE=Plone-5.2.1-UnifiedInstaller-r2 PLONE_MD5=42407c0313791d3626dc86e674684efe
# Wed, 26 Feb 2020 20:47:45 GMT
LABEL plone=5.2.1 os=debian os.version=9 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Wed, 26 Feb 2020 20:47:56 GMT
RUN useradd --system -m -d /plone -U -u 500 plone  && mkdir -p /plone/instance/ /data/filestorage /data/blobstorage
# Wed, 26 Feb 2020 20:47:57 GMT
COPY file:9266bca2e9775c84ef54f877d6d8090bca5c55d7cc6faf7b7226bc188ab30a69 in /plone/instance/ 
# Wed, 26 Feb 2020 21:06:50 GMT
RUN buildDeps="dpkg-dev gcc libbz2-dev libc6-dev libffi-dev libjpeg62-turbo-dev libopenjp2-7-dev libpcre3-dev libssl-dev libtiff5-dev libxml2-dev libxslt1-dev wget zlib1g-dev"  && runDeps="gosu libjpeg62 libopenjp2-7 libtiff5 libxml2 libxslt1.1 lynx netcat poppler-utils rsync wv"  && apt-get update  && apt-get install -y --no-install-recommends $buildDeps  && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz  && echo "$PLONE_MD5 Plone.tgz" | md5sum -c -  && tar -xzf Plone.tgz  && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/  && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg  && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL  && cd /plone/instance  && buildout  && ln -s /data/filestorage/ /plone/instance/var/filestorage  && ln -s /data/blobstorage /plone/instance/var/blobstorage  && find /data  -not -user plone -exec chown plone:plone {} \+  && find /plone -not -user plone -exec chown plone:plone {} \+  && rm -rf /Plone*  && apt-get purge -y --auto-remove $buildDeps  && apt-get install -y --no-install-recommends $runDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /plone/buildout-cache/downloads/*
# Wed, 26 Feb 2020 21:06:57 GMT
VOLUME [/data]
# Wed, 26 Feb 2020 21:06:59 GMT
COPY multi:6f1f55b0dc0550e6d1ba7e7677d6b1c6dfdeec1fa19b34329bf5b1a9830c0720 in / 
# Wed, 26 Feb 2020 21:07:01 GMT
EXPOSE 8080
# Wed, 26 Feb 2020 21:07:04 GMT
WORKDIR /plone/instance
# Wed, 26 Feb 2020 21:07:07 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 26 Feb 2020 21:07:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Feb 2020 21:07:13 GMT
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
	-	`sha256:af1513bf2ee03f2207d52345cb8aab950ec5068ec549b6cc088883cbca15f589`  
		Last Modified: Wed, 26 Feb 2020 06:05:30 GMT  
		Size: 25.9 MB (25876486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b3c1956c8f7efa590d60fe60b38ae14e16d52e0cf761a027fa508bdcc6e9c3`  
		Last Modified: Wed, 26 Feb 2020 06:05:22 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d06518c1d2db54727f6703bbbb53ca3d6c455f37698b29ac36e7f56aa8072b`  
		Last Modified: Wed, 26 Feb 2020 06:05:29 GMT  
		Size: 2.2 MB (2177157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0979f1e8cf6dcc2466de7ff88c1da8b24f21d1981cf323a1357100177df72`  
		Last Modified: Wed, 26 Feb 2020 21:29:59 GMT  
		Size: 3.9 KB (3938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d7021169b65fe3a0fe29d0b106245899e94afccee671744aa0b78f29a77479`  
		Last Modified: Wed, 26 Feb 2020 21:29:59 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb31f56f89b4d9ddf929bc79a25c705f4ea472b254a66931f16eb372ddb207f`  
		Last Modified: Wed, 26 Feb 2020 21:34:15 GMT  
		Size: 156.7 MB (156744482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d994590772d0ed4543da406d847fbd2362b5c00f00a8e39a6858fe972dc7a70d`  
		Last Modified: Wed, 26 Feb 2020 21:29:59 GMT  
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
