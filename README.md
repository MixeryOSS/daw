# Mixery
_Free n' open source digital audio workspace for the web_

This is Mixery standard configuration, which can be built by using [Mixery CLI tool][CLI].

## Building Mixery
You can build Mixery by using the CLI tool:

```sh
git clone https://github.com/MixeryOSS/daw
cd daw
mixerycli build
```

## Host your Mixery build
Since Mixery doesn't require a backing server when using, you can easily deploy Mixery on static web services. Most web services allows you to host static webpages for as little as US$0.02 per month. On GitHub, it's free for all open source projects, like this one.

```sh
# Copy only necessary files
mkdir www
cp build/bundle.js www/
cp build/index.html www/
cp -r build/addons/ www/

# Run static web server
cd www
http-server
```

[CLI]: https://github.com/MixeryOSS/cli