## `python:rc-windowsservercore-1809`

```console
$ docker pull python@sha256:5d8dbbaf09a82358fe5b42dd01755a215ef9ba7407a3127d51b1c4dec246285b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `python:rc-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull python@sha256:2f3de101a2ec79b514b6609fbb03d8a546f369b27db1cf74024dca8670eeac6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2738755252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbb1815b25e33ae49c19f7c2a3af636f4c97e341b9b55a323e68d18f2003dfb6`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:03:01 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 14 Jul 2021 04:03:03 GMT
ENV PYTHON_VERSION=3.10.0b4
# Wed, 14 Jul 2021 04:03:05 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 14 Jul 2021 04:05:03 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Mon, 02 Aug 2021 19:14:31 GMT
ENV PYTHON_PIP_VERSION=21.2.2
# Mon, 02 Aug 2021 19:14:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/a1675ab6c2bd898ed82b1f58c486097f763c74a9/public/get-pip.py
# Mon, 02 Aug 2021 19:14:36 GMT
ENV PYTHON_GET_PIP_SHA256=6665659241292b2147b58922b9ffe11dda66b39d52d8a6f3aa310bc1d60ea6f7
# Mon, 02 Aug 2021 19:16:09 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 02 Aug 2021 19:16:12 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e4f5fed4f2af1e948afc1185311a87f00d191ab9a40187441583dd496a2e6c`  
		Last Modified: Wed, 14 Jul 2021 04:20:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d14de1c64971d5e0f0f4e781c6232ba39b7a8dca520483196aad880aebb033`  
		Last Modified: Wed, 14 Jul 2021 04:20:41 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d92720cec2abb8b1d6e2c93bc9fa0c5b0120125332f8aa6758c84347505557`  
		Last Modified: Wed, 14 Jul 2021 04:20:41 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1236d0dda84e39c03c5aa046d53b3fefd38b9c7ec54f36abfabf5fc8b79b624f`  
		Last Modified: Wed, 14 Jul 2021 04:21:33 GMT  
		Size: 46.8 MB (46807394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4db8ede63d952872cc66814aba3232263793013a44bc12f027f4303a00883c`  
		Last Modified: Mon, 02 Aug 2021 19:22:51 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d82096468cc9f68847b4af8a114be7424c30d6a6e9061b8b547d391ce22a1a`  
		Last Modified: Mon, 02 Aug 2021 19:22:52 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafe8401e892d331df2c0b2863134f87c804a582ab0a4095fabc6785ee35dbd5`  
		Last Modified: Mon, 02 Aug 2021 19:22:51 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a49e616a2f6c56e78f1d9e87cd4be91faf540d7a462236325c8b238a7d2dcc`  
		Last Modified: Mon, 02 Aug 2021 19:22:59 GMT  
		Size: 6.5 MB (6489725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5ca3efbbbd521cddb5dddcd2147344653d24715162b6c7ece50c224536c99f`  
		Last Modified: Mon, 02 Aug 2021 19:22:52 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
