---
slug: ithodaalderop
title: ithodaalderop ventilation and heat pump units
authors: [kolsha]
tags: [notes, ithodaalderop]
---

# How to deal with ventilation and heat pump from ithodaalderop?

Are you a *lucky* owner of these systems and you have no clue how to deal with them? \
Me too, but no worries, I've got you covered.

<!-- truncate --> 


## the setup
In my case, the setup is as follows:
- [WTW-unit HRU ECO 300](https://www.ithodaalderop.nl/nl-NL/consument/product/03-00501)
- [Spider WP Klimaatthermostaat](https://www.ithodaalderop.nl/nl-NL/consument/product/03-00476)
- [Ventilatie sensor RFT CO2](https://www.ithodaalderop.nl/nl-NL/professional/product/04-00045)
- heat pump, to be updated, luckily I have not had problems with it yet



## tldr;

if you have any questions, you can use google ai studio to find and explain the answers from the manuals of the units. You need to upload the manual to the chat and ask your question.
But I've saved you the hassle and created [a chat template](https://aistudio.google.com/prompts/18LZIxRULT4wbjusA5lTme_invrmRUSAk) for you to use.


[![](/img/ithodaalderop-chat-tpl.png)](https://aistudio.google.com/prompts/18LZIxRULT4wbjusA5lTme_invrmRUSAk)


## Other useful links

### Connect spider wp to the ventilation unit

Follow this [youtube video](https://www.youtube.com/watch?v=OM4BM4I3ybE) to connect the spider wp to the ventilation unit.
But before you need to put the ventilation unit in the "pairing" mode.

Go to your main HRU ECO 300 unit.

1.  On the control panel, navigate to the **Communicatie** (Communication) menu (with the wireless icon  <FAIcon icon="fa-wifi" size="1x" />).
2.  Select the **LEARN** option.
3.  A **2-minute timer** will start on the HRU display. You now have two minutes to pair the sensor.


### Connect bathroom controller to the ventilation unit

Put the ventilation unit in the "pairing" mode.
Follow this [youtube video](https://www.youtube.com/watch?v=PdmUXEkXt0w) to connect the bathroom controller to the ventilation unit.


### Connect rft co2 sensor to the ventilation unit



**Before you begin:** You must put your main ventilation unit into pairing mode first. This process is described in the manual for the ventilation unit itself, not the sensor. You have 2 minutes to complete the following steps after putting the ventilation unit in pairing mode.

Here are the steps for the CO2 sensor:

1.  **Power on the Sensor:**
    *   Attach the front cover of the sensor to the wall-mounted base. This will supply power to the unit.
    *   Upon startup, the green LEDs will flash 3 times, and then the status light will turn solid **red**.

2.  **Initiate Pairing Mode:**
    *   Press and hold the main touch button on the sensor for **5-7 seconds**.
    *   Release the button when the status LED turns **white**. The sensor is now sending a pairing signal to the ventilation unit.

3.  **Check the Pairing Status:**
    The status LED will start flashing to indicate the result:

    *   **Flashing GREEN (1x per second):** Pairing was successful with a strong signal. The ventilation unit will briefly speed up to confirm.
    *   **Flashing ORANGE (1x per second):** Pairing was successful, but the signal is moderate. The ventilation unit will also briefly speed up to confirm.
    *   **Flashing RED (1x per second):** Pairing has failed.

**If pairing fails:** You must repeat the entire procedure from the beginning, starting with putting the ventilation unit back into pairing mode.