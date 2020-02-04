# CUT-workshop
Feb 2020 workshop at CUT in Bloemfontein, South Africa

# Monday
## Software verification with code and models

* [Slides](verif-intro.pdf)

# Tuesday
## Testing Software: From Unit Testing to Model-based Testing

Installation in **Git bash**:

```bash
git clone https://github.com/cyrille-artho/modbat.git
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

### Dining philosophers:

To download and run:

```bash
cd
curl https://cyrille-artho.github.io/CUT-workshop/diningphil.tar.gz -O
tar -xzf diningphil.tar.gz
cd diningphil/src
./build.sh && ./run.sh
```

### Concurrent queue

To download and run:

```bash
cd
curl https://cyrille-artho.github.io/CUT-workshop/queue.tar.gz -O
tar -xzf queue.tar.gz
cd queue/src
./build.sh
./run.sh TestQueue
./run.sh ProdCons
```

### Concurrent queue with a flaw

To download and run:

```bash
cd
curl https://cyrille-artho.github.io/CUT-workshop/queue-notify.tar.gz -O
tar -xzf queue-notify.tar.gz
cd queue-notify/src
./build.sh
./run.sh TestQueue
./run.sh ProdCons
```
