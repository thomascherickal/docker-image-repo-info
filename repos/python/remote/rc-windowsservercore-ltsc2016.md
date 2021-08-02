## `python:rc-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:fbd2c23248ab0176a85aa2aa833d9977fe1f04a795b74dbba4e42c328bce3fc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `python:rc-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull python@sha256:d6b0d926212793b9d496e69a0ace85865854d5532f472bf58decca6edcc55b2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6327313532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92538a1052372c9e49404e87466ca277335cc2a11d6caf4351910cc8f7d6233e`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:06:58 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 14 Jul 2021 04:07:01 GMT
ENV PYTHON_VERSION=3.10.0b4
# Wed, 14 Jul 2021 04:07:04 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 14 Jul 2021 04:09:28 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Mon, 02 Aug 2021 19:16:27 GMT
ENV PYTHON_PIP_VERSION=21.2.2
# Mon, 02 Aug 2021 19:16:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/a1675ab6c2bd898ed82b1f58c486097f763c74a9/public/get-pip.py
# Mon, 02 Aug 2021 19:16:31 GMT
ENV PYTHON_GET_PIP_SHA256=6665659241292b2147b58922b9ffe11dda66b39d52d8a6f3aa310bc1d60ea6f7
# Mon, 02 Aug 2021 19:18:26 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 02 Aug 2021 19:18:29 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718585791498e9078e8a473986df9b8d4c6a9a5b8cb08e95e3919fdf469f843b`  
		Last Modified: Wed, 14 Jul 2021 04:21:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170af7b0ea5ed4afd2e7ef33694146d74c3b39214ada23d13982413f0694138f`  
		Last Modified: Wed, 14 Jul 2021 04:21:55 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ac49e5f2c574f9267e327aa23641f061159e13eb9cb55c7710a9ea4658e004`  
		Last Modified: Wed, 14 Jul 2021 04:21:55 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6b6415ea022f801c631ae1ef6c0fb587d05787b67d8583ba2acc0c341e8f33`  
		Last Modified: Wed, 14 Jul 2021 04:22:55 GMT  
		Size: 51.2 MB (51183628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac566ce33c8c5976efba0b48b286939a2be7518e2b809fe73e1e17f3fb53c2f`  
		Last Modified: Mon, 02 Aug 2021 19:23:15 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c63319ca09c07308094bc313ec82324adee1d79f4a7c8856795aec55562f52`  
		Last Modified: Mon, 02 Aug 2021 19:23:15 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861eca4de37fcde1e79bc3e654204427f7106c1e67c82f5ada93188d8f0d14bb`  
		Last Modified: Mon, 02 Aug 2021 19:23:15 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278d3525257cf07194bb9add9da1450d78c50fba107bec04ed5e138ba7dc1982`  
		Last Modified: Mon, 02 Aug 2021 19:23:18 GMT  
		Size: 6.5 MB (6486564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a125c5096c0462e78ea72b3b38ee9fed5393253478b533dcfab6f49db7c35e8`  
		Last Modified: Mon, 02 Aug 2021 19:23:16 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
