## `python:windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:26710727cccf993eee93766494965f8982d7b6088aa48cb816646332308468ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `python:windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull python@sha256:e2e59d2b1b0693207dbcf709730380b0ca0f613d8417b8d8c621754e9ba67453
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815453471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f52fa07643f34d2f95616b348c600e22dba1f2f45fa1aeced4b5d081622447b9`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 06 Oct 2020 21:15:12 GMT
ENV PYTHON_VERSION=3.9.0
# Tue, 06 Oct 2020 21:15:13 GMT
ENV PYTHON_RELEASE=3.9.0
# Tue, 06 Oct 2020 21:17:28 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Tue, 06 Oct 2020 21:17:29 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 06 Oct 2020 21:17:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 06 Oct 2020 21:17:31 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 06 Oct 2020 21:19:14 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 06 Oct 2020 21:19:15 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149c42daa8190082e42f8808bc7cf0ea6dec6c74229e03fe00515bbb09f6c179`  
		Last Modified: Tue, 06 Oct 2020 21:23:10 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00b7274a9a82be0b2ecca3a9680db8d159d6848c7ef329060b1440acdc65a41`  
		Last Modified: Tue, 06 Oct 2020 21:23:11 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39d4110832a95a0bda7f152a2270eca2270e6c859271feae8dfc30599dbac0c`  
		Last Modified: Tue, 06 Oct 2020 21:23:21 GMT  
		Size: 60.7 MB (60718909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595249670dd66e0b6951ec0a75a17019c8bec4af6b2ba4d4a27d0faf6b7e2584`  
		Last Modified: Tue, 06 Oct 2020 21:23:07 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc4ce13a3658161b9f8fbb5b8334c82e27ef658a4b005e067739e2251192c05`  
		Last Modified: Tue, 06 Oct 2020 21:23:08 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65c123e1e9c43abeaa07fefaac41f929da38fa35f54a7253c370c57af438b6d`  
		Last Modified: Tue, 06 Oct 2020 21:23:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec186298ee5fa873437301c6c23551e4236f1de57c381ccf34c320d223719dd`  
		Last Modified: Tue, 06 Oct 2020 21:23:13 GMT  
		Size: 15.5 MB (15472027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1a4b20a23379b3964de1419e1f25ad3ac7b8639d69b1c7b586db954f040acd`  
		Last Modified: Tue, 06 Oct 2020 21:23:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
