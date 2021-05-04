## `hylang:python3.8-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:b3e7c1ea3dd5a4c254f8b37fffc664ba9e640800db1201480d2023b3e1244407
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `hylang:python3.8-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull hylang@sha256:3becc276bfa80063845d2b1bdfb05637654377588cb31b448e766546c5963616
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5871591788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13305011493ddfac93dffe62001c7fdcec61ca72f593c09eff0ed457983e42c7`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 16:15:18 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 04 May 2021 17:31:35 GMT
ENV PYTHON_VERSION=3.8.10
# Tue, 04 May 2021 17:31:36 GMT
ENV PYTHON_RELEASE=3.8.10
# Tue, 04 May 2021 17:33:59 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 04 May 2021 17:34:01 GMT
ENV PYTHON_PIP_VERSION=21.1.1
# Tue, 04 May 2021 17:34:03 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1954f15b3f102ace496a34a013ea76b061535bd2/public/get-pip.py
# Tue, 04 May 2021 17:34:04 GMT
ENV PYTHON_GET_PIP_SHA256=f499d76e0149a673fb8246d88e116db589afbd291739bd84f2cd9a7bca7b6993
# Tue, 04 May 2021 17:35:46 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 04 May 2021 17:35:47 GMT
CMD ["python"]
# Tue, 04 May 2021 18:00:24 GMT
ENV HY_VERSION=1.0a1
# Tue, 04 May 2021 18:01:48 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Tue, 04 May 2021 18:01:49 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b4598ab88dab64b25b4257872564af9825cc6cd41fc8cc1ad11c32958d0da9`  
		Last Modified: Wed, 14 Apr 2021 16:39:38 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c54b739697cab0ca2370a7ad528104932d4e2fadf2cb7ad6da8e89b73f714fc`  
		Last Modified: Tue, 04 May 2021 17:39:57 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f61aac09841e518e1317307f0577eaf833fc32d0a9a5cb4908f5b05ddda4a0a`  
		Last Modified: Tue, 04 May 2021 17:39:57 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6362feebbd7508c3dba997080be08be03292d4819dcf798480a7aeef4eb92a66`  
		Last Modified: Tue, 04 May 2021 17:40:06 GMT  
		Size: 58.8 MB (58783087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58243a2c7f6ad5ee4e3bab8a37da279b1c6e76b0d15d337eea9434e17484646`  
		Last Modified: Tue, 04 May 2021 17:39:54 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955d64d56c5272ecb02bbbdcbba14b724b0fd4a763afb9ad332daff894daf092`  
		Last Modified: Tue, 04 May 2021 17:39:54 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c92a270582606b037215673d116a9084f2de6bfdd5ed977ad0abf30b3944457`  
		Last Modified: Tue, 04 May 2021 17:39:54 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcd486eb103ff0b2302b8fdc4233e77ded81ae26d9d38a820af6c2d233c91a9`  
		Last Modified: Tue, 04 May 2021 17:39:57 GMT  
		Size: 11.4 MB (11443314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f500900696a12514df0aba2b9c8a4619a77f5246b1f207eb16ca18bf2378a3ac`  
		Last Modified: Tue, 04 May 2021 17:39:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4377095f29468f2482b77f12ac45d6b1aa9a850b5bac392f5a30e336bd6453`  
		Last Modified: Tue, 04 May 2021 18:06:17 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068d8aea6c824fd21fbb7ab632b66575ed6411f1d4485f708e5840be448d0774`  
		Last Modified: Tue, 04 May 2021 18:06:19 GMT  
		Size: 6.5 MB (6467506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4214916a59bd4c974ee29fcd5c6a17bc9787daf6ebf0d3e9a804820a7cea78`  
		Last Modified: Tue, 04 May 2021 18:06:17 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
