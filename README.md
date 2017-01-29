# Vagrantfiles
[Vagrantfile](https://www.vagrantup.com/docs/vagrantfile/) for some blank environments.

## Requirement
* >= Vagrant 1.8.x
* >= VirtualBox 5.0.x
* vagrant-vbguest

## Note
The vagrantfiles use `virtualbox` to the [synced folder](https://www.vagrantup.com/docs/synced-folders/).  
The `virtualbox` may need additional configuration such as following.

### Node.js
If you create a node application in `/vagrant` directory, you must use `--no-bin-links` option to `npm install` because the `virtualbox` deny any symbolic links.

And also, the watch feature for monitoring file updates on some applications such as pm2, webpack, browserify must use pooling option for `virtualbox`.

## License
[MIT](https://github.com/ktanakaj/vagrantfiles/blob/master/LICENSE)
