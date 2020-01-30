<h3 align="center">
  <img src="https://raw.githubusercontent.com/maxhumber/gif/master/logo/gif.png" width="300px" alt="gif">
</h3>
<p align="center">
  <a href="https://github.com/maxhumber/gif"><img alt="GitHub" src="https://img.shields.io/github/license/maxhumber/gif"></a>
  <a href="https://travis-ci.org/maxhumber/gif"><img alt="Travis" src="https://img.shields.io/travis/maxhumber/gif.svg"></a>
  <a href="https://pypi.python.org/pypi/gif"><img alt="PyPI" src="https://img.shields.io/pypi/v/gif.svg"></a>
  <a href="https://pepy.tech/project/gif"><img alt="Downloads" src="https://pepy.tech/badge/gif"></a>
</p>



#### About

`gif` is a better way to build animated Matplotlib gifs.



#### Installation

```
pip install -U gif
```



#### Usage

`gif` is easy to use. Just import:

```
import gif
from matplotlib import pyplot as plt
```

Decorate a Matplotlib plot function with `gif.frame`:

```
@gif.frame
def plot(x, y):
    plt.figure(figsize=(5, 5))
    plt.scatter(x, y)
    plt.xlim((0, 100))
    plt.ylim((0, 100))
```

Build a bunch of "frames" with a standard for loop:

```
from random import randint

frames = []
for _ in range(50):
    x = [randint(0, 100) for _ in range(10)]
    y = [randint(0, 100) for _ in range(10)]
    frame = plot(x, y)
    frames.append(frame)
```

Select the duration (milliseconds) between each frame and save:

```
gif.save(frames, 'random.gif', duration=100)
```



#### Examples

Random ([code](https://github.com/maxhumber/gif/blob/master/examples/random.py)):
<<<<<<< HEAD
![](https://raw.githubusercontent.com/maxhumber/gif/master/examples/random.gif){width=200px}

Preferential Attachment ([code](https://github.com/maxhumber/gif/blob/master/examples/attachment.py), [theory](https://en.wikipedia.org/wiki/Preferential_attachment)):
![](https://raw.githubusercontent.com/maxhumber/gif/master/examples/attachment.gif){width=500px}

Wave ([code](https://github.com/maxhumber/gif/blob/master/examples/sin.py), [original](http://louistiao.me/posts/notebooks/save-matplotlib-animations-as-gifs/)):
![](https://raw.githubusercontent.com/maxhumber/gif/master/examples/sin.gif){width=300px}
=======
<br/>
<img src="https://raw.githubusercontent.com/maxhumber/gif/master/examples/random.gif" width="250px" alt="gif" align='left'>
<br/>
Preferential Attachment ([code](https://github.com/maxhumber/gif/blob/master/examples/attachment.py), [theory](https://en.wikipedia.org/wiki/Preferential_attachment)):
<br/>
<img src="https://raw.githubusercontent.com/maxhumber/gif/master/examples/attachment.gif" width="500px" alt="gif" align='left'>
<br/>
Wave ([code](https://github.com/maxhumber/gif/blob/master/examples/sin.py), [original](http://louistiao.me/posts/notebooks/save-matplotlib-animations-as-gifs/)):
<br/>
<img src="https://raw.githubusercontent.com/maxhumber/gif/master/examples/sin.gif" width="400px" alt="gif" align='left'>
>>>>>>> 13d8a6f940aa016daff02a282b1693f220bff186
