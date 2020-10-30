## `python:3-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:8276b9b3e3ed28495855ad100582aad478bb277da30b388676aa95349f748f73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `python:3-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull python@sha256:690cec937034bb4f9f123f1b25e70235b14e5472d81ed8dbc18739c15bf13b2d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817581272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce338a36926a7a7f397f3b344c15c57b71c27fdf0c90e04083cb1e8daf1552c4`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 30 Oct 2020 00:14:08 GMT
ENV PYTHONIOENCODING=UTF-8
# Fri, 30 Oct 2020 00:21:03 GMT
ENV PYTHON_VERSION=3.9.0
# Fri, 30 Oct 2020 00:21:03 GMT
ENV PYTHON_RELEASE=3.9.0
# Fri, 30 Oct 2020 00:23:17 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Fri, 30 Oct 2020 00:23:18 GMT
ENV PYTHON_PIP_VERSION=20.2.4
# Fri, 30 Oct 2020 00:23:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8283828b8fd6f1783daf55a765384e6d8d2c5014/get-pip.py
# Fri, 30 Oct 2020 00:23:21 GMT
ENV PYTHON_GET_PIP_SHA256=2250ab0a7e70f6fd22b955493f7f5cf1ea53e70b584a84a32573644a045b4bfb
# Fri, 30 Oct 2020 00:24:57 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Fri, 30 Oct 2020 00:24:58 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dc0237500b170e70f7bea25e66289624b0f31aaaa023dcbd4e88ae406fe558`  
		Last Modified: Fri, 30 Oct 2020 00:41:49 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645dfafa3c7518a7472d8fa5a9fb9defd5ed4162020040c117c81d18f4db2c79`  
		Last Modified: Fri, 30 Oct 2020 00:44:59 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728a5de7ba4de256603d0b4bd879d11366be2893f2e1a33acc35ea092f5650c2`  
		Last Modified: Fri, 30 Oct 2020 00:44:59 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8e8cd56ce596cab7f5fd2a5d97cd305e9958cedbee8c7a20ca9634c9943a7e`  
		Last Modified: Fri, 30 Oct 2020 00:45:09 GMT  
		Size: 60.7 MB (60735449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73dd148eb11d4a14d271b6e9d87dbd0ae4a1cfe2f7f68a5b83ed53c62be4b24`  
		Last Modified: Fri, 30 Oct 2020 00:44:56 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e60b5f8e2ab83063b904d6da88909fb767a9bb3ac27a4fb99690e344bfc508`  
		Last Modified: Fri, 30 Oct 2020 00:44:57 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4e595e01d73b065a37198dfc926c0abbaca49004942dab3778ec96e685373c`  
		Last Modified: Fri, 30 Oct 2020 00:44:56 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d6f88c22dd7fa178f63811831fa8e6db267b0ba7283a5d4fa2cec63faef300`  
		Last Modified: Fri, 30 Oct 2020 00:45:04 GMT  
		Size: 15.5 MB (15484988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c29830f40a531c0889176844ddb21cd51023a7711d9b95fd8bbd637896a109`  
		Last Modified: Fri, 30 Oct 2020 00:44:56 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
