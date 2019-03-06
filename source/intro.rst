.. sectionauthor:: Михаил Гусев <mikhail.gusev@nextgis.ru>

.. _ngfb_intro:

Введение
========

.. _ngfb_purpose:

Назначение программы
--------------------

Программа **NextGIS Formbuilder** (Редактор форм NextGIS) предназначена для создания, редактирования и настройки форм, используемых в NextGIS Mobile для полевого сбора данных.

Документация описывает NextGIS Formbuilder версии 3.0.

.. _ngfb_launch_conditions:

Лицензия
--------

.. only:: html

   Программа распространяется под лицензией :ref:`GPL v.2 <ngm_gplv2>`.

.. only:: latex

   Программа распространяется под лицензией `GPL v.2 <http://docs.nextgis.ru/docs_ngmanager/source/appendix.html#ngm-gplv2>`_.


Рекомендуемые параметры системы
-------------------------------

Рекомендуемые параметры системы: ОС Windows XP/7/10; ОС Ubuntu Linux; 50 Мб свободного пространства на жёстком диске.

.. _ngfb_run:

Установка и запуск
------------------

Для Windows: скачайте единый установщик программ NextGIS по адресу http://nextgis.ru/nextgis-formbuilder/ и запустите. Следуйте шагам мастера установки. После установки запустите появившийся ярлык на рабочем столе или в меню Пуск.

Для Ubuntu Linux с версии 18.04:

.. code-block:: bash

   sudo apt-get install software-properties-common python-software-properties
   sudo apt-add-repository ppa:nextgis/ppa
   sudo apt-get install formbuilder
   fb
