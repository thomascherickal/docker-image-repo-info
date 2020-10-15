## `hylang:python3.7-windowsservercore-1809`

```console
$ docker pull hylang@sha256:87127c43eb62fb0239601f21a366190552e16423538961888d00d424b4ba9f5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `hylang:python3.7-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull hylang@sha256:9755091aa92696dc6673686ed52e06498643703ab9d6abb358e62cca0f040ffd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2445703448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:391316c72f67bc28c070911f8b876e6deb24c4771e4fe09dba95780a6573d712`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 17:28:39 GMT
ENV PYTHON_VERSION=3.7.9
# Wed, 14 Oct 2020 17:28:39 GMT
ENV PYTHON_RELEASE=3.7.9
# Wed, 14 Oct 2020 17:30:20 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Oct 2020 17:30:21 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Wed, 14 Oct 2020 17:30:22 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Wed, 14 Oct 2020 17:30:23 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Wed, 14 Oct 2020 17:31:09 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 14 Oct 2020 17:31:10 GMT
CMD ["python"]
# Thu, 15 Oct 2020 00:28:07 GMT
ENV HY_VERSION=0.19.0
# Thu, 15 Oct 2020 00:28:45 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Thu, 15 Oct 2020 00:28:46 GMT
CMD ["hy"]
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
	-	`sha256:884423360f7ea1e96ee45c848772a79add61920245e053efb4137bd76e14e3d0`  
		Last Modified: Wed, 14 Oct 2020 17:35:34 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7237cd5eb712f1285ef8b6fa474b2a30e8adb52aa03adfc008afecf2311b7361`  
		Last Modified: Wed, 14 Oct 2020 17:35:33 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31aa099f817724ad4e63a8f8c35d1dea9a2d90da1fc9c398c2bd3d945a8501c`  
		Last Modified: Wed, 14 Oct 2020 17:35:42 GMT  
		Size: 55.8 MB (55835286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6a8c7d016f24a5babc5f8b281c666b50dc916395951a81ea876ce297418ed6`  
		Last Modified: Wed, 14 Oct 2020 17:35:31 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5a0fd798cf804476b9ba94b7b9f71ddc6c5af8cda0dfbda64171472f0ac60c`  
		Last Modified: Wed, 14 Oct 2020 17:35:30 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fe14c9305d8d536d26802840d7f2e1e5259120412bcb1b9257a828ac348632`  
		Last Modified: Wed, 14 Oct 2020 17:35:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48175c74684b2fa7d3bf47798660fada688ccb5b77c88b332baceeb6d2e512b`  
		Last Modified: Wed, 14 Oct 2020 17:35:33 GMT  
		Size: 10.2 MB (10238935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f1b3a4f6557d5a7d61c6936378977b55fa9ff289511c71e691a15ff733d098`  
		Last Modified: Wed, 14 Oct 2020 17:35:31 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad5b52fb08baa813b02bcecc8b55b743e8bc1cd0b8d82307a8517979f9ab5fd`  
		Last Modified: Thu, 15 Oct 2020 00:32:37 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084d2af32b8ada78ec800e7d0b0379c75004b818f6c879bf04eb1dbe04ae4db3`  
		Last Modified: Thu, 15 Oct 2020 00:32:43 GMT  
		Size: 5.5 MB (5528840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39663fb1a702013718ad88c4393c9cf5f41717cbf9ce0b91228b81bbfbe932eb`  
		Last Modified: Thu, 15 Oct 2020 00:32:37 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
