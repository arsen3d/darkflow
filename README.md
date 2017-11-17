```
imac5k2015:test arsen$ git clone https://github.com/arsen3d/darkflow
Cloning into 'darkflow'...
remote: Counting objects: 2558, done.
remote: Total 2558 (delta 0), reused 0 (delta 0), pack-reused 2558
Receiving objects: 100% (2558/2558), 18.69 MiB | 5.72 MiB/s, done.
Resolving deltas: 100% (1719/1719), done.
imac5k2015:test arsen$ cd darkflow/
imac5k2015:darkflow arsen$ LS
LICENSE		README.md	cfg		darkflow	flow		labels.txt	preview.png	sample_img	setup.py	test
imac5k2015:darkflow arsen$ python3 setup.py build_ext --inplace
Compiling darkflow/cython_utils/nms.pyx because it changed.
Compiling darkflow/cython_utils/cy_yolo2_findboxes.pyx because it changed.
Compiling darkflow/cython_utils/cy_yolo_findboxes.pyx because it changed.
[1/3] Cythonizing darkflow/cython_utils/cy_yolo2_findboxes.pyx
[2/3] Cythonizing darkflow/cython_utils/cy_yolo_findboxes.pyx
[3/3] Cythonizing darkflow/cython_utils/nms.pyx
running build_ext
building 'darkflow.cython_utils.nms' extension
creating build
creating build/temp.macosx-10.6-intel-3.6
creating build/temp.macosx-10.6-intel-3.6/darkflow
creating build/temp.macosx-10.6-intel-3.6/darkflow/cython_utils
/usr/bin/clang -fno-strict-aliasing -Wsign-compare -fno-common -dynamic -DNDEBUG -g -fwrapv -O3 -Wall -Wstrict-prototypes -arch i386 -arch x86_64 -g -I/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include -I/Library/Frameworks/Python.framework/Versions/3.6/include/python3.6m -c darkflow/cython_utils/nms.c -o build/temp.macosx-10.6-intel-3.6/darkflow/cython_utils/nms.o
In file included from darkflow/cython_utils/nms.c:547:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/arrayobject.h:4:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/ndarrayobject.h:18:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/ndarraytypes.h:1809:
/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h:15:2: warning: "Using deprecated NumPy API, disable it by "
      "#defining NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION" [-W#warnings]
#warning "Using deprecated NumPy API, disable it by " \
 ^
1 warning generated.
In file included from darkflow/cython_utils/nms.c:547:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/arrayobject.h:4:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/ndarrayobject.h:18:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/ndarraytypes.h:1809:
/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h:15:2: warning: "Using deprecated NumPy API, disable it by "
      "#defining NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION" [-W#warnings]
#warning "Using deprecated NumPy API, disable it by " \
 ^
1 warning generated.
creating build/lib.macosx-10.6-intel-3.6
creating build/lib.macosx-10.6-intel-3.6/darkflow
creating build/lib.macosx-10.6-intel-3.6/darkflow/cython_utils
/usr/bin/clang -bundle -undefined dynamic_lookup -arch i386 -arch x86_64 -g build/temp.macosx-10.6-intel-3.6/darkflow/cython_utils/nms.o -lm -o build/lib.macosx-10.6-intel-3.6/darkflow/cython_utils/nms.cpython-36m-darwin.so
building 'darkflow.cython_utils.cy_yolo2_findboxes' extension
/usr/bin/clang -fno-strict-aliasing -Wsign-compare -fno-common -dynamic -DNDEBUG -g -fwrapv -O3 -Wall -Wstrict-prototypes -arch i386 -arch x86_64 -g -I/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include -I/Library/Frameworks/Python.framework/Versions/3.6/include/python3.6m -c darkflow/cython_utils/cy_yolo2_findboxes.c -o build/temp.macosx-10.6-intel-3.6/darkflow/cython_utils/cy_yolo2_findboxes.o
In file included from darkflow/cython_utils/cy_yolo2_findboxes.c:547:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/arrayobject.h:4:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/ndarrayobject.h:18:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/ndarraytypes.h:1809:
/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h:15:2: warning: "Using deprecated NumPy API, disable it by "
      "#defining NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION" [-W#warnings]
#warning "Using deprecated NumPy API, disable it by " \
 ^
1 warning generated.
In file included from darkflow/cython_utils/cy_yolo2_findboxes.c:547:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/arrayobject.h:4:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/ndarrayobject.h:18:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/ndarraytypes.h:1809:
/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h:15:2: warning: "Using deprecated NumPy API, disable it by "
      "#defining NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION" [-W#warnings]
#warning "Using deprecated NumPy API, disable it by " \
 ^
1 warning generated.
/usr/bin/clang -bundle -undefined dynamic_lookup -arch i386 -arch x86_64 -g build/temp.macosx-10.6-intel-3.6/darkflow/cython_utils/cy_yolo2_findboxes.o -lm -o build/lib.macosx-10.6-intel-3.6/darkflow/cython_utils/cy_yolo2_findboxes.cpython-36m-darwin.so
building 'darkflow.cython_utils.cy_yolo_findboxes' extension
/usr/bin/clang -fno-strict-aliasing -Wsign-compare -fno-common -dynamic -DNDEBUG -g -fwrapv -O3 -Wall -Wstrict-prototypes -arch i386 -arch x86_64 -g -I/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include -I/Library/Frameworks/Python.framework/Versions/3.6/include/python3.6m -c darkflow/cython_utils/cy_yolo_findboxes.c -o build/temp.macosx-10.6-intel-3.6/darkflow/cython_utils/cy_yolo_findboxes.o
In file included from darkflow/cython_utils/cy_yolo_findboxes.c:547:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/arrayobject.h:4:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/ndarrayobject.h:18:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/ndarraytypes.h:1809:
/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h:15:2: warning: "Using deprecated NumPy API, disable it by "
      "#defining NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION" [-W#warnings]
#warning "Using deprecated NumPy API, disable it by " \
 ^
1 warning generated.
In file included from darkflow/cython_utils/cy_yolo_findboxes.c:547:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/arrayobject.h:4:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/ndarrayobject.h:18:
In file included from /Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/ndarraytypes.h:1809:
/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h:15:2: warning: "Using deprecated NumPy API, disable it by "
      "#defining NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION" [-W#warnings]
#warning "Using deprecated NumPy API, disable it by " \
 ^
1 warning generated.
/usr/bin/clang -bundle -undefined dynamic_lookup -arch i386 -arch x86_64 -g build/temp.macosx-10.6-intel-3.6/darkflow/cython_utils/cy_yolo_findboxes.o -lm -o build/lib.macosx-10.6-intel-3.6/darkflow/cython_utils/cy_yolo_findboxes.cpython-36m-darwin.so
copying build/lib.macosx-10.6-intel-3.6/darkflow/cython_utils/nms.cpython-36m-darwin.so -> darkflow/cython_utils
copying build/lib.macosx-10.6-intel-3.6/darkflow/cython_utils/cy_yolo2_findboxes.cpython-36m-darwin.so -> darkflow/cython_utils
copying build/lib.macosx-10.6-intel-3.6/darkflow/cython_utils/cy_yolo_findboxes.cpython-36m-darwin.so -> darkflow/cython_utils
imac5k2015:darkflow arsen$ pip install -e .
Obtaining file:///Users/arsen/test/darkflow
Installing collected packages: darkflow
  Found existing installation: darkflow 1.0.0
    Uninstalling darkflow-1.0.0:
      Successfully uninstalled darkflow-1.0.0
  Running setup.py develop for darkflow
Successfully installed darkflow
imac5k2015:darkflow arsen$ pip install .
Processing /Users/arsen/test/darkflow
  Requirement already satisfied (use --upgrade to upgrade): darkflow==1.0.0 from file:///Users/arsen/test/darkflow in /Users/arsen/test/darkflow
imac5k2015:darkflow arsen$ flow --h
/Users/arsen/anaconda3/lib/python3.6/importlib/_bootstrap.py:219: RuntimeWarning: compiletime version 3.5 of module 'tensorflow.python.framework.fast_tensor_util' does not match runtime version 3.6
  return f(*args, **kwds)

Example usage: flow --imgdir sample_img/ --model cfg/yolo.cfg --load bin/yolo.weights

Arguments:
  --help, --h, -h  show this super helpful message and exit
  --imgdir         path to testing directory with images
  --binary         path to .weights directory
  --config         path to .cfg directory
  --dataset        path to dataset directory
  --labels         path to labels file
  --backup         path to backup folder
  --summary        path to TensorBoard summaries directory
  --annotation     path to annotation directory
  --threshold      detection threshold
  --model          configuration of choice
  --trainer        training algorithm
  --momentum       applicable for rmsprop and momentum optimizers
  --verbalise      say out loud while building graph
  --train          train the whole net
  --load           how to initialize the net? Either from .weights or a checkpoint, or even from scratch
  --savepb         save net and weight to a .pb file
  --gpu            how much gpu (from 0.0 to 1.0)
  --gpuName        GPU device name
  --lr             learning rate
  --keep           Number of most recent training results to save
  --batch          batch size
  --epoch          number of epoch
  --save           save checkpoint every ? training examples
  --demo           demo on webcam
  --queue          process demo in batch
  --json           Outputs bounding box information in json format.
  --saveVideo      Records video from input video or camera
  --pbLoad         path to .pb protobuf file (metaLoad must also be specified)
  --metaLoad       path to .meta file generated during --savepb that corresponds to .pb file

imac5k2015:darkflow arsen$ open .
imac5k2015:darkflow arsen$ flow --model cfg/yolo-new.cfg --load bin/yolo-new.weights --demo videofile.avi
/Users/arsen/anaconda3/lib/python3.6/importlib/_bootstrap.py:219: RuntimeWarning: compiletime version 3.5 of module 'tensorflow.python.framework.fast_tensor_util' does not match runtime version 3.6
  return f(*args, **kwds)

Traceback (most recent call last):
  File "/Users/arsen/anaconda3/bin/flow", line 6, in <module>
    exec(compile(open(__file__).read(), __file__, 'exec'))
  File "/Users/arsen/test/darkflow/flow", line 6, in <module>
    cliHandler(sys.argv)
  File "/Users/arsen/test/darkflow/darkflow/cli.py", line 22, in cliHandler
    tfnet = TFNet(FLAGS)
  File "/Users/arsen/test/darkflow/darkflow/net/build.py", line 58, in __init__
    darknet = Darknet(FLAGS)
  File "/Users/arsen/test/darkflow/darkflow/dark/darknet.py", line 13, in __init__
    self.get_weight_src(FLAGS)
  File "/Users/arsen/test/darkflow/darkflow/dark/darknet.py", line 47, in get_weight_src
    '{} not found'.format(FLAGS.load)
AssertionError: bin/yolo-new.weights not found
imac5k2015:darkflow arsen$ flow --model cfg/yolo-new.cfg --load bin/yolo-new.weights --demo video.mp4
/Users/arsen/anaconda3/lib/python3.6/importlib/_bootstrap.py:219: RuntimeWarning: compiletime version 3.5 of module 'tensorflow.python.framework.fast_tensor_util' does not match runtime version 3.6
  return f(*args, **kwds)

/Users/arsen/test/darkflow/darkflow/dark/darknet.py:54: UserWarning: ./cfg/yolo-new.cfg not found, use cfg/yolo-new.cfg instead
  cfg_path, FLAGS.model))
Parsing cfg/yolo-new.cfg
Traceback (most recent call last):
  File "/Users/arsen/anaconda3/bin/flow", line 6, in <module>
    exec(compile(open(__file__).read(), __file__, 'exec'))
  File "/Users/arsen/test/darkflow/flow", line 6, in <module>
    cliHandler(sys.argv)
  File "/Users/arsen/test/darkflow/darkflow/cli.py", line 22, in cliHandler
    tfnet = TFNet(FLAGS)
  File "/Users/arsen/test/darkflow/darkflow/net/build.py", line 58, in __init__
    darknet = Darknet(FLAGS)
  File "/Users/arsen/test/darkflow/darkflow/dark/darknet.py", line 17, in __init__
    src_parsed = self.parse_cfg(self.src_cfg, FLAGS)
  File "/Users/arsen/test/darkflow/darkflow/dark/darknet.py", line 68, in parse_cfg
    for i, info in enumerate(cfg_layers):
  File "/Users/arsen/test/darkflow/darkflow/utils/process.py", line 66, in cfg_yielder
    layers, meta = parser(model); yield meta;
  File "/Users/arsen/test/darkflow/darkflow/utils/process.py", line 17, in parser
    with open(model, 'rb') as f:
FileNotFoundError: [Errno 2] No such file or directory: 'cfg/yolo-new.cfg'
imac5k2015:darkflow arsen$ flow --model cfg/yolo-new.cfg --load bin/yolo-new.weights --demo video.mp4
/Users/arsen/anaconda3/lib/python3.6/importlib/_bootstrap.py:219: RuntimeWarning: compiletime version 3.5 of module 'tensorflow.python.framework.fast_tensor_util' does not match runtime version 3.6
  return f(*args, **kwds)

Parsing ./cfg/yolo-new.cfg
Layer "button" aria-label not implemented
imac5k2015:darkflow arsen$ flow --model cfg/arsen-yolo.cfg --load bin/yolo-new.weights --demo video.mp4
/Users/arsen/anaconda3/lib/python3.6/importlib/_bootstrap.py:219: RuntimeWarning: compiletime version 3.5 of module 'tensorflow.python.framework.fast_tensor_util' does not match runtime version 3.6
  return f(*args, **kwds)

Parsing ./cfg/yolo-new.cfg
Layer "button" aria-label not implemented
imac5k2015:darkflow arsen$ flow --model cfg/arsen-tiny-yolo-voc.cfg --load bin/arsen-tiny-yolo-voc.weights --demo video.mp4
/Users/arsen/anaconda3/lib/python3.6/importlib/_bootstrap.py:219: RuntimeWarning: compiletime version 3.5 of module 'tensorflow.python.framework.fast_tensor_util' does not match runtime version 3.6
  return f(*args, **kwds)

Parsing ./cfg/arsen-tiny-yolo-voc.cfg
Parsing cfg/arsen-tiny-yolo-voc.cfg
Loading bin/arsen-tiny-yolo-voc.weights ...
Successfully identified 63471556 bytes
Finished in 1.8384089469909668s
Traceback (most recent call last):
  File "/Users/arsen/anaconda3/bin/flow", line 6, in <module>
    exec(compile(open(__file__).read(), __file__, 'exec'))
  File "/Users/arsen/test/darkflow/flow", line 6, in <module>
    cliHandler(sys.argv)
  File "/Users/arsen/test/darkflow/darkflow/cli.py", line 22, in cliHandler
    tfnet = TFNet(FLAGS)
  File "/Users/arsen/test/darkflow/darkflow/net/build.py", line 64, in __init__
    self.framework = create_framework(*args)
  File "/Users/arsen/test/darkflow/darkflow/net/framework.py", line 59, in create_framework
    return this(meta, FLAGS)
  File "/Users/arsen/test/darkflow/darkflow/net/framework.py", line 15, in __init__
    self.constructor(meta, FLAGS)
  File "/Users/arsen/test/darkflow/darkflow/net/yolo/__init__.py", line 24, in constructor
    ).format(meta['model'])
AssertionError: labels.txt and cfg/arsen-tiny-yolo-voc.cfg indicate inconsistent class numbers
imac5k2015:darkflow arsen$ flow --model cfg/arsen-tiny-yolo-voc.cfg --load bin/arsen-tiny-yolo-voc.weights --demo video.mp4
imac5k2015:darkflow arsen$ wget https://pjreddie.com/media/files/yolo.weights
-bash: wget: command not found
imac5k2015:darkflow arsen$ wget https://pjreddie.com/media/files/yolo.weights
imac5k2015:darkflow arsen$ brew wget
brewError: Unknown command: wget
imac5k2015:darkflow arsen$ brew install wget
Updating Homebrew...
==> Auto-updated Homebrew!
Updated 1 tap (caskroom/cask).
No changes to formulae.

==> Installing dependencies for wget: openssl@1.1
==> Installing wget dependency: openssl@1.1
==> Downloading https://homebrew.bintray.com/bottles/openssl@1.1-1.1.0g.high_sierra.bottle.tar.gz
######################################################################## 100.0%
==> Pouring openssl@1.1-1.1.0g.high_sierra.bottle.tar.gz
==> Caveats
A CA file has been bootstrapped using certificates from the system
keychain. To add additional certificates, place .pem files in
  /usr/local/etc/openssl@1.1/certs

and run
  /usr/local/opt/openssl@1.1/bin/c_rehash

This formula is keg-only, which means it was not symlinked into /usr/local,
because this is an alternate version of another formula.

If you need to have this software first in your PATH run:
  echo 'export PATH="/usr/local/opt/openssl@1.1/bin:$PATH"' >> ~/.bash_profile

For compilers to find this software you may need to set:
    LDFLAGS:  -L/usr/local/opt/openssl@1.1/lib
    CPPFLAGS: -I/usr/local/opt/openssl@1.1/include
For pkg-config to find this software you may need to set:
    PKG_CONFIG_PATH: /usr/local/opt/openssl@1.1/lib/pkgconfig

==> Summary
🍺  /usr/local/Cellar/openssl@1.1/1.1.0g: 6,585 files, 15.6MB
==> Installing wget
==> Downloading https://homebrew.bintray.com/bottles/wget-1.19.2.high_sierra.bottle.tar.gz
######################################################################## 100.0%
==> Pouring wget-1.19.2.high_sierra.bottle.tar.gz
🍺  /usr/local/Cellar/wget/1.19.2: 11 files, 1.7MB
imac5k2015:darkflow arsen$ wget https://pjreddie.com/media/files/yolo.weights
--2017-11-16 22:59:44--  https://pjreddie.com/media/files/yolo.weights
Resolving pjreddie.com... 128.208.3.39
Connecting to pjreddie.com|128.208.3.39|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 203934260 (194M) [application/octet-stream]
Saving to: 'yolo.weights'

yolo.weights                                    100%[====================================================================================================>] 194.49M  6.26MB/s    in 27s     

2017-11-16 23:00:11 (7.13 MB/s) - 'yolo.weights' saved [203934260/203934260]

imac5k2015:darkflow arsen$ flow --model cfg/arsen-yolo.cfg --load yolo.weights --demo video.mp4
/Users/arsen/anaconda3/lib/python3.6/importlib/_bootstrap.py:219: RuntimeWarning: compiletime version 3.5 of module 'tensorflow.python.framework.fast_tensor_util' does not match runtime version 3.6
  return f(*args, **kwds)

Parsing ./cfg/yolo.cfg
Parsing cfg/arsen-yolo.cfg
Loading yolo.weights ...
Successfully identified 203934260 bytes
Finished in 3.713236093521118s
Traceback (most recent call last):
  File "/Users/arsen/anaconda3/bin/flow", line 6, in <module>
    exec(compile(open(__file__).read(), __file__, 'exec'))
  File "/Users/arsen/test/darkflow/flow", line 6, in <module>
    cliHandler(sys.argv)
  File "/Users/arsen/test/darkflow/darkflow/cli.py", line 22, in cliHandler
    tfnet = TFNet(FLAGS)
  File "/Users/arsen/test/darkflow/darkflow/net/build.py", line 64, in __init__
    self.framework = create_framework(*args)
  File "/Users/arsen/test/darkflow/darkflow/net/framework.py", line 59, in create_framework
    return this(meta, FLAGS)
  File "/Users/arsen/test/darkflow/darkflow/net/framework.py", line 15, in __init__
    self.constructor(meta, FLAGS)
  File "/Users/arsen/test/darkflow/darkflow/net/yolo/__init__.py", line 24, in constructor
    ).format(meta['model'])
AssertionError: labels.txt and cfg/arsen-yolo.cfg indicate inconsistent class numbers
imac5k2015:darkflow arsen$ flow --model cfg/yolo.cfg --load yolo.weights --demo video.mp4
/Users/arsen/anaconda3/lib/python3.6/importlib/_bootstrap.py:219: RuntimeWarning: compiletime version 3.5 of module 'tensorflow.python.framework.fast_tensor_util' does not match runtime version 3.6
  return f(*args, **kwds)

Parsing ./cfg/yolo.cfg
Parsing cfg/yolo.cfg
Loading yolo.weights ...
Successfully identified 203934260 bytes
Finished in 3.6040267944335938s
Model has a coco model name, loading coco labels.

Building net ...
Source | Train? | Layer description                | Output size
-------+--------+----------------------------------+---------------
       |        | input                            | (?, 608, 608, 3)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 608, 608, 32)
 Load  |  Yep!  | maxp 2x2p0_2                     | (?, 304, 304, 32)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 304, 304, 64)
 Load  |  Yep!  | maxp 2x2p0_2                     | (?, 152, 152, 64)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 152, 152, 128)
 Load  |  Yep!  | conv 1x1p0_1  +bnorm  leaky      | (?, 152, 152, 64)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 152, 152, 128)
 Load  |  Yep!  | maxp 2x2p0_2                     | (?, 76, 76, 128)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 76, 76, 256)
 Load  |  Yep!  | conv 1x1p0_1  +bnorm  leaky      | (?, 76, 76, 128)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 76, 76, 256)
 Load  |  Yep!  | maxp 2x2p0_2                     | (?, 38, 38, 256)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 38, 38, 512)
 Load  |  Yep!  | conv 1x1p0_1  +bnorm  leaky      | (?, 38, 38, 256)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 38, 38, 512)
 Load  |  Yep!  | conv 1x1p0_1  +bnorm  leaky      | (?, 38, 38, 256)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 38, 38, 512)
 Load  |  Yep!  | maxp 2x2p0_2                     | (?, 19, 19, 512)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 19, 19, 1024)
 Load  |  Yep!  | conv 1x1p0_1  +bnorm  leaky      | (?, 19, 19, 512)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 19, 19, 1024)
 Load  |  Yep!  | conv 1x1p0_1  +bnorm  leaky      | (?, 19, 19, 512)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 19, 19, 1024)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 19, 19, 1024)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 19, 19, 1024)
 Load  |  Yep!  | concat [16]                      | (?, 38, 38, 512)
 Load  |  Yep!  | conv 1x1p0_1  +bnorm  leaky      | (?, 38, 38, 64)
 Load  |  Yep!  | local flatten 2x2                | (?, 19, 19, 256)
 Load  |  Yep!  | concat [27, 24]                  | (?, 19, 19, 1280)
 Load  |  Yep!  | conv 3x3p1_1  +bnorm  leaky      | (?, 19, 19, 1024)
 Load  |  Yep!  | conv 1x1p0_1    linear           | (?, 19, 19, 425)
-------+--------+----------------------------------+---------------
Running entirely on CPU
2017-11-16 23:00:58.418427: I tensorflow/core/platform/cpu_feature_guard.cc:137] Your CPU supports instructions that this TensorFlow binary was not compiled to use: SSE4.1 SSE4.2 AVX AVX2 FMA
Finished in 9.086707830429077s

GVA info: Successfully connected to the Intel plugin, offline Gen75 
Press [ESC] to quit demo
0.884 FPS^[^[^[^[

```


