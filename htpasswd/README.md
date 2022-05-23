# user creation instructions



## Create User With Password

- I'm using xmartlabs/htpasswd docker image to use htpasswd to create user:
	```docker run --rm -ti xmartlabs/htpasswd  -Bb omid asadpour | base64```
