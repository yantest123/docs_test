title: How To Boot Into Upgrade Mode
---

There are 5 ways to boot into Upgrade Mode:

1. Keys Mode (Side-Buttons)
2. Serial Mode
3. Linux/Android Command Line
4. TST Mode (Recommended)
5. MRegister Mode

Usually, the first 4 methods will meet the needs of most users. In exceptional cases, for example you've burned the incorrect U-Boot, or your device can't boot at all, you can use method 5: MRegister.

## Keys Mode (U-Boot is Running Normally)
1. Power on Edge.
2. Long press the `Function` key without releasing it.
3. Short press the ‘Reset’ key and release it.
4. Count for 2 to 3 seconds, then release the ‘Function’ key to enter into Upgrade Mode. You will see the sys-led turn ON when you've entered Upgrade Mode (Loader Mode).

## Serial Mode (For Developers)
1. Refer this [guide](/linux/edge/SetupSerialTool.html) to setup your serial tool for Edge.
2. Once again, make sure you've done the correct connections and setup.
3. Hit any keys at the moment of bootup to stop autoboot. This step will let Edge boot into U-Boot Mode.
4. Type `run update` in the terminal of U-Boot as below. You will see the sys-led turn ON when you've entered Upgrade Mode.

```sh
kedge# run update
```
5. Type `run maskrom` on the terminal of U-Boot as below, and you will enter Maskrom Mode.

```sh
kedge# run maskrom
```

## Linux Command Line

1. Refer to this [guide](/linux/edge/SetupSerialTool.html) to setup your serial tool for Edge.
2. Once again, make sure you've done the correct connections and setup.
3. Boot into Android or Linux command line.
4. For Linux, execute `sudo reboot loader`. For Android, execute `su` and `reboot loader`. The system will reboot and enter Upgrade Mode. You will see the sys-led turn ON when you've entered Upgrade Mode (Loader Mode).

## TST Mode (Recommended)

1. Power-on Edge.
2. Quickly press the `Function` key 3 times in 2 seconds, then release the key.
3. You will see the Power-LED (Blue) blink for about 3 seconds. After the Power-LED (Blue) turns OFF, this indicates that the board is in Upgrade Mode (Maskrom Mode).

## MRegister Mode(Maskrom Mode)

1. Power-on Edge.
2. Use a tweezer to short-circuit the two pads of `M` register, then without releasing...
3. Short press the `Reset` key and release it to boot into Upgrade Mode (Maskrom Mode).

![Image of MRegister_ShortCircuit](/linux/images/edge/MRegister_ShortCircuit.png)

{% note info Tip %}
The `M` register is located on the backside of Edge
{% endnote %}
