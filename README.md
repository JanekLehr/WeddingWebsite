
This is a compressed-commit version of
[github.com/t413/SinglePaged](https://github.com/t413/SinglePaged)

# [jzwedding.info](http://jzwedding.info)

The source for jzwedding.info

## Get it up and running
Clone the project and `cd WeddingWebsite`

#### Install nginx
`docker run -d -p 80:80 -v /var/run/docker.sock:/tmp/docker.sock -t jwilder/nginx-proxy`

#### Use Jekyll to serve it
`docker run -e VIRTUAL_HOST=jzwedding.info,www.jzwedding.info -d -v "$PWD:/src" -p 4000:4000 --name wedding_website grahamc/jekyll serve -H 0.0.0.0`
