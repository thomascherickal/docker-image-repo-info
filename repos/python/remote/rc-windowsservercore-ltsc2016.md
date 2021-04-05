## `python:rc-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:ee21b2103c0863e95660751fd1b8f091e058c1747637a1c3e593008608eca67f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `python:rc-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull python@sha256:629e6951cf9ca25cf8594d42653a0111c29b6d6f1dffb2e00c73d0945b990141
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5868876600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:727f9b3066ba5d8617b94fe47edc8502b5e258a421b80d072563f5d13c132135`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 17:06:22 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 10 Mar 2021 17:06:23 GMT
ENV PYTHON_VERSION=3.10.0a6
# Wed, 10 Mar 2021 17:06:24 GMT
ENV PYTHON_RELEASE=3.10.0
# Mon, 05 Apr 2021 17:21:20 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Mon, 05 Apr 2021 17:21:22 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 05 Apr 2021 17:21:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/29f37dbe6b3842ccd52d61816a3044173962ebeb/public/get-pip.py
# Mon, 05 Apr 2021 17:21:24 GMT
ENV PYTHON_GET_PIP_SHA256=e03eb8a33d3b441ff484c56a436ff10680479d4bd14e59268e67977ed40904de
# Mon, 05 Apr 2021 17:23:23 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 05 Apr 2021 17:23:24 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d125fe0eea998b84d015b04287600700e6c6b273702461066209a3d1b9df51d0`  
		Last Modified: Wed, 10 Mar 2021 17:27:40 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3812ec54af73895848fd5a8e631fccae604338c7b2f59b7fd17cd9a7a51f2ea1`  
		Last Modified: Wed, 10 Mar 2021 17:27:37 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd7421109a179e409c8ea1226247e83bc6c3906692af334f5527b74b431b142`  
		Last Modified: Wed, 10 Mar 2021 17:27:39 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dbb0c6cc75df0f9b38a85f82391504bfaeb3331aa44c3c32af83f3f86e5b6c`  
		Last Modified: Mon, 05 Apr 2021 17:41:28 GMT  
		Size: 56.2 MB (56171824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6557b37c6ce4686f621a7463cb6b1e9ac2c5a2ed81b319db9af89a0b716a5d9`  
		Last Modified: Mon, 05 Apr 2021 17:41:14 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6603c8cd4e01f4b94cab1c291dfea3e481477bf785160f8305330a15765b2c`  
		Last Modified: Mon, 05 Apr 2021 17:41:15 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09a85086e54f8303e93246a9f1139b21c06963fa7b67d743986cf92162575ea`  
		Last Modified: Mon, 05 Apr 2021 17:41:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509b4bcc6cf9936a4e43f87090e5560b426184c39435ccc96f32a587da984230`  
		Last Modified: Mon, 05 Apr 2021 17:41:33 GMT  
		Size: 15.8 MB (15782695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a99b6482ba8c08632956600defd6adaad565b4a054454cf6a8417c6b552f45a`  
		Last Modified: Mon, 05 Apr 2021 17:41:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
