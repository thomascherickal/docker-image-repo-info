## `hylang:0-python3.8-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:a24181e883a5e23359148f690f1a579f3c64eb1fb0987dffb8e93485dfc700a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `hylang:0-python3.8-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull hylang@sha256:18b4551d50f9053306b0249f3f23922d306dc7a81d06c77492cdd1586067691d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826051447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6223cab15f488d94fc69c1821b9c2c754b899425460cef7e8d0fdbec8225fc2`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 30 Oct 2020 00:14:08 GMT
ENV PYTHONIOENCODING=UTF-8
# Fri, 30 Oct 2020 00:27:42 GMT
ENV PYTHON_VERSION=3.8.6
# Fri, 30 Oct 2020 00:27:43 GMT
ENV PYTHON_RELEASE=3.8.6
# Fri, 30 Oct 2020 00:29:52 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Fri, 30 Oct 2020 00:29:53 GMT
ENV PYTHON_PIP_VERSION=20.2.4
# Fri, 30 Oct 2020 00:29:54 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8283828b8fd6f1783daf55a765384e6d8d2c5014/get-pip.py
# Fri, 30 Oct 2020 00:29:55 GMT
ENV PYTHON_GET_PIP_SHA256=2250ab0a7e70f6fd22b955493f7f5cf1ea53e70b584a84a32573644a045b4bfb
# Fri, 30 Oct 2020 00:31:33 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Fri, 30 Oct 2020 00:31:33 GMT
CMD ["python"]
# Fri, 30 Oct 2020 01:09:44 GMT
ENV HY_VERSION=0.19.0
# Fri, 30 Oct 2020 01:11:12 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Fri, 30 Oct 2020 01:11:12 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dc0237500b170e70f7bea25e66289624b0f31aaaa023dcbd4e88ae406fe558`  
		Last Modified: Fri, 30 Oct 2020 00:41:49 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b2d040388ba9a3ca4af11e4ec564b3219847335b26f904f261bbc19a5c08a`  
		Last Modified: Fri, 30 Oct 2020 00:47:00 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a5a0fa51b6928922bfbf79d4a3b6c0794cfc1233a88f81e026e75479cdf099`  
		Last Modified: Fri, 30 Oct 2020 00:46:59 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7c9ae7001ab91895f008ec2f97ef9dcff23db256b43e65fd583a59dfeb7e9`  
		Last Modified: Fri, 30 Oct 2020 00:48:07 GMT  
		Size: 58.5 MB (58548106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6957f0d27eea4446fc21800a2a8f4f7df56b6c33b799fd1e34dc8e9775be3ff`  
		Last Modified: Fri, 30 Oct 2020 00:46:57 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1efb53e2157db820df3a7911fc81daeef0ce0594e6df64de78fdfa1260ef986`  
		Last Modified: Fri, 30 Oct 2020 00:46:57 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd275a9e7a1c6b9783aa6d5f5384628547b8d75120f49a58964232985d26cea`  
		Last Modified: Fri, 30 Oct 2020 00:46:56 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb2cda4e2a1273411b41f6c7318a88a436e11e88daa28e583d81a4eed1456d8`  
		Last Modified: Fri, 30 Oct 2020 00:47:02 GMT  
		Size: 15.4 MB (15449277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc47e3c65f1ab3b848ad24990741d009916b28ffaef14a97f4ab80c01524e11`  
		Last Modified: Fri, 30 Oct 2020 00:46:56 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edad44bae8042f95f9f43efe8b4e385885aa463f05da0f702eacec58b044f944`  
		Last Modified: Fri, 30 Oct 2020 01:14:59 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfe5983c03266f9ac442972d6cafdf15de1af8c68b563c8df9ab1f74320dd87`  
		Last Modified: Fri, 30 Oct 2020 01:15:02 GMT  
		Size: 10.7 MB (10691019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f569ec9525c20d000c6fa05cc048dbd30a0f0e132e6a75f39c31fd7b4dc4092`  
		Last Modified: Fri, 30 Oct 2020 01:14:58 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
