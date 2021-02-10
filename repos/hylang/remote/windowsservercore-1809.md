## `hylang:windowsservercore-1809`

```console
$ docker pull hylang@sha256:c5d56590ab31a717c22edbeddc3fd4f6e72e65181c7111c35ba1e32c997c16b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `hylang:windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull hylang@sha256:ccf5015c1ab569218402e2fa0cd2e12c3255a892f02a5ce760858d23f64656e7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2513414665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aff6fd1055e10017e118426f76972bdf13e5b80bcd93075363ba62a5494da839`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 16:07:47 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 10 Feb 2021 16:20:59 GMT
ENV PYTHON_VERSION=3.8.7
# Wed, 10 Feb 2021 16:20:59 GMT
ENV PYTHON_RELEASE=3.8.7
# Wed, 10 Feb 2021 16:22:22 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 16:22:23 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Wed, 10 Feb 2021 16:22:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Wed, 10 Feb 2021 16:22:24 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Wed, 10 Feb 2021 16:23:03 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 10 Feb 2021 16:23:04 GMT
CMD ["python"]
# Wed, 10 Feb 2021 20:12:31 GMT
ENV HY_VERSION=0.20.0
# Wed, 10 Feb 2021 20:13:06 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Wed, 10 Feb 2021 20:13:06 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b84e06535ce9db874df389992b93e0bd5a992e8067ba9fc73059f40ef8966dd`  
		Last Modified: Wed, 10 Feb 2021 16:34:31 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d773d3fabd4894182ab54e230c0b85b35be87af72b77089972ec83d8e507a1a4`  
		Last Modified: Wed, 10 Feb 2021 16:36:19 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffccf0ca1404e7cbaaa9b0155b83d53147df496f989c4847306fa2ce6b2358e`  
		Last Modified: Wed, 10 Feb 2021 16:36:19 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed9660528ba9320e8aa951d220d0393fb4f54c682ba55452a1e59a3bac3f49e`  
		Last Modified: Wed, 10 Feb 2021 16:37:23 GMT  
		Size: 58.3 MB (58339137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c90d010042c9ebd22a1c3552178849676825bb2f8dbe86110d661161a17a69`  
		Last Modified: Wed, 10 Feb 2021 16:36:17 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01468a4a1cda7845e3d07a66e0b026868d7d400fdbb782b4a52721b80926203f`  
		Last Modified: Wed, 10 Feb 2021 16:36:17 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2255237dcfd2ed11ab2dcdb5df687370dfb6826476516835d856dedf3f30db2e`  
		Last Modified: Wed, 10 Feb 2021 16:36:17 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f5105e4ebb45317900f710e68683f159931e4fde56d3248a7d12789b70919b`  
		Last Modified: Wed, 10 Feb 2021 16:36:20 GMT  
		Size: 10.2 MB (10242202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cd50aefd87d91d7be98344e38c5ec2ce638e5a71008fced0a9e844e662fb7d`  
		Last Modified: Wed, 10 Feb 2021 16:36:16 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4077f173080eb1289d117ab330d34deb25076ca7a293841413807fbb31f94d`  
		Last Modified: Wed, 10 Feb 2021 20:14:48 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b875e46965fb2f0fc2c31ae367f42bee22a5638bd539b36b53a6b79091427e1d`  
		Last Modified: Wed, 10 Feb 2021 20:14:55 GMT  
		Size: 5.6 MB (5553004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca634a98c7fa873f67990ec8ff57e5f364f58f9679031980e26e86852edbe4e`  
		Last Modified: Wed, 10 Feb 2021 20:14:48 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
