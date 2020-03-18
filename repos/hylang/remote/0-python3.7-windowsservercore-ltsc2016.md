## `hylang:0-python3.7-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:7da9d65473608d14a3a2910794b5564d8bc2d4eb4708d7f0ad89c72bd324c001
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `hylang:0-python3.7-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull hylang@sha256:b329ae32a3905b4505d4674ffeccbbd1f8d9e471ef3e4f4590bb76b215b6e40f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5796847032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb17de23058aa0dc97648eb3b3b16b156068fae02c50621378ec3519fa28b30`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Fri, 13 Mar 2020 21:32:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 13:52:00 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 18 Mar 2020 13:52:01 GMT
ENV PYTHON_RELEASE=3.7.7
# Wed, 18 Mar 2020 13:54:18 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 18 Mar 2020 13:54:19 GMT
ENV PYTHON_PIP_VERSION=20.0.2
# Wed, 18 Mar 2020 13:54:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d59197a3c169cef378a22428a3fa99d33e080a5d/get-pip.py
# Wed, 18 Mar 2020 13:54:22 GMT
ENV PYTHON_GET_PIP_SHA256=421ac1d44c0cf9730a088e337867d974b91bdce4ea2636099275071878cc189e
# Wed, 18 Mar 2020 13:56:06 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 18 Mar 2020 13:56:06 GMT
CMD ["python"]
# Wed, 18 Mar 2020 15:53:05 GMT
ENV HY_VERSION=0.18.0
# Wed, 18 Mar 2020 15:54:28 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Wed, 18 Mar 2020 15:54:30 GMT
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
	-	`sha256:74d02d7e6af53a8eda6ee3b37c25b60e7e1512511144f183f0b84014de884545`  
		Last Modified: Wed, 18 Mar 2020 14:04:37 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46ef4ebb5370a9ed3739468f5b6d6befef898c6789a0efcc43ff1579f3619a4`  
		Last Modified: Wed, 18 Mar 2020 14:04:37 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6b9765b59bc672330f86818a07bed91b2a1dfc21500c489b21260a0755d43e`  
		Last Modified: Wed, 18 Mar 2020 14:04:45 GMT  
		Size: 51.6 MB (51569004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3dbfc83da6d551f84ff49ba9b1c2e885bdacb400a9f8e6c961dff69082a20e`  
		Last Modified: Wed, 18 Mar 2020 14:04:34 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02eda51a12419df5c96ae8dcd6d5154b393689bb80b63f6a9b07b7706b717ebd`  
		Last Modified: Wed, 18 Mar 2020 14:04:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a35106ef9ff634ea824584b15cdf0605e802d1797acc403b50c8f9623d9e356`  
		Last Modified: Wed, 18 Mar 2020 14:04:35 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce73f0bd71f0ff56fa159b1c0f642a41b219b7c3f93737afcd1b8bcc8707de6`  
		Last Modified: Wed, 18 Mar 2020 14:04:41 GMT  
		Size: 10.4 MB (10363782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1293d0a3f95b9d14ecb5d6d13944475c85c763878ca3f51a948d0374adfb566`  
		Last Modified: Wed, 18 Mar 2020 14:04:35 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d29c0b81ca9f6f4b3e432ea976cb7b55d064284ba3e7aecb2485cc3c16a31db`  
		Last Modified: Wed, 18 Mar 2020 15:58:19 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643f2afd7faca18345f979aa9a82d9dc27b6410f93c5885e1aeea1dc5d33959a`  
		Last Modified: Wed, 18 Mar 2020 15:58:20 GMT  
		Size: 6.1 MB (6142954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cedd13bc6abb0328e80fed9d9b165b7f70773aee6bb7ad00be219ef0eb0b3a`  
		Last Modified: Wed, 18 Mar 2020 15:58:19 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
