Project: midi-player-v2
Authors: David Barnes and Michael Kölling

This project is part of the material for the book

   Objects First with Java - A Practical Introduction using BlueJ
   Seventh edition
   David J. Barnes and Michael Kölling

It is discussed in chapter 3.

In this version, the TuneCreator class can be used to create and play a  
simple demo tune.


Question of Part 3

41: I can see the notes and duration when i call showNote method. Yes, it's possible to play this on a piano.
43: Yes, you can play more than once by passing the SimpleTune object.
45: public void playNote (inernal)
    public void showInstruments (external)
51:
public ClockDisplay()
{
    hours = new NumberDisplay(24);
    minutes = new NumberDisplay(60);
    long millis = System.currentTimeMillis();
    long seconds = millis / 1000;
    int currentMinutes = (int) (seconds / 60 % 60);
    int currentHours   = (int) (seconds / (60 * 60) % 24);
    hours.setValue(currentHours);
    minutes.setValue(currentMinutes);

    updateDisplay();
}
52:

public String getDisplayValue() 
{
    return String.format("%02d", value);
}
It gives the same results as the other one.
54: Breaking point is already there.
58: simpleTune class and addNote method.
When I step , you can see the notes and the durations and after it goes away.

