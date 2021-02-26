## `pypy:2-7-windowsservercore`

```console
$ docker pull pypy@sha256:1a284793ddebbb7ad885ae282d05c7cf19a4694af66c4798e1f0e10f0545bfe5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `pypy:2-7-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull pypy@sha256:8ff71b1fcb086ff1391c6224a3d53ff23e43190aaba95a00bc1fa421987039c8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2521924435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57b22a5082318c54690ef5933dcb38208ce9a8cf4a9902f5d3a0d2634cfbf071`
-	Default Command: `["pypy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 16:07:47 GMT
ENV PYTHONIOENCODING=UTF-8
# Fri, 26 Feb 2021 21:42:03 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Fri, 26 Feb 2021 21:42:34 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = '12a69af8623d70026690ba14139bf3793cc76c865759cad301b207c1793063ed'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Fri, 26 Feb 2021 21:42:35 GMT
ENV PYPY_VERSION=7.3.3
# Fri, 26 Feb 2021 21:43:34 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy2.7-v7.3.3-win32.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = 'b3e660dae8d25d8278fd6a0db77e76a16ac9a8c1dca22e7e103d39ed696dc69e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy2.7-v7.3.3-win32 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Fri, 26 Feb 2021 21:43:35 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Fri, 26 Feb 2021 21:43:37 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Fri, 26 Feb 2021 21:43:38 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Fri, 26 Feb 2021 21:44:52 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing "pip == {0}" ...' -f $env:PYTHON_PIP_VERSION); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Fri, 26 Feb 2021 21:44:53 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b84e06535ce9db874df389992b93e0bd5a992e8067ba9fc73059f40ef8966dd`  
		Last Modified: Wed, 10 Feb 2021 16:34:31 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aaabed8d9431a9b88fec37d271d466d5a4a71c5a858defbdc33c9218343e5e`  
		Last Modified: Fri, 26 Feb 2021 21:48:22 GMT  
		Size: 9.4 MB (9435820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af5416daeb845f767b7f048e64549ab789113414ee2524e7b11584c10229bc8`  
		Last Modified: Fri, 26 Feb 2021 21:48:24 GMT  
		Size: 18.2 MB (18195055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0329c0316aab3a05caff70bd828354dfa6a132d2e3a69a18b846f82f7af2d98c`  
		Last Modified: Fri, 26 Feb 2021 21:48:18 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765a8d2651aa91581c59b7ad0901e720e33753b53a27a59b969fe1f7a268ba5a`  
		Last Modified: Fri, 26 Feb 2021 21:48:30 GMT  
		Size: 48.0 MB (47952858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399601dd74aec9b51e04418168bfc3589d6eb6534f682f48236be7790c37a72c`  
		Last Modified: Fri, 26 Feb 2021 21:48:13 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca4ab541ff3723f7490c8874ba2fd20aeafe186fda60098237d3780b08ccae6`  
		Last Modified: Fri, 26 Feb 2021 21:48:16 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f636b5c8ba4929c627ad3d150dfd1183cb56d45096f8f4aac6335327839f885`  
		Last Modified: Fri, 26 Feb 2021 21:48:16 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b49a9d4b20fd33bae1776c45e62047e4b4bbd50b437abd662736f18be14c21`  
		Last Modified: Fri, 26 Feb 2021 21:48:15 GMT  
		Size: 7.1 MB (7064422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedfbb5793f94ba0d6cb27423c5ecf63808ae5ec1c344d82379b7cd13779542a`  
		Last Modified: Fri, 26 Feb 2021 21:48:16 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
