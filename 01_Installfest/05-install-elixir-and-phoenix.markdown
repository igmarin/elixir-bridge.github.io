---
layout: page
title: Install Elixir and Phoenix
date: 2016-09-24 12:28:28 -0700
---


### Step 6: Install Elixir

You can either install elixir with asdf or brew. We recommend asdf, but either approach will be sufficient.

### asdf

For asdf follow the setup instructions here - [https://github.com/asdf-vm/asdf](https://github.com/asdf-vm/asdf)

#### Homebrew

Before installing anything with homebrew, always update to latest,
by typing this in the terminal:

`brew update`

then you can use homebrew to install elixir:

 `brew install elixir`

#### OR Macports

Alternately, you may install using Macports, by typing this in the terminal:

`sudo port install elixir`

#### Windows installation

Navigate to [https://chocolatey.org/install](https://chocolatey.org/install).

Install the chocolatey package.

Then install elixir. Follow the instructions here: [https://chocolatey.org/packages/Elixir](https://chocolatey.org/packages/Elixir)

#### Check Your Installation

To check that Elixir is installed correctly:

`elixir -v`

You should see a version number greater than 1.5, like this:

`Elixir 1.5.1`

Anything above 1.5 is fine.

Mix is a build tool that ships with Elixir, that provides tasks for creating, compiling, testing your application, managing its dependencies, and more.

To check that Mix is also installed correctly:

`mix -v`

You should see a version number greater than 1.5, like this:

`Mix 1.5.1`

### Step 7: Install Hex

Type this in the terminal:

```
mix local.hex
```

### Step 8: Install Phoenix

Type this in the terminal:

```
mix archive.install hex phx_new 1.4.0
```

You will see:

```
Are you sure you want to install archive "https://github.com/phoenixframework/archives/raw/master/phx_new.ez"? [Yn]
```

Answer "Y" to install. Then you should see:

```
* creating /Users/{your user name}/.mix/archives/phx_new
```

#### Verify
Type this in the terminal:
```
mix help | grep phx
```

Expected Result:

```
mix phx.new       # Creates a new Phoenix v1.3.0 application
```

You will likely see other mix commands, but that's the important one.
