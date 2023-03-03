==============
pyzentao-specs
==============

``pyzentao-specs`` 包含了 `pyzentao <https://github.com/philip1134/pyzentao>`__ 的
禅道API规格文件，在 ``pyzentao r0.4.0`` 版本之后不再维护规格文件，转由本项目更新。


用法
----

下载
~~~~

.. code:: text

    git clone https://github.com/philip1134/pyzentao-specs.git

复制
~~~~

根据你的禅道版本，将对应的规格文件夹复制到你的业务项目目录下，例如你家在用禅道17.6版：

.. code:: text

    cp -r pyzentao-specs/v17.6 /path/to/my/project/pyzentao-specs

使用
~~~~

初始化 pyzentao 对象

.. code:: python

    import pyzentao

    zentao = pyzentao.Zentao({
        "url": "http://my.zentao.site/zentao",
        "username": "admin",
        "password": "123456",
        "spec": "/path/to/my/project/pyzentao-specs/v17.6"
    })

如果需要支持新的禅道版本，可以提 issue，也可以使用 `miaou <https://github.com/philip1134/miaou>`__
自助生成规格文件。
