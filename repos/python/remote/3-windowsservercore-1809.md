## `python:3-windowsservercore-1809`

```console
$ docker pull python@sha256:74aa57cc293424c6215823c5d101dbf24cbe0248215dd79c47c12077b0532836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `python:3-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull python@sha256:04b9a552203a531b2cef40684ba125bf621612673e9d59811019eddde992211d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2504948693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b175d3ad77f16d96c0f4649a4323e17741d543e3cae1895e83fa6f5035f92269`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 19:12:32 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 13 Jan 2021 19:19:41 GMT
ENV PYTHON_VERSION=3.9.1
# Wed, 13 Jan 2021 19:19:42 GMT
ENV PYTHON_RELEASE=3.9.1
# Wed, 13 Jan 2021 19:21:24 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Mon, 25 Jan 2021 23:18:31 GMT
ENV PYTHON_PIP_VERSION=21.0
# Mon, 25 Jan 2021 23:18:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8cc88aca7d9775fce279e8b84ef163cf1d3e8a2e/get-pip.py
# Mon, 25 Jan 2021 23:18:33 GMT
ENV PYTHON_GET_PIP_SHA256=ffb67da2e976f48dd29714fc64812d1ac419eb7d48079737166dd95640d1debd
# Mon, 25 Jan 2021 23:19:23 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 25 Jan 2021 23:19:24 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f229e126d7cfc5407c75c0703062a138f0024cbcf6a1b318a0c87ba901af90a5`  
		Last Modified: Wed, 13 Jan 2021 19:41:55 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795b2d80b5b471ce01d3c4f7d00a67f836755c09b8e1f151637f663dccaf194`  
		Last Modified: Wed, 13 Jan 2021 19:43:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0084aa42c6bc6a8950ed3b47460f88adb1002c5bc244f2ba1d2d918140105acd`  
		Last Modified: Wed, 13 Jan 2021 19:42:58 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6baed7520f0a154fc50be558a3058fd26ecb5a3de62ac190b3338c6549b95ed5`  
		Last Modified: Wed, 13 Jan 2021 19:43:08 GMT  
		Size: 58.9 MB (58877690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a4d64960bb56f3bb3a1645248b8bfc37d811f8ea994da18bcc8bf663466a13`  
		Last Modified: Mon, 25 Jan 2021 23:29:51 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd2d5fdf942e55bc1530818ed67d782c492857e33100edfc62091cd19e9e6f0`  
		Last Modified: Mon, 25 Jan 2021 23:29:51 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41435b5a036b449b6c95a1576e6eb26617ab81bfae1388ee81662656d9549d70`  
		Last Modified: Mon, 25 Jan 2021 23:29:51 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec43e116550bfe2f99b53e4a060530df0bc3bde850cd13cb7ff6b7d3924aed6a`  
		Last Modified: Mon, 25 Jan 2021 23:29:54 GMT  
		Size: 10.3 MB (10288869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f53b506b8507a5da0c9f23a3386c8cd668f2b0ce0da5d2f3ca24fe7490120f`  
		Last Modified: Mon, 25 Jan 2021 23:29:51 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
