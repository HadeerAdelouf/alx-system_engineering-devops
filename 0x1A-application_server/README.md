0x1A. Application server
========================

*For this project, students are expected to look at these concepts:*

- [Web Server](https://alx-intranet.hbtn.io/concepts/17)
- [Server](https://alx-intranet.hbtn.io/concepts/67)
- [Web stack debugging](https://alx-intranet.hbtn.io/concepts/68)

![](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/9/c7d1ed0a2e10d1b4e9b3.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20220509%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220509T135639Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=18505e64c5c07265783b06401b75fba59864a9f8223831a31b28266d77c53490)

Background Context
------------------

[![](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2019/6/2ea1058f813d42c61f48.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20220509%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220509T135639Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=b40c3812be5b4f33861ec32c6b25c94d1c41ed57cfb155c3711676f6a4f0f627)](https://youtu.be/pSrKT7m4Ego)[](http://savefrom.net/?url=https%3A%2F%2Fyoutu.be%2FpSrKT7m4Ego&utm_source=userjs-chrome&utm_medium=extensions&utm_campaign=link_modifier "Obtenir un lien direct")

Your web infrastructure is already serving web pages via `Nginx` that you installed in your [first web stack project](https://alx-intranet.hbtn.io/rltoken/95oRNZ-zRGwLxtWECJqsWA "first web stack project"). While a web server can also serve dynamic content, this task is usually given to an application server. In this project you will add this piece to your infrastructure, plug it to your `Nginx` and make is serve your Airbnb clone project.

Resources
---------

**Read or watch**:

- [Application server vs web server](https://alx-intranet.hbtn.io/rltoken/B9fOBzIxX_t1289WAuRzJw "Application server vs web server")
- [How to Serve a Flask Application with Gunicorn and Nginx on Ubuntu 16.04](https://alx-intranet.hbtn.io/rltoken/kpG6RwmwRJHzRmGUM_ERcA "How to Serve a Flask Application with Gunicorn and Nginx on Ubuntu 16.04") (As mentioned in the video, do **not** install Gunicorn using `virtualenv`, just install everything globally)
- [Running Gunicorn](https://alx-intranet.hbtn.io/rltoken/2LF1j7xKJGYaUtD1HKgUeQ "Running Gunicorn")
- [Be careful with the way Flask manages slash](https://alx-intranet.hbtn.io/rltoken/lEg0zpkkDcLtdl3VD4ACRQ "Be careful with the way Flask manages slash") in [route](https://alx-intranet.hbtn.io/rltoken/Zn8fYk-U9YRm7Z5Coqqb0g "route") - `strict_slashes`
- [Upstart documentation](https://alx-intranet.hbtn.io/rltoken/mcEsKqFsjJA3tHAjiMknaw "Upstart documentation")
