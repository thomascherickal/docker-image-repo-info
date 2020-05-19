## `python:rc-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:da8145ee8601eb55fd693a0cdb296919f7f07916210038ea4eabca620bd1c0bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `python:rc-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull python@sha256:ac65b2ba08e6bd2181a6aedc1c4f2d188c608a0082b5819f3eb9847185b66605
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5800691340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbcb1a9d62fb00f112c4638a26aafd5536ec5ea6383a201087f01a3fb1df9a0d`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 12:34:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 19 May 2020 19:15:23 GMT
ENV PYTHON_VERSION=3.9.0b1
# Tue, 19 May 2020 19:15:24 GMT
ENV PYTHON_RELEASE=3.9.0
# Tue, 19 May 2020 19:18:05 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Tue, 19 May 2020 19:18:08 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Tue, 19 May 2020 19:18:09 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Tue, 19 May 2020 19:18:11 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Tue, 19 May 2020 19:19:53 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 19 May 2020 19:19:55 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e3e9730c43354781e87aa51e853bff3b1e8c1ca7004f527139638a8f9d499c49`  
		Last Modified: Wed, 13 May 2020 12:59:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099f5956d258c85ceb32669bf037c94bce00b6caab6fd161cf224b12620ba443`  
		Last Modified: Tue, 19 May 2020 19:29:28 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45397c0d1865bdf244f6f9ff24e0d9e9ffe9aff79c4271dff4b76be304bd2be`  
		Last Modified: Tue, 19 May 2020 19:29:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9906f004feaa540cb9faff14d6d26718d5da9b40061a6bbd9dd39466caec297e`  
		Last Modified: Tue, 19 May 2020 19:29:38 GMT  
		Size: 58.2 MB (58232342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563497d7199d4439a673e51dd9c17a4412c7f8dc1a823ce933a58d6c74c1c6e8`  
		Last Modified: Tue, 19 May 2020 19:29:25 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1625915a06f61d20f2b5f9f720654a7a7ce920b19108df12e47b6aca6457ac5`  
		Last Modified: Tue, 19 May 2020 19:29:25 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cdda8f05f37fb3b5fd77b4f57532f6241ecfaba0cc883e7e0d1340381db8c2`  
		Last Modified: Tue, 19 May 2020 19:29:25 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530b28b75805f6369caed9922e59c2c3de7f9116271e7aa14af619f01459bb4a`  
		Last Modified: Tue, 19 May 2020 19:29:30 GMT  
		Size: 10.6 MB (10561118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be72d6fb78c6ec5e484744845128bb0fd5927d71d6118ed284cacf866556ffef`  
		Last Modified: Tue, 19 May 2020 19:29:24 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
