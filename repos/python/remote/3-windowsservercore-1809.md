## `python:3-windowsservercore-1809`

```console
$ docker pull python@sha256:6f9109401d370d2c11ba63a0c00a91b54863731f92b811f7a040dbd87b76592e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `python:3-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull python@sha256:aeb5b71d47f19d3d5866736bc1cd1c919dea69b34ef2954cb9eb6eaa9198708f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2444520550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58a542772251a2ebf9de1c70ac3662802b38191e7b204f4c7ddd3f8c90c2ab1`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 30 Oct 2020 00:18:21 GMT
ENV PYTHONIOENCODING=UTF-8
# Fri, 30 Oct 2020 00:25:15 GMT
ENV PYTHON_VERSION=3.9.0
# Fri, 30 Oct 2020 00:25:16 GMT
ENV PYTHON_RELEASE=3.9.0
# Fri, 30 Oct 2020 00:26:50 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Fri, 30 Oct 2020 00:26:51 GMT
ENV PYTHON_PIP_VERSION=20.2.4
# Fri, 30 Oct 2020 00:26:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8283828b8fd6f1783daf55a765384e6d8d2c5014/get-pip.py
# Fri, 30 Oct 2020 00:26:53 GMT
ENV PYTHON_GET_PIP_SHA256=2250ab0a7e70f6fd22b955493f7f5cf1ea53e70b584a84a32573644a045b4bfb
# Fri, 30 Oct 2020 00:27:36 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Fri, 30 Oct 2020 00:27:36 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb794c56bcd1cabc090769fa40a9a01dc0b440ce7fd0dfbd8d3e17dab67ebd04`  
		Last Modified: Fri, 30 Oct 2020 00:43:41 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e770b2482b45402433114ea803af4c03f9cbac46afdb11a750347997d88e4b6d`  
		Last Modified: Fri, 30 Oct 2020 00:45:30 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0271319ebf06e30249889512c57eacdfb7f4d4563116e62fcce6b3696a83e22`  
		Last Modified: Fri, 30 Oct 2020 00:45:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38474cb3c70b7dedb43a4782aa1aa462941f3d721ea04cc6471293d5da79d92`  
		Last Modified: Fri, 30 Oct 2020 00:46:39 GMT  
		Size: 60.1 MB (60103960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119320ea1e116d445a62f5acfda102995c8022b504de12a4ed6d4aee2cde63ed`  
		Last Modified: Fri, 30 Oct 2020 00:45:27 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0779b9fefa65407812d6850e3534c4492a4d8ddc876d82da8adc847ab2081169`  
		Last Modified: Fri, 30 Oct 2020 00:45:27 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2866be1a22ae3483ee11732de0bf267a2173bb424eba05975c74e69db0c0a6e1`  
		Last Modified: Fri, 30 Oct 2020 00:45:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c19c6b04fd218648a35d612e85bbfbf2e68a84bd47283d023635e962e070f1`  
		Last Modified: Fri, 30 Oct 2020 00:45:38 GMT  
		Size: 10.3 MB (10317397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9331355d43d5b2f3eaed0f4531a17692af363017d4e1332a76558d6c8b3b454f`  
		Last Modified: Fri, 30 Oct 2020 00:45:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
