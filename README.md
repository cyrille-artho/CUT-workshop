# CUT-workshop
Feb 2020 workshop at CUT in Bloemfontein, South Africa

# Monday
## Software verification with code and models

* [Slides](verif-intro.pdf)

# Tuesday
## Testing Software: From Unit Testing to Model-based Testing

Installation in **Git bash**:

```bash
git https://github.com/cyrille-artho/modbat.git
cd modbat
./gradlew assemble
cd src/test/scala/modbat/tutorial
```

* [Slides: IoT testing](enase-2019.pdf)
* [Slides: Modbat Tutorial](mbt.pdf)
* [Modbat](https://github.com/cyrille-artho/modbat/)
* [Tutorial](https://github.com/cyrille-artho/modbat/tree/master/src/test/scala/modbat/tutorial)

# Wednesday
## Java Pathfinder

How to configure the environment in the CUT computer labs using **Git bash**:

```bash
mkdir ~/jpf
cd ~/jpf
git clone https://github.com/javapathfinder/jpf-core.git
cd jpf-core
git show 46ae > patch
patch -p1 < patch
./gradlew

export PATH=$PATH:/c/Program\ Files/Java/jdk1.8.0_162/bin
```

* [Slides](jpf-intro-1.pdf)
* [Java Pathfinder](https://github.com/javapathfinder/jpf-core/)
* [Dining philosophers source](diningphil.tar.gz) (.tar.gz)
* [Concurrent queue source](queue.tar.gz) (.tar.gz)
* [Concurrent queue source with flaw](queue-notify.tar.gz) (.tar.gz)
