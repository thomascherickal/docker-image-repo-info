## `python:3-windowsservercore`

```console
$ docker pull python@sha256:a25714d54030937be45371de3086013ce4d6a7a2c3874b76bb9087fa4a773da1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1366; amd64
	-	windows version 10.0.17763.3770; amd64

### `python:3-windowsservercore` - windows version 10.0.20348.1366; amd64

```console
$ docker pull python@sha256:7499a7308ebadd62d6d98b8796435f079d28e43244524cc9af4f0f56029677dd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2552152757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9c55ce9249987b188f64c69b70a127788fdb8f5d7d929cbe140016fe5398b56`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 09 Dec 2022 09:36:47 GMT
RUN Install update 10.0.20348.1366
# Tue, 13 Dec 2022 22:45:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Dec 2022 06:04:58 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 14 Dec 2022 06:13:03 GMT
ENV PYTHON_VERSION=3.11.1
# Wed, 14 Dec 2022 06:14:40 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 14 Dec 2022 06:14:42 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Fri, 06 Jan 2023 19:36:17 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Fri, 06 Jan 2023 19:36:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/66030fa03382b4914d4c4d0896961a0bdeeeb274/public/get-pip.py
# Fri, 06 Jan 2023 19:36:19 GMT
ENV PYTHON_GET_PIP_SHA256=1e501cf004eac1b7eb1f97266d28f995ae835d30250bec7f8850562703067dc6
# Fri, 06 Jan 2023 19:37:14 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Fri, 06 Jan 2023 19:37:15 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfa20ce142ecceb471dc070d9582fff942cef447b7c8ff22f2223ffe3737c99`  
		Last Modified: Tue, 13 Dec 2022 23:54:14 GMT  
		Size: 1.0 GB (1021665190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb8b9a4ec3ca516cfaa44f64e80b1e3aaecdbde870177411ff046f81f991dd2`  
		Last Modified: Tue, 13 Dec 2022 23:51:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c68370c3d49a9b3e8573290390ebab58e4c413205befb2943160fcff44e0a08`  
		Last Modified: Wed, 14 Dec 2022 06:30:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1443414f3afd900a891565d46286e6673040670a2a2d5f9b86c2130a1ad688c1`  
		Last Modified: Wed, 14 Dec 2022 06:31:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39c22de226773f3a2415f2edb8ea43f746fe28251da4ed46f016fed76fbcb70`  
		Last Modified: Wed, 14 Dec 2022 06:32:05 GMT  
		Size: 50.6 MB (50606076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f3ab17e1b2a2ec478eb467e4900b1e0cbfa3d471225f24df852c5ee576bfd0`  
		Last Modified: Wed, 14 Dec 2022 06:31:50 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdc73ce0f216b9256c44c210b926e3dc30fc61e74fd06595c90df3892d2495d`  
		Last Modified: Fri, 06 Jan 2023 19:43:45 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce282227b628600576ea796875e86f89e8ba0d15cebfbe699a17e0641eb40260`  
		Last Modified: Fri, 06 Jan 2023 19:43:45 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7654e5342c989b7160357fd40cb30151986270f47d3e2d14162f47f07d527358`  
		Last Modified: Fri, 06 Jan 2023 19:43:45 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc40204bf804c82ab0616a076a5ba8b543a9ad83fa593da01156352dbfd153d0`  
		Last Modified: Fri, 06 Jan 2023 19:43:47 GMT  
		Size: 5.9 MB (5872490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691e2a73ceb2d0ab4de89febe0f5e7fb4049e89c50c4b271d7e4ce15db259904`  
		Last Modified: Fri, 06 Jan 2023 19:43:45 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-windowsservercore` - windows version 10.0.17763.3770; amd64

```console
$ docker pull python@sha256:17d6bfe14778464aa4582a2e8cecf2c21be15bbb1ab947b01ad501973305d4a7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2836796140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc95b2af33c31f9a8844440241d2bb8bae867f645ec78a45b9f91c7b134cb274`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Tue, 13 Dec 2022 22:48:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Dec 2022 06:08:13 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 14 Dec 2022 06:16:17 GMT
ENV PYTHON_VERSION=3.11.1
# Wed, 14 Dec 2022 06:18:37 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 14 Dec 2022 06:18:38 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Fri, 06 Jan 2023 19:37:32 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Fri, 06 Jan 2023 19:37:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/66030fa03382b4914d4c4d0896961a0bdeeeb274/public/get-pip.py
# Fri, 06 Jan 2023 19:37:33 GMT
ENV PYTHON_GET_PIP_SHA256=1e501cf004eac1b7eb1f97266d28f995ae835d30250bec7f8850562703067dc6
# Fri, 06 Jan 2023 19:39:16 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Fri, 06 Jan 2023 19:39:17 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9debb9503ac53c2f64685982eca56ac5110ea6baf7278b27af54ab8fbc409`  
		Last Modified: Tue, 13 Dec 2022 23:54:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8587266d5d0bc3c248349db1d03442ca00c2d54740997f42104985cb6d808f`  
		Last Modified: Wed, 14 Dec 2022 06:31:24 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c308ce38695050025ec0cc9a87503f4ceefcc6405ce487b2d71cfff8a73dfc9`  
		Last Modified: Wed, 14 Dec 2022 06:32:24 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730c20f0500d72b14d1c5f910b95556ace944bf925f86ffb46880d1031926a19`  
		Last Modified: Wed, 14 Dec 2022 06:32:37 GMT  
		Size: 50.4 MB (50406737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a6b87f792e5cecb966b18c2ea385ad041b9ec0279ce6b4c467f62edb7d154a`  
		Last Modified: Wed, 14 Dec 2022 06:32:23 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a40b73046ead67a402d3f0591c76c090d2b8a56713078645221afa818f33d`  
		Last Modified: Fri, 06 Jan 2023 19:44:00 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4dd4e8aa0952210caa25f0c3733e6a50ef5a5fc0cf8f025f776e255db2b328`  
		Last Modified: Fri, 06 Jan 2023 19:44:00 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d46f38e1429acec728ce40f73d5d1a41a0afb36cd28b3a0e49d313fa279faa4`  
		Last Modified: Fri, 06 Jan 2023 19:44:00 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e284421736624056ec5ba54aafae1e98fe8c4284dac2a479e5eff905a205c56`  
		Last Modified: Fri, 06 Jan 2023 19:44:01 GMT  
		Size: 5.7 MB (5680863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de61f5375f1887f09232daefb482a0b9030acc00ca2a9ff417102a662ab0cd6f`  
		Last Modified: Fri, 06 Jan 2023 19:44:00 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
