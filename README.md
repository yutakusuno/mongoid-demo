## Description

Demonstration using [MongoDB Atlas](https://www.mongodb.com/atlas) and [Mongoid](https://github.com/mongodb/mongoid). Mongoid is an ODM (Object-Document Mapper) framework for MongoDB in Ruby, and you can make almost the same method calls as Active Record by using it.

## Getting Started

### Tool versions

- ruby 2.7.6
- bundler 2.3.11

See `Gemfile` or `Gemfile.lock` for other dependencies.

### Install

Set a path installing gems.

```
bundle config --local path vendor/bundle
```

Install gems.

```
bundle
```

Install libralies.

```
bin/yarn
```

### Set environmental variable

Create the `.env` file on this project's root path.

```
touch .env
```

And then add an environmental variable like this.

```
ATLAS_URI='mongodb+srv://<username>:<password>@<yourcluster>.mongodb.net/<databasename>?retryWrites=true&w=majority'
```

We have already `dotenv` gem installed and been preparing to load environmental variables, so we just need to add this one.

### Start development

Run the rails server.

```
bin/rails s
```

Open this url.

```
http://localhost:3000/posts
```
