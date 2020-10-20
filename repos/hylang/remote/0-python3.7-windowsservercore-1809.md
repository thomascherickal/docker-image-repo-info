## `hylang:0-python3.7-windowsservercore-1809`

```console
$ docker pull hylang@sha256:d58a48f7a041301e68f018d15dea949ad4c2e36a8dc50b708ada128f0a90d75d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `hylang:0-python3.7-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull hylang@sha256:b6eeab89537072a9e632dc16b578dd57db4ac901e26822aa6ba14dc9c2c3b322
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2445715430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c952a78ae8beadd6077ae9e656ff4a819d298301562dddf2b54b29a504f8ec`
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
# Tue, 20 Oct 2020 17:35:01 GMT
ENV PYTHON_PIP_VERSION=20.2.4
# Tue, 20 Oct 2020 17:35:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8283828b8fd6f1783daf55a765384e6d8d2c5014/get-pip.py
# Tue, 20 Oct 2020 17:35:02 GMT
ENV PYTHON_GET_PIP_SHA256=2250ab0a7e70f6fd22b955493f7f5cf1ea53e70b584a84a32573644a045b4bfb
# Tue, 20 Oct 2020 17:35:52 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 20 Oct 2020 17:35:53 GMT
CMD ["python"]
# Tue, 20 Oct 2020 17:59:55 GMT
ENV HY_VERSION=0.19.0
# Tue, 20 Oct 2020 18:00:32 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Tue, 20 Oct 2020 18:00:32 GMT
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
	-	`sha256:68dc07d96898ddb91555cfbe75f49c2bf95073bcca17efe6594c4082b269de64`  
		Last Modified: Tue, 20 Oct 2020 17:39:30 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0abbf7567d7874b32d8e2e9d064f6cb3094bba4de346a61777fe6a5c87d9f8a4`  
		Last Modified: Tue, 20 Oct 2020 17:39:29 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50a64e130c85752d71df235efabd63116b0fc7f4a0f411af9c97af629dc3f2d`  
		Last Modified: Tue, 20 Oct 2020 17:39:29 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e781b7deb0fb3e91d57386d3290b4d85e9dd99d0ede7ceb32a398420ddec61f4`  
		Last Modified: Tue, 20 Oct 2020 17:39:33 GMT  
		Size: 10.3 MB (10250847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f140be7ed6f689c4b2450cdcfc2ffd89dc805eddff370af7ac59d9d14eb87cad`  
		Last Modified: Tue, 20 Oct 2020 17:39:29 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c067563b9e66175529e45eb79897da2f8ae12c6cf8b820bac35abd15b7e5b6b`  
		Last Modified: Tue, 20 Oct 2020 18:05:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79547ba2aa713d516d8091707434207c9f0986bfe992c55393dd7128a77f844`  
		Last Modified: Tue, 20 Oct 2020 18:05:11 GMT  
		Size: 5.5 MB (5528956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bdafcb9e21ab02d305973d422e7a8f2b24840b3427d4ce994be01ff03d0045`  
		Last Modified: Tue, 20 Oct 2020 18:05:05 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
