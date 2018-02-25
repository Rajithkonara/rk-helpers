---
layout: default
---
- Base Image

	```FROM node:7-alpine ```

- RUN cmd to execute cmds

	```RUN mkdir -p /src/app```

- Change WorkingDir
	
    ```WORKDIR /src/app```

- NPM install
	
    ```COPY package.json /src/app/package.json   ```
	
    ```RUN 
    npm install```

- Expose ports
	
    ```COPY . /src/app```
	
    ```EXPOSE 3000```
	
    ```CMD [ "npm", "start"]```

- Building and Launching
	Build

	```docker build -t my-nodeapp .```

	Launch

	```docker run -d --name my-running-app -p 3000:3000 my-nodeapp```

- Environment Variables
    env can be defined when you launched a new container 
	
	```docker run -d --name my-production-running-app -e 
		NODE_ENV=production -p 3000:3000 my-nodejs-app ```