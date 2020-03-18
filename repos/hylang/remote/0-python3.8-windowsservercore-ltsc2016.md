## `hylang:0-python3.8-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:162d79620d65403518145fadf78b61ad2b16d0232566b31592dfaf0491f474db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `hylang:0-python3.8-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull hylang@sha256:e745f2ea08b163d51f01019fd7df684e60d533701c46a7c44b3a9856f05e6220
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802439730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b9689da4b1c03c8fc34e663cfa25afd2b2c1b244610ef34d912e2c42a8d0bd9`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Fri, 13 Mar 2020 21:32:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 13:47:28 GMT
ENV PYTHON_VERSION=3.8.2
# Wed, 18 Mar 2020 13:47:29 GMT
ENV PYTHON_RELEASE=3.8.2
# Wed, 18 Mar 2020 13:49:54 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 18 Mar 2020 13:49:56 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 18 Mar 2020 13:49:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 18 Mar 2020 13:49:58 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 18 Mar 2020 13:51:45 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 18 Mar 2020 13:51:45 GMT
CMD ["python"]
# Wed, 18 Mar 2020 15:51:32 GMT
ENV HY_VERSION=0.18.0
# Wed, 18 Mar 2020 15:52:52 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Wed, 18 Mar 2020 15:52:52 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f08cc5bf7287bc1d8f72edfe2439c99210e433230a22fc73264fcf1685850ed2`  
		Last Modified: Fri, 13 Mar 2020 22:09:47 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c4389a998e15eacb1456bae53eda1ae995c217d91d9bc9fd9e8f3d005b8f4d`  
		Last Modified: Wed, 18 Mar 2020 14:03:20 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5f5c7790f76a9b567b08fe42b17c4003e18a70890298dc38d041a9b11790df`  
		Last Modified: Wed, 18 Mar 2020 14:03:19 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf291b339e015d5a7302fd5dc96b5ce783760d8706b46469d5800eb83cb4de85`  
		Last Modified: Wed, 18 Mar 2020 14:04:18 GMT  
		Size: 57.1 MB (57105197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9156968bdc262ad7f40f3e9aee617d5e4b29b5d3942bb629d8fcdf0e3e88814c`  
		Last Modified: Wed, 18 Mar 2020 14:03:17 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6f192e96bfac957591307049c6adbacacc63f4f8db1ef0838893270112906d`  
		Last Modified: Wed, 18 Mar 2020 14:03:17 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b9b09b212daccc4341dce37537741bc21ca501993c4fbc58f070fa8f649ec5`  
		Last Modified: Wed, 18 Mar 2020 14:03:17 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2dfdaa00a45898e6557d4ac77b924e0bba5caf50b9b0fc99418da1f8af0d46`  
		Last Modified: Wed, 18 Mar 2020 14:03:20 GMT  
		Size: 10.4 MB (10406050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1c11c2cbd1417e369ee1641755b852973637bdd9dd6c65b5a36c39ecbac161`  
		Last Modified: Wed, 18 Mar 2020 14:03:17 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e54ecc8019f36dd1e14813a341913f6de77b007b1b738fb9f6400a1e02c8e`  
		Last Modified: Wed, 18 Mar 2020 15:55:21 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094cae2ed55033673a591cf6b8b4f7ae89f85e61d9da815718bf5105d9d19db0`  
		Last Modified: Wed, 18 Mar 2020 15:55:23 GMT  
		Size: 6.2 MB (6157215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024a4b7fbfe28a56e836a3e7675197f78ecb9af35adb61f82a5e3b3689c0aa4d`  
		Last Modified: Wed, 18 Mar 2020 15:55:21 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
