## `hylang:pypy3.8`

```console
$ docker pull hylang@sha256:f0ac7fae201f73d2c421976be38725d99e9c75d48cd81f540afedbb666a4d72b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; 386
	-	windows version 10.0.17763.2565; amd64

### `hylang:pypy3.8` - linux; amd64

```console
$ docker pull hylang@sha256:074186ac3cdb3e4af4a98b7adeb575f287c2032d1a2d139b538a808872e4ed2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73800036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d977d15eb74e3b26e67f1371643cb45c31c2a592c733fd1b3fb11a6b1da9e1e`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 01:40:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 01:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 01:40:53 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Mar 2022 01:40:53 GMT
ENV PYPY_VERSION=7.3.8
# Tue, 08 Mar 2022 05:18:45 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-linux64.tar.bz2'; 			sha256='089f8e3e357d6130815964ddd3507c13bd53e4976ccf0a89b5c36a9a6775a188'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='0210536e9f1841ba283c13b04783394050837bb3e6f4091c9f1bd9c7f2b94b55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-linux32.tar.bz2'; 			sha256='bea4b275decd492af6462157d293dd6fcf08a949859f8aec0959537b40afd032'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-s390x.tar.bz2'; 			sha256='ad53d373d6e275a41ca64da7d88afb6a17e48e7bfb2a6fff92daafdc06da6b90'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 08 Mar 2022 05:18:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 08 Mar 2022 05:18:45 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 08 Mar 2022 05:18:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Mar 2022 05:18:57 GMT
CMD ["pypy3"]
# Tue, 08 Mar 2022 09:18:30 GMT
ENV HY_VERSION=1.0a4
# Tue, 08 Mar 2022 09:18:31 GMT
ENV HYRULE_VERSION=0.1
# Tue, 08 Mar 2022 09:18:35 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 08 Mar 2022 09:18:35 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85840658c910f38522200d385220880921e0966db76c8fa51084fb39dfcbb859`  
		Last Modified: Wed, 02 Mar 2022 01:54:42 GMT  
		Size: 1.1 MB (1066001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f328d57be8b5b52631397af12d1bc6753056e05f12e91b6e48253b5f374c9f`  
		Last Modified: Tue, 08 Mar 2022 05:28:56 GMT  
		Size: 35.9 MB (35944869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e92f19ea6b6b328a732cedd32218ba5b6b246e892bed59a218952d95637f21`  
		Last Modified: Tue, 08 Mar 2022 05:28:50 GMT  
		Size: 2.6 MB (2631453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ad4705f8e5cdc577db8e1b8d144be522a980a18d82e5934550db175dd43920`  
		Last Modified: Tue, 08 Mar 2022 11:04:26 GMT  
		Size: 2.8 MB (2791317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - linux; 386

```console
$ docker pull hylang@sha256:a9a17ef7b29b2333f086bea2ff70230084626a2e65673c46b0c925f1730e1bb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74172894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa31c8574f65d314ed205bf0e4906e1dea3b16c72359dc9d5dd89cf8086b70e`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 21:18:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 21:18:08 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 21:18:08 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 21:18:08 GMT
ENV PYPY_VERSION=7.3.8
# Tue, 08 Mar 2022 04:00:01 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-linux64.tar.bz2'; 			sha256='089f8e3e357d6130815964ddd3507c13bd53e4976ccf0a89b5c36a9a6775a188'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='0210536e9f1841ba283c13b04783394050837bb3e6f4091c9f1bd9c7f2b94b55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-linux32.tar.bz2'; 			sha256='bea4b275decd492af6462157d293dd6fcf08a949859f8aec0959537b40afd032'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-s390x.tar.bz2'; 			sha256='ad53d373d6e275a41ca64da7d88afb6a17e48e7bfb2a6fff92daafdc06da6b90'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 08 Mar 2022 04:00:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 08 Mar 2022 04:00:02 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 08 Mar 2022 04:00:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Mar 2022 04:00:14 GMT
CMD ["pypy3"]
# Tue, 08 Mar 2022 04:32:31 GMT
ENV HY_VERSION=1.0a4
# Tue, 08 Mar 2022 04:32:31 GMT
ENV HYRULE_VERSION=0.1
# Tue, 08 Mar 2022 04:32:35 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 08 Mar 2022 04:32:35 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644e74815eb3f18f96bfa2e149a7a246bd0c7482f5681e0a9b0929bad87cdbeb`  
		Last Modified: Tue, 01 Mar 2022 21:39:32 GMT  
		Size: 1.1 MB (1078416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be008a69253632f5895c9ccd68821966b19058b691f4c865a9122e68f4e6aab5`  
		Last Modified: Tue, 08 Mar 2022 04:14:36 GMT  
		Size: 35.3 MB (35294616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748d2e6ac145cd77ada3277d01c199e695e840bcc7754ead85c87e0a508b9322`  
		Last Modified: Tue, 08 Mar 2022 04:14:28 GMT  
		Size: 2.6 MB (2631196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22c0b4afaf94f54767009d0daeea2348ff26f7da7c3459e9bbad534670e292b`  
		Last Modified: Tue, 08 Mar 2022 04:40:28 GMT  
		Size: 2.8 MB (2791277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - windows version 10.0.17763.2565; amd64

```console
$ docker pull hylang@sha256:255685849b9a0e343ceda9627ad9e8695871a9644c2b0659b76b98a1efe242c3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762068109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3763da34df45b36405e1651cec938deddb3ea1d098d1f383478c33bf59a3991`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 13:09:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Feb 2022 13:11:21 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 09 Feb 2022 13:12:34 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 23 Feb 2022 02:14:43 GMT
ENV PYPY_VERSION=7.3.8
# Wed, 23 Feb 2022 02:20:22 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.8-v7.3.8-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '0894c468e7de758c509a602a28ef0ba4fbf197ccdf946c7853a7283d9bb2a345'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.8-v7.3.8-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 23 Feb 2022 02:20:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 23 Feb 2022 02:20:25 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 23 Feb 2022 02:22:19 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 23 Feb 2022 02:22:20 GMT
CMD ["pypy3"]
# Wed, 23 Feb 2022 02:50:44 GMT
ENV HY_VERSION=1.0a4
# Wed, 23 Feb 2022 02:50:45 GMT
ENV HYRULE_VERSION=0.1
# Wed, 23 Feb 2022 02:52:12 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 23 Feb 2022 02:52:13 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f0c1566a9285d9465334dc923e9d6fd93a51b3ef6cb8497efcacbcf64e3b93fc`  
		Last Modified: Wed, 09 Feb 2022 13:26:13 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977ed2cf6839223b96336b95fbc7b18790a8c388e758a4b5f403696804739a5b`  
		Last Modified: Wed, 09 Feb 2022 13:26:12 GMT  
		Size: 356.8 KB (356819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090aceebb35b9bcb96fa341afc3e961eb65c37ed4bc746e7e03249273d754df9`  
		Last Modified: Wed, 09 Feb 2022 13:26:29 GMT  
		Size: 15.5 MB (15490453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c5d1f58c9ccb416475e7fa5abc5710e84a4ac8f6056172d00158c7cae3171c`  
		Last Modified: Wed, 23 Feb 2022 02:31:06 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a565cc760a2d39bed62e2827f303804769e84e5167a5eb8936bd9f1a54602c8`  
		Last Modified: Wed, 23 Feb 2022 02:31:54 GMT  
		Size: 26.0 MB (25950734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84669a85ad56c6d6c7f5697fc3824efce000f437f69085748b048709542aa0e`  
		Last Modified: Wed, 23 Feb 2022 02:31:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fdec1b0e3f802f8f9e3601a4ea25ac8f4481b026081cc382dc68af9ee8ef6d`  
		Last Modified: Wed, 23 Feb 2022 02:31:47 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2ea80c5c490b7acf9e148f8524930a187afb4672f36cb0370baea5f5d3f535`  
		Last Modified: Wed, 23 Feb 2022 02:31:48 GMT  
		Size: 3.0 MB (2986217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9654545f7adacf97c10c28e2887ca2bb9dba165a94c85f7bd107b0ae96c6b4`  
		Last Modified: Wed, 23 Feb 2022 02:31:47 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b35f1a69f85e6f6f7d702790a2671caba5152a4b98df794df7e03a5b0c5743`  
		Last Modified: Wed, 23 Feb 2022 02:54:34 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc52a846359e80fcccba7a2ea2e1dacf357899dc9b8b896e2eaa8ad8c67e220`  
		Last Modified: Wed, 23 Feb 2022 02:54:34 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a3553f87cd95a337ac2d93d49102a4c696599ffc885efc251c1af41ceddf12`  
		Last Modified: Wed, 23 Feb 2022 02:54:36 GMT  
		Size: 3.6 MB (3557809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4e2a51a6c7cf1887f71639c8bda44133b6754b2bb7064547163a0af98e9f4b`  
		Last Modified: Wed, 23 Feb 2022 02:54:35 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
