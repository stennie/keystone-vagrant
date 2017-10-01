# Ubuntu 14.04 64-bit Vagrant Box for KeystoneJS

### What is this for?

This box recipe provides a quick start to trying out the [KeystoneJS](http://keystonejs.com/) content management system using a [Vagrant](http://www.vagrantup.com/) 1.1+ development environment.

After successful installation you will have:

 * Ubuntu 14.04 64-bit VM listening on 192.168.192.168 
 * Current version of [Node.js](http://nodejs.org/) (software platform that powers Keystone)
 * Current version of [MongoDB](http://www.mongodb.org/) (NoSQL document-oriented database)
 * All `npm` dependencies for KeystoneJS including [Mongoose](http://mongoosejs.com/) and [Express](http://expressjs.com/).
 * Current version of the [Keystone Yeoman generator](https://www.npmjs.org/package/generator-keystone) (aka 'yo keystone')
 * [Heroku Toolbelt](https://toolbelt.heroku.com/) for deployment

If you would prefer to install the Keystone Generator manually, you can instead follow the documentation on the [`generator-keystone`](https://www.npmjs.org/package/generator-keystone) page on npmjs.org.


### How do you use this box?
1. [Download and install VirtualBox](https://www.virtualbox.org/wiki/Downloads) (tested with 4.3.6)
2. [Download and install Vagrant](http://www.vagrantup.com/downloads.html) - 1.1 or newer required (tested with 1.4.3)
3. Clone this repository
4. `cd keystone-vagrant/`
5. `vagrant up`
6. Grab a cup of coffee while you wait for the server to download and install. This will take a little while depending on your internet connection.
7. Once done `vagrant ssh` and in that folder run `yo keystone`.
8. Answer all of the setup questions and then acces your brand new keystone site at `192.168.192.168:3000`. Login with the default user: `user@keystonejs.com`, pw: `admin`.

### Further Reading
- [Vagrant Documentation](http://docs.vagrantup.com/)
- [Node.js](http://nodejs.org/api/)
- [MongoDB](http://docs.mongodb.org)
- [KeystoneJS](http://keystonejs.com/)

### Credits
 - Based on [node-mongo-vagrant](https://github.com/markdunphy/node-mongo-vagrant) (thanks @markdunphy!)
 - Created for the [Sydney MongoDB User Group](http://www.meetup.com/SydneyMUG/) meetup on 25th Feb, 2014.
