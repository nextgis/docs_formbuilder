.. sectionauthor:: Михаил Гусев <mikhail.gusev@nextgis.ru>

.. _ngfb_intro:

Введение
========

.. _ngfb_purpose:

Назначение программы 
--------------------

Программа **NextGIS Formbuilder** (Редактор форм NextGIS) предназначена для работы с формами сбора данных, используемых в NextGIS Mobile. Formbuilder позволяет создавать, редактировать и настраивать формы, состоящие из элементов (виджетов), используемых для ввода атрибутивной информации объектов слоя. В основе любого проекта Formbuilder лежит слой данных, который упаковывается вместе с формой в файл формата .ngfp, после чего он может быть отправлен на Android-устройство для использования в NextGIS Mobile.

Документация описывает NextGIS Formbuilder версии 2.1.

.. _ngfb_launch_conditions:

Лицензия
---------

Программа распространяется под лицензией :ref:`GPL v.2 <ngm_gplv2>`.

Рекомендуемые параметры системы
-------------------------------

Рекомендуемые параметры системы: ОС Windows XP/Vista/7; ОС Ubuntu Linux; 48 Мб свободного пространства на жёстком диске.

.. _ngfb_run:

Установка и запуск
------------------

Для Windows: скачайте установочный файл программы по адресу http://nextgis.ru/nextgis-formbuilder/ и запустите. Следуйте шагам мастера установки. Запустите появившийся ярлык на рабочем столе или в меню Пуск.

Для Ubuntu Linux: 

.. code-block:: bash

   sudo apt-get install software-properties-common python-software-properties
   sudo apt-add-repository ppa:nextgis/ppa
   sudo apt-get install formbuilder
   fb
