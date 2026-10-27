# uSDX
Firmware for a Chinese clone of the uSDX transceiver, featuring support for the Cyrillic script and minor enhancements.

Two interface languages ​​(RU/EN).

Panoramic display (panadapter):
16 points, +/- 8, 16, or 32 kHz; the audio output is intermittent, signaling the center frequency.
Encoder: used for tuning. A long press triggers a "preview" mode (scanning pauses, and the audio becomes continuous); a short press exits the mode and sets the frequency.
Buttons: exit the mode without changing the frequency.

Auto-scan:
Direction: based on the last direction of encoder rotation; uses the current step size; the threshold is set in menu 10.4.
Activation: double-press the "menu" button.
Works in all modes, as the signal level is measured from the raw I/Q data prior to demodulation.

Displays the current band instead of the "uSDX" label.

Frequency memory for each band.

Encoder acceleration.

Double-pressing the encoder switches to the next/previous band.

Holding the "menu" button while rotating the encoder changes the tuning step; holding the "mode" button while rotating the encoder changes the modulation mode.

Flash via a programmer (ISP/USBasp) without a bootloader ("MiniCore - No bootloader" setting) and with LTO (Link Time Optimization) enabled.

Since I am using an 8-band transceiver, I have limited the frequency range to 3.5–29.7 MHz. This can be easily modified in the code.

================== Rus/Русский

Два языка интерфейса (ru/en). 

Панрама: 
16 точек, +/- 8, 16 или 32 кГц, звук прерывестый транслирует сигнал цнтральной частоты; 
Энкодер - перестройка, долгое нажатие - "предпросмотр" (сканирование прерывается, звук ровный), короткое выход с установкой частоты;
Кнопки - просто выход без перестройки. 

Автопоиск: 
Направление - последнее направление вращения энкодера, шаг текущий, порог выставляется в меню 10.4;
Запуск - двойное нажатие кнопки "меню";
Работать во всех режимах, т.к. уровень измеряется по сырым I/Q до демодуляции.

Вместо надписи uSDX индекация текущего диапазона. 

Запоминание частоты для каждого диаппазона. 

Ускорение энкодера. 

Двойное нажатие энкодера переход на следующий/предыдущий диапазон. 

Удержание нажатой кнопки "menu" и вращение энкодера меняет шаг настройки, удержание кнопки "mode" и вращение энкодера - модуляция. 

Шить через программатор (ISP/USBasp) без загрузчика (MiniCore - No bootloader) и с LTO.

Т.к. у меня 8 диапазонный трансивр, то частоты ограничел с 3,5 по 29,7 МГц. Легко меняется в коде. 
