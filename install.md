Sometimes, we need to install mulitversions of Java, expecially in Android, which may depend on java8. 

In MacOS, we could use ```brew``` to install java and ```jenv``` to manage running environment.

* Install Java (latest version)

```shell
# homebrew-cask is an extention to homebrew, which provides wider software, especially UI apps, such as GoogleChrome.
brew update && brew cask install java 
```

* Install [Jenv](https://www.jenv.be/)

```shell
brew install jenv
```

* Activate Jenv
```shell
echo 'eval "$(jenv init -)"' >> ~/.bash_profile # or ~/.zshrc
```

* Install Java 8

```shell
# jdk8 is not maintained in brew, use adoptopenjdk instead
brew tap adoptopenjdk/openjdk # add thirdparty repos
# `brew tap` could show newly added repos
# `brew search openjdk8` could find adoptopenjdk8 package
brew cask install adoptopenjdk8
```

* check the installtion env (for Mac)

```shell
ls -1 /Library/Java/JavaVirtualMachines
```

* Add java8 (for Mac)

```shell
jenv add /Library/Java/JavaVirtualMachines/adoptopenjdk-8.jdk/Contents/Home/
```

* Some Jenv commands

```shell
jenv help
jenv doctor # check jenv
jenv versions # list java versions
jenv remove [version-name] # remove version
jenv local [version-name] # change local java version
jenv global [version-name] # change global java version
```

* Other
