..  Copyright (c) 2014-present PlatformIO <contact@platformio.org>
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
       http://www.apache.org/licenses/LICENSE-2.0
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

.. _platform_maxim32:

Maxim 32
========

:Configuration:
  :ref:`projectconf_env_platform` = ``maxim32``

Maxim's microcontrollers provide low-power, efficient, and secure solutions for challenging embedded applications. Maxim's processors embed cutting-edge technologies to secure data and intellectual property, proven analog circuitry for real-world applications, and battery-conserving low power operation.

For more detailed information please visit `vendor site <https://www.maximintegrated.com/en/products/digital/microcontrollers.html?utm_source=platformio&utm_medium=docs>`_.

.. contents:: Contents
    :local:
    :depth: 1


Examples
--------

Examples are listed from `Maxim 32 development platform repository <https://github.com/platformio/platform-maxim32/tree/master/examples?utm_source=platformio&utm_medium=docs>`_:

* `mbed-blink <https://github.com/platformio/platform-maxim32/tree/master/examples/mbed-blink?utm_source=platformio&utm_medium=docs>`_
* `mbed-serial <https://github.com/platformio/platform-maxim32/tree/master/examples/mbed-serial?utm_source=platformio&utm_medium=docs>`_
* `mbed-rtos <https://github.com/platformio/platform-maxim32/tree/master/examples/mbed-rtos?utm_source=platformio&utm_medium=docs>`_
* `mbed-events <https://github.com/platformio/platform-maxim32/tree/master/examples/mbed-events?utm_source=platformio&utm_medium=docs>`_
* `mbed-dsp <https://github.com/platformio/platform-maxim32/tree/master/examples/mbed-dsp?utm_source=platformio&utm_medium=docs>`_

Debugging
---------

:ref:`piodebug` - "1-click" solution for debugging with a zero configuration.

.. contents::
    :local:


Tools & Debug Probes
~~~~~~~~~~~~~~~~~~~~

Supported debugging tools are listed in "Debug" column. For more detailed
information, please scroll table by horizontal.
You can switch between debugging :ref:`debugging_tools` using
:ref:`projectconf_debug_tool` option in :ref:`projectconf`.

.. warning::
    You will need to install debug tool drivers depending on your system.
    Please click on compatible debug tool below for the further instructions.


On-Board Debug Tools
^^^^^^^^^^^^^^^^^^^^

Boards listed below have on-board debug probe and **ARE READY** for debugging!
You do not need to use/buy external debug probe.


.. list-table::
    :header-rows:  1

    * - Name
      - MCU
      - Frequency
      - Flash
      - RAM
    * - :ref:`board_maxim32_max32600mbed`
      - MAX32600
      - 24MHz
      - 256KB
      - 32KB


External Debug Tools
^^^^^^^^^^^^^^^^^^^^

Boards listed below are compatible with :ref:`piodebug` but **DEPEND ON**
external debug probe. They **ARE NOT READY** for debugging.
Please click on board name for the further details.


.. list-table::
    :header-rows:  1

    * - Name
      - MCU
      - Frequency
      - Flash
      - RAM
    * - :ref:`board_maxim32_max32620fthr`
      - MAX32620FTHR
      - 96MHz
      - 2MB
      - 256KB
    * - :ref:`board_maxim32_max32620hsp`
      - MAX32620
      - 96MHz
      - 2MB
      - 256KB
    * - :ref:`board_maxim32_maxwsnenv`
      - MAX32610
      - 24MHz
      - 256KB
      - 32KB


Stable and upstream versions
----------------------------

You can switch between `stable releases <https://github.com/platformio/platform-maxim32/releases>`__
of Maxim 32 development platform and the latest upstream version using
:ref:`projectconf_env_platform` option in :ref:`projectconf` as described below.

Stable
~~~~~~

.. code-block:: ini

    ; Latest stable version
    [env:latest_stable]
    platform = maxim32
    board = ...

    ; Custom stable version
    [env:custom_stable]
    platform = maxim32@x.y.z
    board = ...

