## `hylang:pypy`

```console
$ docker pull hylang@sha256:63af40986a0cb3c9c9268e0d9c6df24cfe6b8bc958691d31251a4b4393a03337
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; s390x

### `hylang:pypy` - linux; amd64

```console
$ docker pull hylang@sha256:7d554d9e87b1a1e757633babed6aff9954813cb18b0dc9e50c86e95123b6d887
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70327751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e611f04aaf701de728bc4344ee83d0cfba1d18142866e5d64e0e78a519a045`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 15:25:13 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 15:25:14 GMT
ENV LANG=C.UTF-8
# Tue, 14 Apr 2020 19:22:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 14 Apr 2020 19:22:39 GMT
ENV PYPY_VERSION=7.3.0
# Tue, 14 Apr 2020 19:24:26 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='d3d549e8f43de820ac3385b698b83fa59b4d7dd6cf3fe34c115f731e26ad8856' ;; 		arm64) pypyArch='aarch64'; sha256='b900241bca7152254c107a632767f49edede99ca6360b9a064141267b47ef598' ;; 		i386) pypyArch='linux32'; sha256='7045b295d38ba0b5ee65bd3f078ca249fcf1de73fedeaab2d6ad78de2eab0f0e' ;; 		ppc64el) pypyArch='ppc64le'; sha256='d6f3b701313df69483b43ebdd21b9652ae5e808b2eea5fbffe3b74b82d2e7433' ;; 		s390x) pypyArch='s390x'; sha256='0fe2f7bbf42ea88b40954d7de773a43179a44f40656f2f58201524be70699544' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	find /usr/local/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		pypy3 --version; 		if [ -f /usr/local/lib_pypy/_ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		cd /usr/local/lib_pypy; 		pypy3 _ssl_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 	find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 14 Apr 2020 19:24:26 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Tue, 14 Apr 2020 19:24:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Tue, 14 Apr 2020 19:24:27 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Tue, 14 Apr 2020 19:24:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 14 Apr 2020 19:24:43 GMT
CMD ["pypy3"]
# Thu, 16 Apr 2020 00:24:49 GMT
ENV HY_VERSION=0.18.0
# Thu, 16 Apr 2020 00:24:59 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Thu, 16 Apr 2020 00:24:59 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04fe01560d2b7c4b36a1a707c3c469a9557e7b82395be77c0a88a37b321b6d2`  
		Last Modified: Tue, 14 Apr 2020 19:25:36 GMT  
		Size: 2.7 MB (2741590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb804993f13d35c0e42d7a159a55cd62669b1487f2f7c378304c789dc2d09de`  
		Last Modified: Tue, 14 Apr 2020 19:26:26 GMT  
		Size: 35.4 MB (35399778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0bad163fa08d6c2789379b52ddb1ae6ceba422ac113e80d05b023e70cabb25`  
		Last Modified: Tue, 14 Apr 2020 19:26:18 GMT  
		Size: 2.2 MB (2166509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4796a686d8019568e2619c52e84cb86760aabfea4a8d6790f9eebe9164bcc2`  
		Last Modified: Thu, 16 Apr 2020 00:25:38 GMT  
		Size: 2.9 MB (2928012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy` - linux; 386

```console
$ docker pull hylang@sha256:eb0653397bf5f830e1c5502e93bfeb4548fd9a0b1eac9e3ad35a4b0029506f4c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65518242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9ab6add0033a9fcd1dc3f7a83d6aa7d9e97419e08599a41372ff6a434dd516`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 Sep 2019 22:43:38 GMT
ADD file:8bc08dfa2497c2f2aa5368a174cab8c82ad30aa91d233a203cd0c750ada01781 in / 
# Wed, 11 Sep 2019 22:43:38 GMT
CMD ["bash"]
# Thu, 12 Sep 2019 05:55:39 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Sep 2019 05:55:39 GMT
ENV LANG=C.UTF-8
# Thu, 12 Sep 2019 13:58:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Oct 2019 23:20:37 GMT
ENV PYPY_VERSION=7.2.0
# Tue, 15 Oct 2019 23:21:14 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='aa128e555ad0fe5c4c15104ae0903052bd232b6e3a73f5fe023d27b8fd0d6089' ;; 		arm64) pypyArch='aarch64'; sha256='f82dc9dc6c692417ee9727f23beae75364a5757ebdc657a2a1d0010ac3ad17ab' ;; 		i386) pypyArch='linux32'; sha256='45e99de197cb3e974cfc8d45e0076ad2066852e61e56b3eafd1237efafd2c43e' ;; 		ppc64el) pypyArch='ppc64le'; sha256='6aef73a3b68e9a6c062cadd83d3db16790960cf97401ca6f2aad2195e9b05c35' ;; 		s390x) pypyArch='s390x'; sha256='a11da8118064db102d159e9221319c428b298c4a87f26166fd6ae94be8d6ae0d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	find /usr/local/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		pypy3 --version; 		if [ -f /usr/local/lib_pypy/_ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		cd /usr/local/lib_pypy; 		pypy3 _ssl_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 	find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Oct 2019 23:21:15 GMT
ENV PYTHON_PIP_VERSION=19.3
# Tue, 15 Oct 2019 23:21:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/65986a26949050d26e6ec98915da4aade8d8679d/get-pip.py
# Tue, 15 Oct 2019 23:21:15 GMT
ENV PYTHON_GET_PIP_SHA256=8d412752ae26b46a39a201ec618ef9ef7656c5b2d8529cdcbe60cd70dc94f40c
# Tue, 15 Oct 2019 23:21:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Oct 2019 23:21:34 GMT
CMD ["pypy3"]
# Wed, 16 Oct 2019 00:13:36 GMT
ENV HY_VERSION=0.17.0
# Wed, 16 Oct 2019 00:13:53 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Wed, 16 Oct 2019 00:13:53 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:16e2336ed3f3170046025d653edb3b949aab72dc5130b1452406847e32444b2b`  
		Last Modified: Wed, 11 Sep 2019 22:49:22 GMT  
		Size: 23.1 MB (23139280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08833067c6c7ece3cf735d9bebcd100bcb537ed6d868f4feef7f5409d4618cff`  
		Last Modified: Thu, 12 Sep 2019 14:01:59 GMT  
		Size: 3.3 MB (3321761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194321324f12d83e33decd6c1df9df8ac33c367fe39122ffd20f3ef521593951`  
		Last Modified: Tue, 15 Oct 2019 23:23:31 GMT  
		Size: 34.0 MB (33968943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202570e0b8996a1b426e93356c3c1bb7774cede2dc5786cca1c07d5630053507`  
		Last Modified: Tue, 15 Oct 2019 23:23:21 GMT  
		Size: 2.1 MB (2137918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023db7cd3d9315950f1aa485563c782392a6b5740bd1d413d79649792bbb0c55`  
		Last Modified: Wed, 16 Oct 2019 00:17:21 GMT  
		Size: 3.0 MB (2950340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy` - linux; s390x

```console
$ docker pull hylang@sha256:bc46a0008487f09fd973d82b904178831476e879f572e33fa608bc68451ab9a1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65069766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c92ab5b476b682cc3e5b0d1e1be51d84343b1f98975babd9979314a870ee29b`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 Sep 2019 22:44:13 GMT
ADD file:ec0f180243d217822dbf38503c62160c63e6adee835d76a8f9772c9cfbdb4b09 in / 
# Wed, 11 Sep 2019 22:44:13 GMT
CMD ["bash"]
# Thu, 12 Sep 2019 00:47:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Sep 2019 00:47:55 GMT
ENV LANG=C.UTF-8
# Thu, 12 Sep 2019 00:48:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libexpat1 		libffi6 		libgdbm3 		libsqlite3-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Oct 2019 22:56:43 GMT
ENV PYPY_VERSION=7.2.0
# Tue, 15 Oct 2019 22:57:16 GMT
RUN set -ex; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) pypyArch='linux64'; sha256='aa128e555ad0fe5c4c15104ae0903052bd232b6e3a73f5fe023d27b8fd0d6089' ;; 		arm64) pypyArch='aarch64'; sha256='f82dc9dc6c692417ee9727f23beae75364a5757ebdc657a2a1d0010ac3ad17ab' ;; 		i386) pypyArch='linux32'; sha256='45e99de197cb3e974cfc8d45e0076ad2066852e61e56b3eafd1237efafd2c43e' ;; 		ppc64el) pypyArch='ppc64le'; sha256='6aef73a3b68e9a6c062cadd83d3db16790960cf97401ca6f2aad2195e9b05c35' ;; 		s390x) pypyArch='s390x'; sha256='a11da8118064db102d159e9221319c428b298c4a87f26166fd6ae94be8d6ae0d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libncurses5 	; 		wget -O pypy.tar.bz2 "https://bitbucket.org/pypy/pypy/downloads/pypy3.6-v${PYPY_VERSION}-${pypyArch}.tar.bz2" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum -c; 	tar -xjC /usr/local --strip-components=1 -f pypy.tar.bz2; 	find /usr/local/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		pypy3 --version; 		if [ -f /usr/local/lib_pypy/_ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		cd /usr/local/lib_pypy; 		pypy3 _ssl_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 	find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Oct 2019 22:57:17 GMT
ENV PYTHON_PIP_VERSION=19.3
# Tue, 15 Oct 2019 22:57:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/65986a26949050d26e6ec98915da4aade8d8679d/get-pip.py
# Tue, 15 Oct 2019 22:57:17 GMT
ENV PYTHON_GET_PIP_SHA256=8d412752ae26b46a39a201ec618ef9ef7656c5b2d8529cdcbe60cd70dc94f40c
# Tue, 15 Oct 2019 22:57:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Oct 2019 22:57:34 GMT
CMD ["pypy3"]
# Tue, 15 Oct 2019 23:39:51 GMT
ENV HY_VERSION=0.17.0
# Tue, 15 Oct 2019 23:40:10 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Tue, 15 Oct 2019 23:40:10 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:dcc9fb138818bd495610317481ca5b236dccfeecf43998fc55d72e2d85ae592c`  
		Last Modified: Wed, 11 Sep 2019 22:48:31 GMT  
		Size: 22.4 MB (22362105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b30934dea02879a491bf2bd219c93ba21b53d77d013ddb2e792277e87ce808`  
		Last Modified: Thu, 12 Sep 2019 00:51:34 GMT  
		Size: 3.0 MB (3016223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a51ece90cac8d97ab2d24b4f653647580ad83eda5b28d69433dbb497593e3c`  
		Last Modified: Tue, 15 Oct 2019 22:58:42 GMT  
		Size: 34.6 MB (34603890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e13d43002f01b13afd797447eb004f2aff9b1f7ad71079a0b8daf11cf254f0`  
		Last Modified: Tue, 15 Oct 2019 22:58:33 GMT  
		Size: 2.1 MB (2137430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc3bcd2b1e4c449e04825cb162411ce3eac20e1fd9908b09830e9599a67e8ff`  
		Last Modified: Tue, 15 Oct 2019 23:45:15 GMT  
		Size: 3.0 MB (2950118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
