## `pypy:3-7-windowsservercore`

```console
$ docker pull pypy@sha256:59a405b4b6c345587892857063ab650602abbdc22ae663da0d4ec2cb4c6bb3cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2113; amd64
	-	windows version 10.0.17763.5122; amd64

### `pypy:3-7-windowsservercore` - windows version 10.0.20348.2113; amd64

```console
$ docker pull pypy@sha256:2812cf61f8cddded3afc0352b2edfb519493f6577af881ef22a591dec401da28
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1932659397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73e6d7d464dcc1f5c742e9374361dd0c675ee9d59182e81376dc2ff49540d031`
-	Default Command: `["pypy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 07:42:28 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Thu, 16 Nov 2023 07:42:59 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 16 Nov 2023 07:43:00 GMT
ENV PYPY_VERSION=7.3.13
# Thu, 16 Nov 2023 07:43:57 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.10-v7.3.13-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '5b99422fb8978b2f4bbf97961bca49963a82dc47c2fa51b7d23c493db3a2e0f0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.10-v7.3.13-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 16 Nov 2023 07:43:58 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 16 Nov 2023 07:43:59 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 16 Nov 2023 07:45:18 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 16 Nov 2023 07:45:19 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0520b952359e3af7287fcc142829a9521346bde390d4a8d361ea8eb9da2f9ad`  
		Last Modified: Thu, 16 Nov 2023 08:54:24 GMT  
		Size: 457.9 KB (457936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed00290516415425e4ecf4addafc1634ef66c6f927439e33fce310e647c65f88`  
		Last Modified: Thu, 16 Nov 2023 08:54:26 GMT  
		Size: 15.5 MB (15460173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e13047ae2bb17e9dcef20d1e9816167c772ef92c98f9d54983b02bdfd7f3f4`  
		Last Modified: Thu, 16 Nov 2023 08:54:24 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657cda163cc049ad04047ab9b7418163b1020e6d5a4ec65f212bb66808de33a4`  
		Last Modified: Thu, 16 Nov 2023 08:54:29 GMT  
		Size: 26.1 MB (26111453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcc10768ba128ec08f20edfb80249408cf39f3235905564875332b239e7b122`  
		Last Modified: Thu, 16 Nov 2023 08:54:22 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ad4294d2ddee60d3c2a6543f116c0d4669c69e15ae0537163a6fcdc350d8dc`  
		Last Modified: Thu, 16 Nov 2023 08:54:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928a9cc1bcd0089e9f0952898e27a47305513ce517865269966481481067f4`  
		Last Modified: Thu, 16 Nov 2023 08:54:24 GMT  
		Size: 3.8 MB (3841383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60807da1658bd15501c241806659b757935f374f655f5d610acebc3b889c34cd`  
		Last Modified: Thu, 16 Nov 2023 08:54:22 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:3-7-windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull pypy@sha256:45c7532e5a6596beee450c9f9c6a9b08b4f664c30f12071b20893a7bf5c137f7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2103243619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed3b148b47f7f4905bb8cd7d8dd4cf790c894cc1d348d0eec42bd454560ae59`
-	Default Command: `["pypy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 07:46:44 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Thu, 16 Nov 2023 07:48:07 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 16 Nov 2023 07:48:08 GMT
ENV PYPY_VERSION=7.3.13
# Thu, 16 Nov 2023 07:49:54 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.10-v7.3.13-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '5b99422fb8978b2f4bbf97961bca49963a82dc47c2fa51b7d23c493db3a2e0f0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.10-v7.3.13-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 16 Nov 2023 07:49:55 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 16 Nov 2023 07:49:56 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 16 Nov 2023 07:52:05 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 16 Nov 2023 07:52:06 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e430ddef0312e491229f8dfb31c1c4b5a4c5c2376b98a14535ce6c5a80ffb943`  
		Last Modified: Thu, 16 Nov 2023 08:54:59 GMT  
		Size: 438.1 KB (438076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5a86f421addaeba63d93e1af89aaeb9017a3ecc28ebdc0de7cb683e7349980`  
		Last Modified: Thu, 16 Nov 2023 08:55:02 GMT  
		Size: 15.4 MB (15437374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d52bc09e21e8ea36cdaf8bdf8228a3ba92b7b60d10a6705e89e33532615362`  
		Last Modified: Thu, 16 Nov 2023 08:54:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36070f329097c467ca7c995acfeeabe8328963d78fe0fcf385d0beee9ba636e4`  
		Last Modified: Thu, 16 Nov 2023 08:55:03 GMT  
		Size: 26.1 MB (26096439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c777ed6751299fc9eba701e0999e79a7b3b1d85edab553c15985e280e1a103e4`  
		Last Modified: Thu, 16 Nov 2023 08:54:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e7cb799409d734d8cc250e90a939e7a6844176af150cfd124399dc7cab98fe`  
		Last Modified: Thu, 16 Nov 2023 08:54:57 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18779e6b68f6df91ac675e8749b33a8a626a6389d85bd43fab653e1a2118cb02`  
		Last Modified: Thu, 16 Nov 2023 08:54:58 GMT  
		Size: 3.8 MB (3833122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49a8f9aeb4b448ed794fe34a7cb40bd7797b4da4ea35e9942632a3402f54d7c`  
		Last Modified: Thu, 16 Nov 2023 08:54:56 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