## Intro

[![Build Status](https://travis-ci.org/thtrieu/darkflow.svg?branch=master)](https://travis-ci.org/thtrieu/darkflow) [![codecov](https://codecov.io/gh/thtrieu/darkflow/branch/master/graph/badge.svg)](https://codecov.io/gh/thtrieu/darkflow)

Real-time object detection and classification. Paper: [version 1](https://arxiv.org/pdf/1506.02640.pdf), [version 2](https://arxiv.org/pdf/1612.08242.pdf).

Read more about YOLO (in darknet) and download weight files [here](http://pjreddie.com/darknet/yolo/). In case the weight file cannot be found, I uploaded some of mine [here](https://drive.google.com/drive/folders/0B1tW_VtY7onidEwyQ2FtQVplWEU), which include `yolo-full` and `yolo-tiny` of v1.0, `tiny-yolo-v1.1` of v1.1 and `yolo`, `tiny-yolo-voc` of v2.


Click on this image to see demo from yolov2:

[![img](preview.png)](http://i.imgur.com/EyZZKAA.gif)

## Dependencies

Python3, tensorflow 1.0, numpy, opencv 3.

### Getting started

You can choose _one_ of the following three ways to get started with darkflow.

1. Just build the Cython extensions in place. NOTE: If installing this way you will have to use `./flow` in the cloned darkflow directory instead of `flow` as darkflow is not installed globally.
    ```
    python3 setup.py build_ext --inplace
    ```

2. Let pip install darkflow globally in dev mode (still globally accessible, but changes to the code immediately take effect)
    ```
    pip install -e .
    ```

3. Install with pip globally
    ```
    pip install .
    ```

## Update

**Android demo on Tensorflow's** [here](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/examples/android/src/org/tensorflow/demo/TensorFlowYoloDetector.java)

**I am looking for help:**
 - `help wanted` labels in issue track

## Parsing the annotations

Skip this if you are not training or fine-tuning anything (you simply want to forward flow a trained net)

For example, if you want to work with only 3 classes `tvmonitor`, `person`, `pottedplant`; edit `labels.txt` as follows

```
tvmonitor
person
pottedplant
```

And that's it. `darkflow` will take care of the rest. You can also set darkflow to load from a custom labels file with the `--labels` flag (i.e. `--labels myOtherLabelsFile.txt`). This can be helpful when working with multiple models with different sets of output labels. When this flag is not set, darkflow will load from `labels.txt` by default (unless you are using one of the recognized `.cfg` files designed for the COCO or VOC dataset - then the labels file will be ignored and the COCO or VOC labels will be loaded).

## Design the net

Skip this if you are working with one of the original configurations since they are already there. Otherwise, see the following example:

```python
...

[convolutional]
batch_normalize = 1
size = 3
stride = 1
pad = 1
activation = leaky

[maxpool]

[connected]
output = 4096
activation = linear

...
```

## Flowing the graph using `flow`

```bash
# Have a look at its options
flow --h
```

First, let's take a closer look at one of a very useful option `--load`

```bash
# 1. Load yolo-tiny.weights
flow --model cfg/yolo-tiny.cfg --load bin/yolo-tiny.weights

# 2. To completely initialize a model, leave the --load option
flow --model cfg/yolo-new.cfg

# 3. It is useful to reuse the first identical layers of tiny for `yolo-new`
flow --model cfg/yolo-new.cfg --load bin/yolo-tiny.weights
# this will print out which layers are reused, which are initialized
```

All input images from default folder `sample_img/` are flowed through the net and predictions are put in `sample_img/out/`. We can always specify more parameters for such forward passes, such as detection threshold, batch size, images folder, etc.

```bash
# Forward all images in sample_img/ using tiny yolo and 100% GPU usage
flow --imgdir sample_img/ --model cfg/yolo-tiny.cfg --load bin/yolo-tiny.weights --gpu 1.0
```
json output can be generated with descriptions of the pixel location of each bounding box and the pixel location. Each prediction is stored in the `sample_img/out` folder by default. An example json array is shown below.
```bash
# Forward all images in sample_img/ using tiny yolo and JSON output.
flow --imgdir sample_img/ --model cfg/yolo-tiny.cfg --load bin/yolo-tiny.weights --json
```
JSON output:
```json
[{"label":"person", "confidence": 0.56, "topleft": {"x": 184, "y": 101}, "bottomright": {"x": 274, "y": 382}},
{"label": "dog", "confidence": 0.32, "topleft": {"x": 71, "y": 263}, "bottomright": {"x": 193, "y": 353}},
{"label": "horse", "confidence": 0.76, "topleft": {"x": 412, "y": 109}, "bottomright": {"x": 592,"y": 337}}]
```
 - label: self explanatory
 - confidence: somewhere between 0 and 1 (how confident yolo is about that detection)
 - topleft: pixel coordinate of top left corner of box.
 - bottomright: pixel coordinate of bottom right corner of box.

## Training new model

Training is simple as you only have to add option `--train`. Training set and annotation will be parsed if this is the first time a new configuration is trained. To point to training set and annotations, use option `--dataset` and `--annotation`. A few examples:

```bash
# Initialize yolo-new from yolo-tiny, then train the net on 100% GPU:
flow --model cfg/yolo-new.cfg --load bin/yolo-tiny.weights --train --gpu 1.0

# Completely initialize yolo-new and train it with ADAM optimizer
flow --model cfg/yolo-new.cfg --train --trainer adam
```

During training, the script will occasionally save intermediate results into Tensorflow checkpoints, stored in `ckpt/`. To resume to any checkpoint before performing training/testing, use `--load [checkpoint_num]` option, if `checkpoint_num < 0`, `darkflow` will load the most recent save by parsing `ckpt/checkpoint`.

```bash
# Resume the most recent checkpoint for training
flow --train --model cfg/yolo-new.cfg --load -1

# Test with checkpoint at step 1500
flow --model cfg/yolo-new.cfg --load 1500

# Fine tuning yolo-tiny from the original one
flow --train --model cfg/yolo-tiny.cfg --load bin/yolo-tiny.weights
```

Example of training on Pascal VOC 2007:
```bash
# Download the Pascal VOC dataset:
curl -O https://pjreddie.com/media/files/VOCtest_06-Nov-2007.tar
tar xf VOCtest_06-Nov-2007.tar

# An example of the Pascal VOC annotation format:
vim VOCdevkit/VOC2007/Annotations/000001.xml

# Train the net on the Pascal dataset:
flow --model cfg/yolo-new.cfg --train --dataset "~/VOCdevkit/VOC2007/JPEGImages" --annotation "~/VOCdevkit/VOC2007/Annotations"
```

### Training on your own dataset

*The steps below assume we want to use tiny YOLO and our dataset has 3 classes*

1. Create a copy of the configuration file `tiny-yolo-voc.cfg` and rename it according to your preference `tiny-yolo-voc-3c.cfg` (It is crucial that you leave the original `tiny-yolo-voc.cfg` file unchanged, see below for explanation).

2. In `tiny-yolo-voc-3c.cfg`, change classes in the [region] layer (the last layer) to the number of classes you are going to train for. In our case, classes are set to 3.
    
    ```python
    ...

    [region]
    anchors = 1.08,1.19,  3.42,4.41,  6.63,11.38,  9.42,5.11,  16.62,10.52
    bias_match=1
    classes=3
    coords=4
    num=5
    softmax=1
    
    ...
    ```

3. In `tiny-yolo-voc-3c.cfg`, change filters in the [convolutional] layer (the second to last layer) to num * (classes + 5). In our case, num is 5 and classes are 3 so 5 * (3 + 5) = 40 therefore filters are set to 40.
    
    ```python
    ...

    [convolutional]
    size=1
    stride=1
    pad=1
    filters=40
    activation=linear

    [region]
    anchors = 1.08,1.19,  3.42,4.41,  6.63,11.38,  9.42,5.11,  16.62,10.52
    
    ...
    ```

4. Change `labels.txt` to include the label(s) you want to train on (number of labels should be the same as the number of classes you set in `tiny-yolo-voc-3c.cfg` file). In our case, `labels.txt` will contain 3 labels.

    ```
    label1
    label2
    label3
    ```
5. Reference the `tiny-yolo-voc-3c.cfg` model when you train.

    `flow --model cfg/tiny-yolo-voc-3c.cfg --load bin/tiny-yolo-voc.weights --train --annotation train/Annotations --dataset train/Images`


* Why should I leave the original `tiny-yolo-voc.cfg` file unchanged?
    
    When darkflow sees you are loading `tiny-yolo-voc.weights` it will look for `tiny-yolo-voc.cfg` in your cfg/ folder and compare that configuration file to the new one you have set with `--model cfg/tiny-yolo-voc-3c.cfg`. In this case, every layer will have the same exact number of weights except for the last two, so it will load the weights into all layers up to the last two because they now contain different number of weights.


## Camera/video file demo

For a demo that entirely runs on the CPU:

```bash
flow --model cfg/yolo-new.cfg --load bin/yolo-new.weights --demo videofile.avi
```

For a demo that runs 100% on the GPU:

```bash
flow --model cfg/yolo-new.cfg --load bin/yolo-new.weights --demo videofile.avi --gpu 1.0
```

To use your webcam/camera, simply replace `videofile.avi` with keyword `camera`.

To save a video with predicted bounding box, add `--saveVideo` option.

## Using darkflow from another python application

Please note that `return_predict(img)` must take an `numpy.ndarray`. Your image must be loaded beforehand and passed to `return_predict(img)`. Passing the file path won't work.

Result from `return_predict(img)` will be a list of dictionaries representing each detected object's values in the same format as the JSON output listed above.

```python
from darkflow.net.build import TFNet
import cv2

options = {"model": "cfg/yolo.cfg", "load": "bin/yolo.weights", "threshold": 0.1}

tfnet = TFNet(options)

imgcv = cv2.imread("./sample_img/dog.jpg")
result = tfnet.return_predict(imgcv)
print(result)
```


## Save the built graph to a protobuf file (`.pb`)

```bash
## Saving the lastest checkpoint to protobuf file
flow --model cfg/yolo-new.cfg --load -1 --savepb

## Saving graph and weights to protobuf file
flow --model cfg/yolo.cfg --load bin/yolo.weights --savepb
```
When saving the `.pb` file, a `.meta` file will also be generated alongside it. This `.meta` file is a JSON dump of everything in the `meta` dictionary that contains information nessecary for post-processing such as `anchors` and `labels`. This way, everything you need to make predictions from the graph and do post processing is contained in those two files - no need to have the `.cfg` or any labels file tagging along.

The created `.pb` file can be used to migrate the graph to mobile devices (JAVA / C++ / Objective-C++). The name of input tensor and output tensor are respectively `'input'` and `'output'`. For further usage of this protobuf file, please refer to the official documentation of `Tensorflow` on C++ API [_here_](https://www.tensorflow.org/versions/r0.9/api_docs/cc/index.html). To run it on, say, iOS application, simply add the file to Bundle Resources and update the path to this file inside source code.

Also, darkflow supports loading from a `.pb` and `.meta` file for generating predictions (instead of loading from a `.cfg` and checkpoint or `.weights`).
```bash
## Forward images in sample_img for predictions based on protobuf file
flow --pbLoad built_graph/yolo.pb --metaLoad built_graph/yolo.meta --imgdir sample_img/
```
If you'd like to load a `.pb` and `.meta` file when using `return_predict()` you can set the `"pbLoad"` and `"metaLoad"` options in place of the `"model"` and `"load"` options you would normally set.

That's all.
