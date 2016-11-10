# Admiral icons

This is an unofficial repository containing product icons for customizing [Admiral's](https://vmware.github.io/admiral/) template and application views.

## How it works?

As described in the [official Admiral documentation](https://github.com/vmware/admiral/wiki/Customization#container-icons):
> For every image search, template definition, container instance or application, Admiral will look up for a resource in `container-images` folder of the defined user resources path based on the image's "namespace/reponame", so for example if you provision a container based on the `vmware/photon:1.0` image, it will lookup for a file `{user-resources-path}/container-icons/vmware/photon.png` and display it if such exists, otherwise it will default to an auto-generated identicon.

Therefore when we provide this set of icons in Admiral's user resources path it will show more friendly product icons of all containers and applications that are based on those images.

## How to use?

You can download the latest contents of this repository as zip by clicking [here](https://github.com/tgeorgiev/admiral-icons/archive/master.zip). Once the zip is downloaded, based on your setup there are 2 options:
1. If running the Admiral Java process, extract the zip to your Admiral user resource folder (configured with the `container.user.resources.path` property, defaults to `/etc/xenon/user-resources/`).
2. If running as container, extract the zip in a folder of your preference and run the Admiral container with:

    `docker run -d -P -v {path-to-extracted-zip}/container-icons/:/etc/xenon/user-resources/container-icons/ vmware/admiral`

## Contributing

Contibutions are welcomed!

If you want to submit a new icon or modify and existing one please fork this repository, make the needed modifications and submit a pull request with the new icon. The icons have to be 64x64 .png files. The source of the icon should also be specified in the list bellow.

## License

All brand icons are trademarks of their respective owners.

Brand icons should only be used to represent the company or product to which they refer.

Icon sources:

* library/alpine.png - <https://twitter.com/alpinelinux>
* library/crate.png - <https://crate.io/>
* library/elasticsearch.png - <https://www.elastic.co/products/elasticsearch>
* library/jenkins.png - <https://wiki.jenkins-ci.org/display/JENKINS/Logo>
* library/mariadb.png - <https://twitter.com/mariadb>
* library/mongodb.png - <http://blog.mongodb.org/>
* library/mysql.png - <https://twitter.com/mysql>
* library/nginx.png - <http://www.myiconfinder.com/icon/nginx-coding-code-programming-website-web-development/1391>
* library/node.png - <https://twitter.com/nodejs>
* library/percona.png - <https://twitter.com/percona>
* library/photon.png - <https://vmware.github.io/photon/>
* library/postgres.png - <https://www.postgresql.org/about/press/presskit95/>
* library/python.png - <https://commons.wikimedia.org/wiki/File:Python-logo-notext.svg>
* library/redis.png - <https://www.iconfinder.com/icons/202809/redis_icon>
* library/rethinkdb.png - <https://mhdzaherghaibeh.name>
* library/ubuntu.png - <http://design.ubuntu.com/downloads?metadata=element-logo+brand-ubuntu>
* library/wordpress.png - <https://wordpress.org/about/logos/>


* kitematic/hello-world-nginx.png - <https://github.com/kitematic>
* kitematic/minecraft.png - <http://www.rw-designer.com/icon-detail/5547>


* vmware/admiral_agent.png - <https://vmware.github.io/admiral/>
* vmware/admiral.png - <https://vmware.github.io/admiral/>
* vmware/photon.png - <https://vmware.github.io/photon/>