## `python:rc-windowsservercore-1809`

```console
$ docker pull python@sha256:f25d834b6c67131811b9b7980036df354a5c9149ed33f726d6635137e6a1fcd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `python:rc-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull python@sha256:375d0d5be71836d724c0d964aed6256362755c1f1b41f4f7c3460e60c91c863b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2504772073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba328c13459622082b5a1fea61d95d59df049083babd4c081db3aabfee0b4211`
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
# Wed, 13 Jan 2021 19:12:33 GMT
ENV PYTHON_VERSION=3.10.0a4
# Wed, 13 Jan 2021 19:12:34 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 13 Jan 2021 19:14:18 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Mon, 25 Jan 2021 23:15:06 GMT
ENV PYTHON_PIP_VERSION=21.0
# Mon, 25 Jan 2021 23:15:08 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8cc88aca7d9775fce279e8b84ef163cf1d3e8a2e/get-pip.py
# Mon, 25 Jan 2021 23:15:09 GMT
ENV PYTHON_GET_PIP_SHA256=ffb67da2e976f48dd29714fc64812d1ac419eb7d48079737166dd95640d1debd
# Mon, 25 Jan 2021 23:16:02 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 25 Jan 2021 23:16:04 GMT
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
	-	`sha256:f9ba3b72e7c8a7e1f1ded2154d31d1b7a807760255250e4c2537da280ace46a4`  
		Last Modified: Wed, 13 Jan 2021 19:41:54 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bca48002666e8ca6f802da0ddcc2385c9822559ef9feab39b4717187da034b`  
		Last Modified: Wed, 13 Jan 2021 19:41:55 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b1abe0979545ef03907a8e75b282eadae4bd033ba772668c7ebd23654af066`  
		Last Modified: Wed, 13 Jan 2021 19:42:09 GMT  
		Size: 58.6 MB (58643014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ecf18828beeb6dee5c50930df3d7a4ddc08a04df3e246e45d5854679098097`  
		Last Modified: Mon, 25 Jan 2021 23:29:17 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497d7b6c4b22bfd8238da2769ad129cdd3b2e7cf1cd815550b5d7a888e3eda70`  
		Last Modified: Mon, 25 Jan 2021 23:29:17 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a72c732e7623ccaaba0fb7c5fae33c8c2a128f459ecc0cfbfa14190b21330c`  
		Last Modified: Mon, 25 Jan 2021 23:29:17 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843ff0c671394bacde7d5dcc6b56b37f87666d189af40766234309083f9d7fd1`  
		Last Modified: Mon, 25 Jan 2021 23:29:20 GMT  
		Size: 10.3 MB (10346967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b9243817587aa245ea16e29957fe9049625dcf55faa35a207eca4da3205534`  
		Last Modified: Mon, 25 Jan 2021 23:29:17 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
