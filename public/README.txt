Scroll down for English language


UA
==

Як налаштувати перемикання каналів відео в повітрі
==================================================

Betaflight:
-----------

Перевір, що Betaflight firmware правильної версії, для цього в CLI виконай команду: 'version'
    > version
вона повинна містити:
    # +custom VTX channel switch
(або, у вас своя прошивка і там є ця можливість)


ELRS TX
-------

Перейдіть до VTX Admin:

Band (тут F) і Channel (тут 1) є діапазоном і каналом за замовчуванням, ви можете змінити їх як забажаєте.
VtxSecondary - перемикач, який керує альтернативними відеоканалами.
AUX1 - CH5, AUX2 - CH6 і так далі. напр. для каналу 10 це буде AUX6
AltCh/AltBand - альтернативні діапазони та канали для перемикання. Їх 5 штук.
Залежно від значення VtxSecondary канал відео буде перемикатися на один із них.


   PWM               номер каналу
------------------------------------
  1000-1166 | за замовчуванням (Band, Channel)
  1167-1333 | AltCh/AltBand 0
  1334-1500 | AltCh/AltBand 1
  1501-1666 | AltCh/AltBand 2
  1667-1833 | AltCh/AltBand 3
  1834-2000 | AltCh/AltBand 3

Якщо будь-який AltBand не встановлено, він дорівнюватиме стандартному діапазону/каналу за замовчуванням, тому бажано встановити усі значення AltCh/AltBand навіть якщо вони однакові.

Дрон повинен мати дзеркальні налаштування у cli, якщо ELRS телеметрія не використовується.




EN
==


HOWTO Setup Video channels switching
====================================

Betaflight:
-----------

Check that Betaflight firmware is correct. For this enter CLI and enter 'version' command:
    > version
it should contain:
    # +custom VTX channel switch
(or you are using your own Betaflight firmware with this ability)

ELRS TX
-------

Go to VTX Admin:

Band (here F) and Channel (here 1) is the default band and channel, you can change it as you want. 
VtxSecondary - is the switch which controls alternative video channels.
AUX1 - CH5, AUX2 - CH6, and so on. e.g. for channel 10 it will be AUX6
AltCh/AltBand - are alternative bands and channels to switch to. There are 4 of them.
Depending on the value of VtxSecondary channel video will be switched to one of them.


   PWM             Channel Number 
----------------------------------
1000-1166 | default (Band, Channel)
1167-1333 | AltCh/AltBand 0
1334-1500 | AltCh/AltBand 1
1501-1666 | AltCh/AltBand 2
1667-1833 | AltCh/AltBand 3
1834-2000 | AltCh/AltBand 3

	
If any AltBand is not set it will be equal to the default Band/Channel.

Drone should have similar settings in cli, if ELRS telemetry is not used.









