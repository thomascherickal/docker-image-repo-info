## `python:3-windowsservercore-1809`

```console
$ docker pull python@sha256:611435f53714ad354e31d5ef1909c801ee7d1f7ffead46a6f12d1df7b908fce6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `python:3-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull python@sha256:4108042ca7d27c233cc5897b11d1ec0a54ef55eefb04f8c614b36414d1647aec
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2504949946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:860d3977ed937875afad151c86b2a51c3e55a7fb7d43dba3dfbd8d065e163e6b`
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
# Mon, 01 Feb 2021 22:16:51 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 22:16:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 22:16:53 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 22:17:33 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 01 Feb 2021 22:17:34 GMT
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
	-	`sha256:e0f86b46a7eee328fde839c9b45abe4e246b9e01206f992495e0e119dbbc3819`  
		Last Modified: Mon, 01 Feb 2021 22:26:41 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c15433be82b12898185a0c71c6651779b2a3e34fa15a999e530c82881d8c49`  
		Last Modified: Mon, 01 Feb 2021 22:26:41 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a385af4eb7b88f7cf3230f3071cfa5cab8c53c3e6e2e9732bc32474718d1ef`  
		Last Modified: Mon, 01 Feb 2021 22:26:41 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825af99bf22a416d987486d332bab90f3b50225f4dbae0af1539b9e036db51b0`  
		Last Modified: Mon, 01 Feb 2021 22:26:44 GMT  
		Size: 10.3 MB (10290203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d838b52970fb46f8f70196973b320ca302a0b025296d4a66c2adfdb8baa04b`  
		Last Modified: Mon, 01 Feb 2021 22:26:41 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
