# Lab Test at Information Theory

View the read-only file by simply clicking it in the list above.


Launch it in a local Jupyter server by clicking [IT_Lab_Test.ipynb](http://192.168.209.78/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Fnikcleju%2FIT_Lab_Test&urlpath=tree%2FIT_Lab_Test%2FIT_Lab_Test.ipynb&branch=master)


Launch on public Binder server by clicking `launch Binder` below:


[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nikcleju/IT_Lab_Test/HEAD?labpath=IT_Lab_Test.ipynb)
 
## Macro definitions

Macro definitions we used during the labs:

```c++

#define READ_BIT(x,i)       (int)(((x) & (1U << (i))) != 0)                                 /* read bit i from x */
#define SET_BIT(x,i)        ((x) = (x) | (1U << (i)))                                       /* set bit i from x to 1 */
#define CLEAR_BIT(x,i)      ((x) = (x) & ~(1U << (i)))                                      /* clear bit i from x to 0 */
#define WRITE_BIT(x,i,val)  ((val) ? SET_BIT((x),(i)) : CLEAR_BIT((x),(i)))                 /* write 'val' in bit i from x */
#define TOGGLE_BIT(x,i)     ((x) = (x) ^ (1U << (i)))                                       /* toggle bit i from x */
#define VECREAD_BIT(v,i)       (READ_BIT((v[(i)/8]),(i)%8))                                 /* read bit i from byte vector v */
#define VECWRITE_BIT(v,i,val)  (WRITE_BIT((v[(i)/8]),((i)%8),val))                          /* write 'val' in bit i from byte vector v */
#define VECTOGGLE_BIT(v,i)  (TOGGLE_BIT((v[(i)/8]),(i)%8))
```

## About

These laboratories use `xeus-cling`, a Jupyter kernel for C++ based on the C++ interpreter [cling](https://github.com/root-project/cling) and
the native implementation of the Jupyter protocol [xeus](https://github.com/jupyter-xeus/xeus).

![xeus-cling](docs/source/xeus-cling.svg)
[![Azure Pipelines](https://dev.azure.com/jupyter-xeus/jupyter-xeus/_apis/build/status/jupyter-xeus.xeus-cling?branchName=master)](https://dev.azure.com/jupyter-xeus/jupyter-xeus/_build/latest?definitionId=4&branchName=master)
[![Appveyor](https://ci.appveyor.com/api/projects/status/qn0wskxlvy52utuv?svg=true)](https://ci.appveyor.com/project/jupyter-xeus/xeus-cling)
[![Documentation Status](http://readthedocs.org/projects/xeus-cling/badge/?version=latest)](https://xeus-cling.readthedocs.io/en/latest/?badge=latest)
[![Binder](https://img.shields.io/badge/launch-binder-brightgreen.svg)](https://mybinder.org/v2/gh/jupyter-xeus/xeus-cling/stable?filepath=notebooks/xcpp.ipynb)
[![Join the Gitter Chat](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/QuantStack/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)


