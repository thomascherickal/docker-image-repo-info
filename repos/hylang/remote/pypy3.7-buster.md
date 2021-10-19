## `hylang:pypy3.7-buster`

```console
$ docker pull hylang@sha256:742efc04a5e4b85f0f84441c746b7cf3560236ebde3de2d114928682f8626c52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `hylang:pypy3.7-buster` - linux; amd64

```console
$ docker pull hylang@sha256:6ed962a341caf3eb590444317dcfe7d28fb2243673e9d8b67e13fd8574255bae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.2 MB (72171683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:753080055b767a8be677aff49f2bdc35b91a2a1df189d1f02ee95ff47e580c34`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:10:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:10:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:10:11 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Oct 2021 21:40:05 GMT
ENV PYPY_VERSION=7.3.6
# Mon, 18 Oct 2021 21:40:35 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux64.tar.bz2'; 			sha256='c41d07063b1d002a91ad2a0763b4baaca2b306ec635889c2e4826e706cc7f9ca'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-aarch64.tar.bz2'; 			sha256='d446b6987eeaa03d706603863e83d6b99df69232cf1e06d3ee5706add6a84cd6'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux32.tar.bz2'; 			sha256='459e77c845b31fa9367f7b1b1122155f0ba7888b1d4ce4455c35d2111eeeb275'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-s390x.tar.bz2'; 			sha256='3659bf96a177a53426ffc38d3619c6ee307e600c80e924edc9cee604680c141d'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Mon, 18 Oct 2021 21:40:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Mon, 18 Oct 2021 21:40:36 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Mon, 18 Oct 2021 21:40:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 18 Oct 2021 21:40:53 GMT
CMD ["pypy3"]
# Mon, 18 Oct 2021 22:06:31 GMT
ENV HY_VERSION=1.0a3
# Mon, 18 Oct 2021 22:06:40 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 18 Oct 2021 22:06:40 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9691daf778691e301182cf757435ee1bd54288ea1f709d9f89568cb18cb64ad9`  
		Last Modified: Tue, 12 Oct 2021 16:18:00 GMT  
		Size: 2.8 MB (2757989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aafe8ae8396ca2acc77d553157eaf6b2f0ce099120adf468dd29fad922bf92a`  
		Last Modified: Mon, 18 Oct 2021 21:46:59 GMT  
		Size: 36.8 MB (36841281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c250a7c2fc5892df70c284a9d3c2f6a48e0da198ba344ae6208fb3a71f3fec4`  
		Last Modified: Mon, 18 Oct 2021 21:46:52 GMT  
		Size: 2.4 MB (2366237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b1b1f63e7eee41da48e5412c0bd3868ad60c9ff75bdd164a77c21b36bd695b`  
		Last Modified: Mon, 18 Oct 2021 22:08:39 GMT  
		Size: 3.1 MB (3066666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:1272a322aa852b5eb7c6d8d49ef33318346b2dc2153584605d6be1452fe77f05
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66855475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e9acaa1c1a1fbaa06643fddf0157bfc11daa60297bf9aeaad56b89368dc79f0`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 16:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 16:41:49 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 16:41:50 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Oct 2021 22:24:54 GMT
ENV PYPY_VERSION=7.3.6
# Mon, 18 Oct 2021 22:25:20 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux64.tar.bz2'; 			sha256='c41d07063b1d002a91ad2a0763b4baaca2b306ec635889c2e4826e706cc7f9ca'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-aarch64.tar.bz2'; 			sha256='d446b6987eeaa03d706603863e83d6b99df69232cf1e06d3ee5706add6a84cd6'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux32.tar.bz2'; 			sha256='459e77c845b31fa9367f7b1b1122155f0ba7888b1d4ce4455c35d2111eeeb275'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-s390x.tar.bz2'; 			sha256='3659bf96a177a53426ffc38d3619c6ee307e600c80e924edc9cee604680c141d'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Mon, 18 Oct 2021 22:25:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Mon, 18 Oct 2021 22:25:21 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Mon, 18 Oct 2021 22:25:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 18 Oct 2021 22:25:34 GMT
CMD ["pypy3"]
# Mon, 18 Oct 2021 23:24:45 GMT
ENV HY_VERSION=1.0a3
# Mon, 18 Oct 2021 23:24:56 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 18 Oct 2021 23:24:56 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f33f924dedcf5fbbc21c8d0606479984ab4304a4ae0b5f0351fe9ed1980959`  
		Last Modified: Wed, 13 Oct 2021 16:50:22 GMT  
		Size: 2.6 MB (2626756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a67d7a3f2620050d1e27bba318014ece2a5ab023b7d29fb1653d6e0ae7af11`  
		Last Modified: Mon, 18 Oct 2021 22:33:13 GMT  
		Size: 33.1 MB (33099927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa70da33d5b9bf021fa2333594c159c339cf7891f231a4291f431043d9511ee`  
		Last Modified: Mon, 18 Oct 2021 22:33:08 GMT  
		Size: 2.2 MB (2154105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c7aad9e9a9d738b5255b89f697f8e80429748e7aa9aee569790b7b6e035201`  
		Last Modified: Mon, 18 Oct 2021 23:28:21 GMT  
		Size: 3.1 MB (3066208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-buster` - linux; 386

```console
$ docker pull hylang@sha256:1c682c89abe58302dc5ab987853df3a5253bae9a992a6f923a7ffe011c411978
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74685990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe4d195c214232d379fe6415db8a98c25bcc793cf34b7091b0811196f0a14b66`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:54:02 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 09:54:03 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Oct 2021 21:49:17 GMT
ENV PYPY_VERSION=7.3.6
# Mon, 18 Oct 2021 21:49:49 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux64.tar.bz2'; 			sha256='c41d07063b1d002a91ad2a0763b4baaca2b306ec635889c2e4826e706cc7f9ca'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-aarch64.tar.bz2'; 			sha256='d446b6987eeaa03d706603863e83d6b99df69232cf1e06d3ee5706add6a84cd6'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux32.tar.bz2'; 			sha256='459e77c845b31fa9367f7b1b1122155f0ba7888b1d4ce4455c35d2111eeeb275'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-s390x.tar.bz2'; 			sha256='3659bf96a177a53426ffc38d3619c6ee307e600c80e924edc9cee604680c141d'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Mon, 18 Oct 2021 21:49:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Mon, 18 Oct 2021 21:49:50 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Mon, 18 Oct 2021 21:50:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 18 Oct 2021 21:50:02 GMT
CMD ["pypy3"]
# Mon, 18 Oct 2021 22:20:27 GMT
ENV HY_VERSION=1.0a3
# Mon, 18 Oct 2021 22:20:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 18 Oct 2021 22:20:36 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524c209c075137bc466a890c426fede913f5ca5e85b3773a09154d1c05a5fbc6`  
		Last Modified: Tue, 12 Oct 2021 10:04:42 GMT  
		Size: 2.8 MB (2769479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a38956c78e8143388bf5989c02295fbd7f0d382e8a949993c9ef573bb0a48ad`  
		Last Modified: Mon, 18 Oct 2021 21:59:05 GMT  
		Size: 38.7 MB (38692377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59edab33f25c468e86208cf63cce3016278f14b3e98fdf26b800a8e0efc3763d`  
		Last Modified: Mon, 18 Oct 2021 21:58:56 GMT  
		Size: 2.4 MB (2366002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6904f2c36f51ab5be11b39b9a3c5a70bf4b249fa7d5578be748d75a02151aef0`  
		Last Modified: Mon, 18 Oct 2021 22:24:31 GMT  
		Size: 3.1 MB (3066687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-buster` - linux; s390x

```console
$ docker pull hylang@sha256:edb3c056c656a620037e5643a742b04c6e5445fc3ccd1c6c15a9adb754bb79a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67427458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:533de9b1aeb2d2ca2f36425c12947b4c7c904ec8c04cdf4e69dd0067c8baff71`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 07:37:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 07:37:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 07:37:39 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Oct 2021 22:05:06 GMT
ENV PYPY_VERSION=7.3.6
# Mon, 18 Oct 2021 22:05:32 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux64.tar.bz2'; 			sha256='c41d07063b1d002a91ad2a0763b4baaca2b306ec635889c2e4826e706cc7f9ca'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-aarch64.tar.bz2'; 			sha256='d446b6987eeaa03d706603863e83d6b99df69232cf1e06d3ee5706add6a84cd6'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux32.tar.bz2'; 			sha256='459e77c845b31fa9367f7b1b1122155f0ba7888b1d4ce4455c35d2111eeeb275'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-s390x.tar.bz2'; 			sha256='3659bf96a177a53426ffc38d3619c6ee307e600c80e924edc9cee604680c141d'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Mon, 18 Oct 2021 22:05:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Mon, 18 Oct 2021 22:05:36 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Mon, 18 Oct 2021 22:05:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 18 Oct 2021 22:05:48 GMT
CMD ["pypy3"]
# Mon, 18 Oct 2021 22:25:31 GMT
ENV HY_VERSION=1.0a3
# Mon, 18 Oct 2021 22:25:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 18 Oct 2021 22:25:39 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc903ecfe37be2bc114c57a6a772f19f0f9fd9c9c99cd3513fb964b0bb9146ea`  
		Last Modified: Tue, 12 Oct 2021 07:39:05 GMT  
		Size: 2.5 MB (2452801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d7a25b9b0bffe12cfd2faa5d165bee14fda9885228121fb567ec533b1a0fcb`  
		Last Modified: Mon, 18 Oct 2021 22:07:15 GMT  
		Size: 33.8 MB (33787901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a387fc913171a1a96e9efe7d2a8d4d4c8a6351960aa6a72f5d33dff16cc8da53`  
		Last Modified: Mon, 18 Oct 2021 22:07:09 GMT  
		Size: 2.4 MB (2366059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735282625db03e96b92f2e7c67248df3476ede37c89fd63c7dd4bf8ace8c9bbe`  
		Last Modified: Mon, 18 Oct 2021 22:29:22 GMT  
		Size: 3.1 MB (3066445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
