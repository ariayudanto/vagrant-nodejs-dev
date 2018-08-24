# NodeJS, MySQL and Nginx Vangrant Box

Boilerplate Vagrant environment for running NodeJS and MySQL for development. Also proxied through Nginx.

Simply clone the repo and run the following (ensure you have VirtualBox and Vagrant installed):
```
vagrant up
vagrant ssh

```

After ssh to terminal, run the following command

```
vagrant ssh
cd /workspace

```

/workspace is your project folder

To create skeleton project, run the following command
```
express <app_name>
```

Then
```
cd <app_name>
npm install --save
```

Optional, do the following :
- Open app.js file in your app folder then add following line at the end of file

```
app.listen(3000, function () {
  console.log('Example app listening on port 3000!')
})
```

To run you app
```
nodemon -L -q app.js
```