Upstream
~~~~~~~~

.. code-block:: ini

    [env:upstream_develop]
    platform = https://github.com/platformio/platform-maxim32.git
    board = ...


Packages
--------

.. list-table::
    :header-rows:  1

    * - Name
      - Description

    * - `framework-mbed <http://mbed.org?utm_source=platformio&utm_medium=docs>`__
      - mbed Framework

    * - `tool-jlink <https://www.segger.com/downloads/jlink/?utm_source=platformio&utm_medium=docs>`__
      - SEGGER J-Link Software and Documentation Pack

    * - `tool-pyocd <https://github.com/mbedmicro/pyOCD?utm_source=platformio&utm_medium=docs>`__
      - Open source python library for programming and debugging ARM Cortex-M microcontrollers using CMSIS-DAP

    * - `toolchain-gccarmnoneeabi <https://launchpad.net/gcc-arm-embedded?utm_source=platformio&utm_medium=docs>`__
      - gcc-arm-embedded

.. warning::
    **Linux Users**:

        * Install "udev" rules :ref:`faq_udev_rules`
        * Raspberry Pi users, please read this article
          `Enable serial port on Raspberry Pi <https://hallard.me/enable-serial-port-on-raspberry-pi/>`__.


    **Windows Users:**

        Please check that you have a correctly installed USB driver from board
        manufacturer


Frameworks
----------
.. list-table::
    :header-rows:  1

    * - Name
      - Description

    * - :ref:`framework_mbed`
      - The mbed framework The mbed SDK has been designed to provide enough hardware abstraction to be intuitive and concise, yet powerful enough to build complex projects. It is built on the low-level ARM CMSIS APIs, allowing you to code down to the metal if needed. In addition to RTOS, USB and Networking libraries, a cookbook of hundreds of reusable peripheral and module libraries have been built on top of the SDK by the mbed Developer Community.

Boards
------

.. note::
    * You can list pre-configured boards by :ref:`cmd_boards` command or
      `PlatformIO Boards Explorer <https://platformio.org/boards>`_
    * For more detailed ``board`` information please scroll the tables below by
      horizontally.

Maxim
~~~~~

.. list-table::
    :header-rows:  1

    * - Name
      - Debug
      - MCU
      - Frequency
      - Flash
      - RAM
    * - :ref:`board_maxim32_max32620fthr`
      - External
      - MAX32620FTHR
      - 96MHz
      - 2MB
      - 256KB
    * - :ref:`board_maxim32_max32625mbed`
      - No
      - MAX32625
      - 96MHz
      - 512KB
      - 160KB
    * - :ref:`board_maxim32_max32625nexpaq`
      - No
      - MAX32625
      - 96MHz
      - 512KB
      - 160KB
    * - :ref:`board_maxim32_max32625pico`
      - No
      - MAX32625
      - 96MHz
      - 512KB
      - 160KB
    * - :ref:`board_maxim32_max32600mbed`
      - On-board
      - MAX32600
      - 24MHz
      - 256KB
      - 32KB
    * - :ref:`board_maxim32_max32620hsp`
      - External
      - MAX32620
      - 96MHz
      - 2MB
      - 256KB
    * - :ref:`board_maxim32_max32630fthr`
      - No
      - MAX32630
      - 96MHz
      - 2MB
      - 512KB
    * - :ref:`board_maxim32_maxwsnenv`
      - External
      - MAX32610
      - 24MHz
      - 256KB
      - 32KB

Sigma Delta Technologies
~~~~~~~~~~~~~~~~~~~~~~~~

.. list-table::
    :header-rows:  1

    * - Name
      - Debug
      - MCU
      - Frequency
      - Flash
      - RAM
    * - :ref:`board_maxim32_sdt32620b`
      - No
      - MAX32620IWG
      - 96MHz
      - 2MB
      - 256KB
    * - :ref:`board_maxim32_sdt32625b`
      - No
      - MAX32625ITK
      - 96MHz
      - 512KB
      - 160KB
