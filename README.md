# midino
In this repository you will find a `.py` (**Python**) file that converts a `.mid` (**MIDI**) file to a `.ino` (*Arduino*) file that plays the song using a buzzer.
There are also samples for **.mid** and **.ino** files for
- __Megalovania__[^1][^2] (from Undertale) - by *Toby Fox🦊*
- __sans.__ (from Undertale) - by *Toby Fox🦊*
- __Driftveil City__ (from Pokémon Black & White, "Toothless Dance") - by *Hitomi Sato*
- __Jerk it out__[^1] - by *Caesars Palace*
- __The best song of the universe__ - by *Kcir Yeltsa*

[^1]: These samples have two files, one for the melody, and another one for the accompainment, if you connect the **A0** pin from an Arduino to the **A1** pin of another one, and vice versa, and put both `.ino` files on these, they will sync and play the song together. I have still not added this feature to the conversion, but you can manually add it by adding the lines of the sample file to your song.

[^2]: Wanna have a bad time? - Sans (from Undertale)
## Tips & Tricks
> [!NOTE]
> This code plays the *highest* note at each moment, so if a note in the melody is not the highest one, it will not play.

> [!NOTE]
> If your song is too long it won't compile. (The Megalovania accompainment uses ***~75%*** of the available space in my Arduino Uno R3 x_x)

> [!TIP]
> I personally recommend downloading from Musescore as a `.mscz` (**Musescore score**) file and then just remove everything but the melody. If you aren't willing to pay a Musescore subscription, you can download Musescore 3 and open a tab with the song you want to transcribe and copy the melody. [^3]
> Save the file on the same folder from which you run the script, and when inputting file names, the file extension is unnecessary. (If the file is named `Megalovania.mid` input `Megalovania`)

> [!TIP]
> If instead of connecting a buzzer to the Arduino you connect a motor, by bringing the motor close to your ear you will also hear the song play.

> [!IMPORTANT]
> Make sure that you have downloaded the ***Mido*** Python library. `pip install mido`

[^3]: Well, obviously, if you are doing the accompainment remove the, melody 🙄. It should technically be possible to connect three Arduinos, or various buzzers to the same arduino, but I don't own that much Arduinos nor buzzers. :(
