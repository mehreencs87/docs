---
title: Ruby API Tutorial
name: Ruby API
alias:
  - ruby
languages:
  - Ruby
thirdParty: false
image: /media/platforms/rails.png
lodash: true
tags:
  - quickstart
snippets:
  dependencies: server-apis/ruby/dependencies
  setup: server-apis/ruby/setup
  use: server-apis/ruby/use
---

<%= include('../../_includes/_package', {
pkgRepo: 'auth0-rubyonrails-sample', 
githubUrl: 'https://github.com/auth0-samples/auth0-rubyonrails-sample/tree/master/00-Starter-Seed',
pkgBranch: 'master', 
pkgPath: '00-Starter-Seed/ruby-api', 
pkgFilePath: null, 
pkgType: 'server' }) %>

## Ruby API Tutorial

> Note: If you're creating a Ruby On Rails app, please check [this other tutorial](/server-apis/rails).

Otherwise, Please follow the steps below to configure your existing Ruby app to use it with Auth0.

### 1. Add jwt dependency to your Gemfile

You need to add the jwt dependency.

Open your Gemfile and add the following:

${snippet(meta.snippets.dependencies)}

### 2. Validate JWT token

You need to validate the [JWT](/jwt)s to make sure the user is authenticated. For that, in a filter or in a middleware processor that runs before your actions, you should write the following code:

${snippet(meta.snippets.use)}

### 3. You're done!

Now you have both your FrontEnd and Backend configured to use Auth0. Congrats, you're awesome!
