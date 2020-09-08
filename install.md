Sometimes, we need to install mulitversions of Java, expecially in Android, which may depend on java8. 

In MacOS, we could use ```brew``` to install java and ```jenv``` to manage running environment.

* Install Java (latest version)

```shell
brew update && brew cask install java
```

* Install Jenv

```shell
brew install https://raw.githubusercontent.com/entrypass/jenv/homebrew/homebrew/jenv.rb
```

* Activate Jenv
```shell
echo 'eval "$(jenv init -)"' >> ~/.bash_profile
```

* Install Java 8

```shell
# jdk8 is not maintained in brew, use adoptopenjdk cask instead
brew tap adoptopenjdk/openjdk
brew cask install adoptopenjdk8
```

* check the installtion env

```shell
ls -1 /Library/Java/JavaVirtualMachines
```

* Add java8

```shell
jenv add /Library/Java/JavaVirtualMachines/adoptopenjdk-8.jdk/Contents/Home/
```

* Some Jenv commands

```
# check jenv
jenv doctor

# check java versions
jenv versions

# change local java version
jenv local xxx

# change global java version
jenv global xxx
```

* Other
