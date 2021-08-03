## `python:rc-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:2fae6f44da6946e941256be2264b7e75f3da999a523d5c29acac73fa8c1101de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `python:rc-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull python@sha256:87375e7219704cd7e999cafcd0e0b57eb0934ee31f686626fc8826d386053587
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6327325916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97e6ef718010c7563bf56197a0a0dc9fe119cbefc51aa268422e040bf033f13`
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
# Tue, 03 Aug 2021 20:19:06 GMT
ENV PYTHON_VERSION=3.10.0rc1
# Tue, 03 Aug 2021 20:19:09 GMT
ENV PYTHON_RELEASE=3.10.0
# Tue, 03 Aug 2021 20:21:30 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 03 Aug 2021 20:21:34 GMT
ENV PYTHON_PIP_VERSION=21.2.2
# Tue, 03 Aug 2021 20:21:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/a1675ab6c2bd898ed82b1f58c486097f763c74a9/public/get-pip.py
# Tue, 03 Aug 2021 20:21:38 GMT
ENV PYTHON_GET_PIP_SHA256=6665659241292b2147b58922b9ffe11dda66b39d52d8a6f3aa310bc1d60ea6f7
# Tue, 03 Aug 2021 20:23:22 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 03 Aug 2021 20:23:25 GMT
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
	-	`sha256:47a19592ef5fa869cd5f38850f49140db0672ee65674b7e0400e60494f908765`  
		Last Modified: Tue, 03 Aug 2021 20:24:41 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587cc1a23bbb215b8b77284d1336f7b836e6d4ef8509f9fcc794c7e5613d147c`  
		Last Modified: Tue, 03 Aug 2021 20:24:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59a7de0fbc9989b427071f5315a32386ed5dfe5c15d4ee91856954c1824a13f`  
		Last Modified: Tue, 03 Aug 2021 20:24:49 GMT  
		Size: 51.2 MB (51194728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a19ec0b130494f375c536343f1708caee5795fb732d4b3cc3b02e02933fce6`  
		Last Modified: Tue, 03 Aug 2021 20:24:38 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46ac31ca312f8eafb0c2abc90264d0f74c5cfb4e7b2fbe78e5b977bf4cedb8`  
		Last Modified: Tue, 03 Aug 2021 20:24:39 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f049c0e6b7bb7a827f42f44097eb3282e5f034992f7580a98da9f2349dd84b`  
		Last Modified: Tue, 03 Aug 2021 20:24:39 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64402476b29f2e170909af6c43bd90bc09ec4baa97a247c66d39b2265ac5cfe`  
		Last Modified: Tue, 03 Aug 2021 20:24:47 GMT  
		Size: 6.5 MB (6487822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9b731e934dee523d315889d73cfaa6f4f859cf9a4ece3ef4676e3404cf162`  
		Last Modified: Tue, 03 Aug 2021 20:24:39 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
