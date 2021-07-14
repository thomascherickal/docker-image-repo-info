## `python:rc-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:f226baeefe49426ff4c7987339d5b5b2f7d9490cd3acb5e9776b62783a91e759
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4530; amd64

### `python:rc-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull python@sha256:63a977b54e6073f7a03e8040768885fc248d2bb389dabf028616bbf2dba1e26e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6327254584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:945b0ddfed6974a6970d1fd45c867ca295ebf8bb526d87aa9aa35e52f5d10803`
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
# Wed, 14 Jul 2021 04:09:30 GMT
ENV PYTHON_PIP_VERSION=21.1.3
# Wed, 14 Jul 2021 04:09:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/a1675ab6c2bd898ed82b1f58c486097f763c74a9/public/get-pip.py
# Wed, 14 Jul 2021 04:09:36 GMT
ENV PYTHON_GET_PIP_SHA256=6665659241292b2147b58922b9ffe11dda66b39d52d8a6f3aa310bc1d60ea6f7
# Wed, 14 Jul 2021 04:11:26 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 14 Jul 2021 04:11:28 GMT
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
	-	`sha256:b1ab37780a4f64444c1f5cdd89be455b8d18c219aa0231cabc5a2ae878048ce0`  
		Last Modified: Wed, 14 Jul 2021 04:21:52 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a894e9645dce5d79c6d89f1ed2636450dbb0f0d5515580077f4c51a4e65f346`  
		Last Modified: Wed, 14 Jul 2021 04:21:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82678b05d80ed442d1f85b59425ab484a0621c21f10ae150e1af64c7860b171`  
		Last Modified: Wed, 14 Jul 2021 04:21:52 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5056bdce1a7a6ca8a0b52910a9cc0cb412c7620fcfbf05ea171ebd721a64036f`  
		Last Modified: Wed, 14 Jul 2021 04:22:00 GMT  
		Size: 6.4 MB (6427797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166098206d43f3654bd768c1417ca5bcbcd59351acc6898c130aa331408243d0`  
		Last Modified: Wed, 14 Jul 2021 04:21:52 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
