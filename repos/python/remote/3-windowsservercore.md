## `python:3-windowsservercore`

```console
$ docker pull python@sha256:29ef76dce24736714d60a5d738c4838033bb50b4c0584da67ad376e456c8d98b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `python:3-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull python@sha256:4d6ad94e94ebf0ee499d3e50c8bac18bd2200d38f351576fc9851a27434c438a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2459984427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b74f2e28c3ce4c4bc7d69af6706f80e7f5ef0b5dad8173bf16125219d4a3ef`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 17:43:53 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 09 Dec 2020 17:50:46 GMT
ENV PYTHON_VERSION=3.9.1
# Wed, 09 Dec 2020 17:50:47 GMT
ENV PYTHON_RELEASE=3.9.1
# Wed, 09 Dec 2020 17:52:27 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 09 Dec 2020 17:52:28 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Wed, 09 Dec 2020 17:52:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Wed, 09 Dec 2020 17:52:30 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Wed, 09 Dec 2020 17:53:17 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 09 Dec 2020 17:53:17 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94dd2e25fa016037458dfad84ce68c5f51c1d9a517cbb1d6a9d9037fb27a47b`  
		Last Modified: Wed, 09 Dec 2020 18:12:33 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43c1e1f0964479f228315ffd503fded10414f92c67f89d956a85cd6afbb593e`  
		Last Modified: Wed, 09 Dec 2020 18:13:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4905032a1c78aca05b445c178cfb9f2b232e664998995eec7a7ec6c5e9c0a11`  
		Last Modified: Wed, 09 Dec 2020 18:13:35 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c025c30481676471955858b2228cc152047dd812f258db8bb69da882bdfc85d`  
		Last Modified: Wed, 09 Dec 2020 18:13:44 GMT  
		Size: 58.8 MB (58753562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897c43b058d364c0cfe42936994f818c9a8b09b0ea08bb55aa6fc819d1ed2166`  
		Last Modified: Wed, 09 Dec 2020 18:13:33 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f8f24f052dc99033501acebee22fac2231edee372a691b66e128b885d2486d`  
		Last Modified: Wed, 09 Dec 2020 18:13:32 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ab626fe701f307562f1e26401acffce062852c9f94f8594c06bee4ce07f9e8`  
		Last Modified: Wed, 09 Dec 2020 18:13:32 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b216f88a03dd996b4d093e4bd48c81c3228f56ecb408ca5474a05f3ff2f68026`  
		Last Modified: Wed, 09 Dec 2020 18:13:50 GMT  
		Size: 10.3 MB (10347266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f2d6922b1ca8f13967e7ed7af3f36f964f09aa3fa5fe8e15e7570cb232bf81`  
		Last Modified: Wed, 09 Dec 2020 18:13:32 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull python@sha256:9ce7afa14a81778ee17773f926931b87da7e3985a393c5bf49c80a4c4289d036
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5844029938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d866ede06291b789f8dfdf8aa3b0986295b32cf13902094bde50accd98f1fcbf`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 17:46:34 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 09 Dec 2020 17:53:27 GMT
ENV PYTHON_VERSION=3.9.1
# Wed, 09 Dec 2020 17:53:28 GMT
ENV PYTHON_RELEASE=3.9.1
# Wed, 09 Dec 2020 17:55:43 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 09 Dec 2020 17:55:44 GMT
ENV PYTHON_PIP_VERSION=20.3.1
# Wed, 09 Dec 2020 17:55:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/91630a4867b1f93ba0a12aa81d0ec4ecc1e7eeb9/get-pip.py
# Wed, 09 Dec 2020 17:55:45 GMT
ENV PYTHON_GET_PIP_SHA256=d48ae68f297cac54db17e4107b800faae0e5210131f9f386c30c0166bf8d81b7
# Wed, 09 Dec 2020 17:57:28 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 09 Dec 2020 17:57:29 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18db14afcdaf52f01f53af42090925b5c891dfe60bedf017c011f3a9f08413b`  
		Last Modified: Wed, 09 Dec 2020 18:13:02 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ca29429f89cd854a8f504abd4eab2422cc201417b761cb25739da44e3d8f17`  
		Last Modified: Wed, 09 Dec 2020 18:14:13 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1653b9b41b03210c8d1c3c8e78f6f3b736d190f1e837b58e198b57564904287e`  
		Last Modified: Wed, 09 Dec 2020 18:14:13 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcfda6dd459e164fb22907204f47203086a18db50ac0fc85c2332ece599eb7b`  
		Last Modified: Wed, 09 Dec 2020 18:15:21 GMT  
		Size: 59.5 MB (59511092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffe81a4096bff4d1bf0523da2616ea9b1f60e9a4f2ea316062cca468f359bd6`  
		Last Modified: Wed, 09 Dec 2020 18:14:10 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2885308362db6236732ab5d3c4b08585b50ba5c271b2962981d7260d4dce0a5f`  
		Last Modified: Wed, 09 Dec 2020 18:14:10 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582349fec9eadd94781cd3719864cc1329516eb1c5acaad75a5468241f656041`  
		Last Modified: Wed, 09 Dec 2020 18:14:11 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d5ce8d444da26a15b607a6da87306131802e476db2b93eec8f33b96a36aa28`  
		Last Modified: Wed, 09 Dec 2020 18:14:14 GMT  
		Size: 15.7 MB (15665700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d9625bb9cca0bf263ae33004e926769ccd433ef06a9d2c36df018cd0bdeac0`  
		Last Modified: Wed, 09 Dec 2020 18:14:09 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
