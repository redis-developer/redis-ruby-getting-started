# Getting Started with Ruby and Redis

In order to use Redis with Ruby you will need a Ruby Redis client. 
In the following sections, we will demonstrate the use of redis-rb, a Ruby client library for Redis. 
Additional Ruby clients for Redis can be found under the Ruby section of the Redis Clients page.


## Clone the repository

```
git clone https://github.com/redis-developer/redis-ruby-getting-started
```

##  Install redis-rb:

```
$ gem install redis
```

OR

## Use Gemfile

```$cat Gemfile
gem 'redis'
```


## Execute

```
$ bundle install
```

```
Resolving dependencies...
Using bundler 2.2.6
Using redis 4.2.5
Following files may not be writable, so sudo is needed:
  /Library/Ruby/Gems/2.6.0
  /Library/Ruby/Gems/2.6.0/build_info
  /Library/Ruby/Gems/2.6.0/cache
  /Library/Ruby/Gems/2.6.0/doc
  /Library/Ruby/Gems/2.6.0/extensions
  /Library/Ruby/Gems/2.6.0/gems
  /Library/Ruby/Gems/2.6.0/specifications
Bundle complete! 1 Gemfile dependency, 2 gems now installed.
Use `bundle info [gemname]` to see where a bundled gem is installed.
```

## Verifying 
  
```
bundle info redis
  * redis (4.2.5)
	Summary: A Ruby client library for Redis
	Homepage: https://github.com/redis/redis-rb
	Documentation: https://www.rubydoc.info/gems/redis/4.2.5
	Source Code: https://github.com/redis/redis-rb/tree/v4.2.5
	Changelog: https://github.com/redis/redis-rb/blob/master/CHANGELOG.md
	Bug Tracker: https://github.com/redis/redis-rb/issues
	Path: /Library/Ruby/Gems/2.6.0/gems/redis-4.2.5
```

## Opening a Connection to Redis Using redis-rb

The following code creates a connection to Redis using redis-rb:

```
require 'redis'

redis = Redis.new (
    :host => 'hostname',
    :port => port,
    :password => 'password')
```

To adapt this example to your code, make sure that you replace the following values with those of your database:

In line 4, the

```
:host
```

should be your database’s hostname or IP address

In line 5, the

```
:port
```

should be your database’s port

In line 6, the

```
:password
```

should be your database’s password
