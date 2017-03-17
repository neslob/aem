
## check current version

  java -version

## list available versions

  /usr/libexec/java_home -V

## install versions

  brew install Caskroom/versions/java8
  brew install Caskroom/versions/java7
  brew install Caskroom/versions/java6

## change version (current shell)

  export JAVA_HOME=$(/usr/libexec/java_home -v 1.8)
  export JAVA_HOME=$(/usr/libexec/java_home -v 1.7)

## permanently (add to .bashrc)

  export JAVA_HOME=$(/usr/libexec/java_home -v 1.7)
